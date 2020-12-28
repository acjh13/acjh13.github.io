---
title: "Postmortem: Kindred"
toc: true
categories:
  - blog
tags:
  - postmortem
---

**DISCLAIMER**: This is a *personal* postmortem from the viewpoint of the game's Producer, Andrew Chong. All thoughts are his own.

# Overview
Kindred is a 3rd Person Narrative Platformer developed by Arctic Studios as part of the GAM300/350 module at DigiPen Singapore. For a more detailed overview of Kindred and my roles in the project, click [here]({% link _projects/kindred.md %}). This postmortem describes what went right and what went wrong with the development of the game.  
  
  
# What Went Right
## Many initial game pitches and prototypes
I was extremely happy with the pre-production process our team had early on. In the prior semester, the team would gather throw out various ideas on what would be feasible to develop.
  
We probably had about 10 different ideas (strangely 3 of them involved food) and there was a lot of discussion during the pre-production meetings on the potential of each idea, what unique spin we could do on certain genres, which could be fun etc...
  
We ended up with 3 strong ideas that we prototyped (on paper and in Unity) and pitched them to different lecturers. In the end, a narrative-based prototype stood out from the rest and it was further trimmed down into what eventually became Kindred.

## Inter-discipline Pipelines
While this point may not seem like anything major, I'm extremely proud of how each department of the team managed to work together smoothly with the help of some workflows/pipelines.  
These pipelines included:  
- Narrative & Design & Art  
The narrative designer, level designer and art team would work together and develop iterations of the level. First the narrative designer would communicate the general look of the level to the level designer and what part of the story the level would take place in.  
Following this, the level designer would blockout the level and communicate the key locations of level to the art team. The art team would then create assets befitting the level's location and start to populate the level.
- Art & Editor  
The art team learnt how to use the level editor and was able to not only test models/animations and create effects by themselves, but also independently work on populating the levels with environmental props once the level design was complete.
- Design & Tech  
The design team was able to work independently of the technical team when they were scripting behaviours for the game's mechanics. The technical team would layout guidelines on how to use the different parts of the engine, while the designers would report any bugs encountered with a standardised bug report template.  
Designers could also request certain features to be exposed to the scripting system and the respective programmer would do so or present a work-around.  

## Constant Feedback
With Kindred being a narrative focused game with some puzzle elements, there were several key elements we had to get right. These included the story, level/puzzle design and the overall visual style of the game. While majority of the praise must be directed to my team for pushing the game to what it is, it would be amiss if I did not mention the numerous play-testers and consultants from the other student teams and the faculty.  
  
To be totally honest, almost half of the school's faculty had weighed in on various parts of Kindred. We approached lecturers who were experts in level design, cinematic design, story design and visual design, incorporating all their advice/criticisms/complaints into team meetings where we discussed how to apply them. 
  
Our fellow students also helped us out greatly, as we received advice regarding puzzle design, audio design and dialogue while also observing their responses during playtest sessions.

## (Personal) Assisted in overseeing game's direction
On a personal note, I feel like I've learnt a lot about working on narrative design, cinematics and game directing. With the game being based on a past version of Singapore, we had to ensure that the environment looked the part, characters sounded the part and have a story that would resonate in some capacity with our players. This meant there had to be a lot of research done as part of pre-production and any details that were "off" could affect the game greatly.  
  
Working with the narrative designer also made me extremely aware of how to pace the game, when to have low points and when to have high points - and whether these points should be a cutscene or a passing voice over or incorporated into the game's puzzles.  
  
Similarly, learning to build cinematics was also a totally new experience for me. I had to identify landmarks in the level, script interesting moments and figure out how to create smooth cutscenes that didn't confuse the player. A lot of time was spent watching cutscenes in AAA games and then attempting to emulate them in the game.  
  
In terms of directing the game, I'd say that there were many discussions where the team would talk about how certain scenes should play out and it was a iterative process where the scene would sound good on paper but wouldn't play out as well in-game. As development went on, I was generally able to take note of minor details that would make or break a scene and be able to give suggestions or implement changes early to ensure a higher quality outcome.
  
  
# What Went Wrong
## Story underwent many changes
It's natural that a narrative focused game would have had its narrative undergone many changes before its fully developed. In the case of Kindred however, there was simply much lesser time available to develop the story due to is being a school project. As mentioned before, the initial prototype was completely different than the final product and the story that made it into the final game only began to develop when the project was ~40% complete. Over the semester break, the story was completely revamped, and we began to use it as a baseline that the level designer and art team could work off.  
  
By this point, we were already fairly off-schedule and were having almost daily conversations about story changes as we had playtest sessions and lecturer consultations. This is most obviously seen towards the end of the game, where we had trouble combining the level design and the final arc of the game into the last level.  
  
More troubling was the fact that with story changes came dialogue changes. New lines had to be recorded, the recording booth had to be booked (in an already busy semester with other projects needing to use it too) and old lines needing to be re-recording to adjust for tone and potential new lines coming in. This was one of the major areas that I failed to take note of as a producer and unfortunately caused a lot of distress for the team and weakened the game overall.

## Technical Issues
While the game engine that Kindred runs on ("Arctic Engine" as we called it) is extremely well-done, there were several oversights that slowed down development momentum considerably.  
Most notably were:  
- Serialization System  
The system was a custom done "JSON"-like system that would save every object with its various components into human-readable files for level or prefab loading. The system had to be manually updated whenever new components or variables were introduced and was usually up to the respective engineer to add them in.  
Late in development, there were some major changes to how some components worked. This would have been fine, except that the serialization system was not updated. This led to almost all our levels not being able to load and mass confusion within the team. While most of it was fixed within a week or so, a lot of valuable work had to be re-done.
- Parenting System  
While not a major feature by any means, it was overlooked until the team noticed that moving chunks of the level around was extremely time-consuming. This was because the art team had placed each object on its own and shifting say a building involved shifting every object inside it by hand. Once we attempted to parent smaller object to structures, we realised that the parenting system was buggy. While fixes were implemented, ultimately most objects were moved by hand.
- Cinematic Camera  
Although initially proposed as we knew that we would be developing cutscenes, it was eventually scrapped due to time constraints. This meant that other than the camera movement during cutscenes, the camera's facing direction was dictated by a custom script that, while functional, had a lot of room for improvement.

## Reserved Team Culture
An admittedly minor point in the grand scheme of things, the team's culture was fairly reserved and made it somewhat difficult to have proper discussions about the overall status of the game and its engine.  
  
Initially, it was difficult to get the designers to communicate their wants and needs to the programmers. When I attempted to act as a middleman, it made things worse as I would misinterpret intentions or get details wrong - facilitating miscommunication. In the end, the leads of each department setup a pipeline to better facilitate their discussions.  
  
I also made it a point to use proper meeting rooms (which I had to ask permission for from my lecturers), as it made the meetings more "proper" and removed distractions.

## (Personal) Not always level-headed 
As with any project, that will always be ups-and-downs. While developing Kindred, I had set out to try to have the smoothest development cycle possible, where crunch would not have to be forced - coming from a previously crunch heavy game project. However, with such an ambitious and complex project, there was a tight schedule to adhere to - with various internal milestones that had to be met to ensure the development cycle went off without a hitch.  
  
As project milestones approached and internal deadlines were not kept, I would become more moody, which led to me saying thorny or confrontational words to team members. This was extremely unprofessional and had a clear negative impact on the team morale. I'm extremely lucky to have a teammate pull me aside and set me straight. While I wouldn't say the rest of the project went off as planned, I did take note of my personal feelings and did my best to have team discussions to discuss solutions whenever there were missed deadlines or blockers affecting the team.  
  
This is a clear failure on my part that I, as a producer, was not level-headed. I feel like the learning point here is to be transparent with the team and look for alternative solutions rather than internalise and lash out.

# Conclusion
I'm extremely proud of my team and their efforts to produce a game that was conceptually ambitious and extremely difficult to pull off. I personally learnt a lot about the narrative/cinematic portions of game development and managing projects of a larger scale.  
  
While Kindred didn't manage to win any awards, I do believe that the entire team learnt a big deal from it, and it will make for an excellent portfolio piece.