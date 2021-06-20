---
title: "Postmortem: Kindred"
toc: true
categories:
  - blog
tags:
  - postmortem
---

**DISCLAIMER**: This is a *personal* postmortem from the viewpoint of the game's Producer, Andrew Chong. All thoughts are my own.

# Overview
Kindred is a 3rd Person Narrative Platformer developed by Arctic Studios as part of the GAM300/350 module at DigiPen Singapore. For a more detailed overview of Kindred and my roles in the project, click [here]({% link _projects/kindred.md %}). This postmortem describes what went right and what went wrong with the development of the game.  
  
  
# What Went Right
## Many initial game pitches and prototypes
I was extremely happy with the pre-production process our team had early on. In the prior semester, the team would gather throw out various ideas on what would be feasible to develop.
  
We probably had about 10 different ideas (strangely 3 of them involved food) and there was a lot of discussion during the pre-production meetings on the potential of each idea, what unique spin we could do on certain genres, which could be fun etc...
  
We ended up with 3 strong ideas that we prototyped (on paper and in Unity) and pitched them to different lecturers. In the end, a narrative-based prototype stood out from the rest, and it was further trimmed down into what eventually became Kindred.

## Inter-discipline Pipelines
While this point may not seem like anything major, I am extremely proud of how each department of the team managed to work together smoothly with the help of some workflows/pipelines.  
These pipelines included:  
- Narrative + Design + Art  
The narrative designer, level designer and art team would work together and develop iterations of the level.  
First, the narrative designer would communicate the general look of the level to the level designer and what part of the story the level would take place in.  
Next, the level designer would blockout the level and communicate the key locations of level to the art team.  
Finally, the art team would create assets befitting the level's theme and location, and start to populate the level.
- Art + Editor  
The art team learnt how to use the level editor and was able to not only test models/animations and create effects by themselves, but also independently work on populating the levels with environmental props once the level design was complete.
- Design + Tech  
The design team was able to work independently of the technical team when they were scripting behaviours for the game's mechanics.  
The technical team would layout guidelines on how to use the different parts of the engine, while the designers would report any bugs encountered with a standardised bug report template.  
Designers could also request certain features to be exposed to the scripting system and the respective programmer would do so or present a work-around.  

## Constant Feedback
With Kindred being a narrative focused game with puzzle elements, there were several key areas we had to get right. These included the story, level/puzzle design and the overall visual style of the game. While majority of the praise must be directed to my team for pushing the game to what it is, it would be amiss if I did not mention the numerous playtesters and consultants from the other student teams and DigiPen Singapore's faculty.  
  
To be totally honest, almost half of the school's faculty had weighed in on various parts of Kindred. We approached lecturers who were experts in level design, cinematic design, story design and visual design, incorporating all their feedback into team meetings where we discussed how to apply them. 
  
Our fellow students also helped us out greatly, as we received advice regarding puzzle design, audio design and dialogue while also being able to observe their responses during playtest sessions.

## (Personal) Assisted in overseeing game's direction
On a personal note, I learnt a lot about working on narrative design, cinematics and game directing. With the game being based on a past version of Singapore, we had to ensure that the environment looked the part, characters sounded the part and have a story that would resonate in some capacity with our players. This meant there had to be a lot of research done as part of pre-production and any details that were "off" could affect the game greatly.  
  
Working with the narrative designer also made me extremely aware of how to pace the game, when to have low points and when to have high points - and whether these points should be a cutscene or a passing voice over and whether it should be incorporated into the game's puzzles.  
  
Similarly, learning to build cinematics was also a totally new experience for me. I had to identify landmarks in the level, script interesting moments and figure out how to create smooth cutscenes that did guided the player. A lot of time was spent watching cutscenes in AAA games and then using similar techniques to achieve impactful cutscenes.  
  
In terms of directing the game, I'd say that there were many discussions where the team would talk about how certain scenes should play out and it was an iterative process where the scene would sound good on paper but would not play out as well in-game. As development progressed, I gradually got better at taking note of minor details that would make or break a scene and give suggestions or implement changes early to ensure a higher quality outcome.
  
  
# What Went Wrong
## Story underwent many changes
It is natural that a narrative focused game would have its narrative undergo many changes before its fully developed. In the case of Kindred however, there was simply much lesser time available to develop the story due to the inherent nature of it being a school project. As mentioned before, the initial prototype was completely different than the final product and the story that made it into the final game only began to take shape when the project was ~40% complete. Over a semester break, the story was completely revamped, and we began to use that as a baseline that the level designer and art team could work off.  
  
By this point, we were already fairly off-schedule and were having almost daily conversations about story changes between playtest sessions and lecturer consultations. This is most obvious towards the end of the game, where we had trouble combining the level design and the final arc of the narrative into the last level.  
  
More troubling was the fact that with story changes came dialogue changes. New lines had to be written and recorded, along with booking a session at the recording booth (in an already busy semester with other projects teams using it). Old lines also needed to be re-recorded to adjust for tone when new dialouge was added. This was one of the major areas that I failed to take note of as a producer and unfortunately caused a lot of distress for the team and weakened the game overall.

## Technical Issues
While the game engine that Kindred runs on ("Arctic Engine" as we called it) is extremely well-done, there were several oversights that slowed down development momentum considerably.  
Most notably:  
- Serialization System  
This system was a custom developed "JSON"-like system that would save every object with its various components into human-readable files for level or prefab loading. The system had to be manually updated whenever new components or variables were introduced and was usually up to the respective engineer to add them in.  
Late in development, there were some major changes to how some components worked. This would have been fine, except that the serialization system was not updated alongside that change. This led to almost all our levels not being able to load and mass confusion within the team. While most of it was fixed within a week or so, a lot of valuable work had to be re-done.
- Parenting System  
While not a major feature by any means, it was overlooked until the team noticed that moving large chunks of the level around was extremely time-consuming. This was because the art team had placed each object on its own and shifting a building also involved shifting every object inside it by hand. Once we attempted to parent smaller object to structures, we realised that the parenting system was buggy. While fixes were implemented, ultimately most objects were still moved by hand.
- Cinematic Camera  
Although initially proposed as we knew that our game would be cutscene-heavy, it was eventually scrapped due to time constraints. This meant that other than the camera movement during cutscenes, the camera's facing direction was dictated by a custom script that, while functional, had a lot of room for improvement.

## Reserved Team Culture
An admittedly minor point, the team's reserved culture made it difficult to have proper discussions about the overall status of the game and its engine.  
  
Initially, it was difficult to get the designers to communicate their wants and needs to the engineering team. When I attempted to act as a middleman, it made things worse as I would misinterpret intentions or get details wrong - causing miscommunication. In the end, the leads of each department setup a pipeline to better facilitate their discussions.  
  
I also made it a point to use proper meeting rooms (which I had to ask permission for from my lecturers), as it made the meetings more focused and minimized distractions.

## (Personal) Not always level-headed 
As with any project, there will always be ups-and-downs. While developing Kindred, I had set out to try to have the smoothest development cycle possible, where crunch would not have to be forced (my previous project was crunch heavy). However, with Kindred being such an ambitious and complex project, there was a tight schedule to adhere to - with various internal milestones that had to be met to ensure the development cycle went off without a hitch.  
  
As project milestones approached and internal deadlines were not kept, I would become moodier, which led to me saying thorny or confrontational words to team members. This was extremely unprofessional and had a clear negative impact on the team morale. I am extremely lucky to have a teammate pull me aside and set me straight. While I would not say the rest of the project went off as planned, I did take note of my personal feelings and did my best to have team discussions to discuss solutions whenever there were missed deadlines or blockers affecting the team.  
  
This is a clear failure on my part that I, as a producer, was not level-headed. I feel like the learning point here is to be transparent with the team and look for alternative solutions rather than to internalise the issue and potentially let it lash out.

# Conclusion
I am extremely proud of my team and their efforts to produce a game that was conceptually ambitious and extremely challenging to pull off. I personally learnt a lot about the narrative/cinematic portions of game development and managing projects of a larger scale.  
  
While Kindred did not manage to win any awards, I do believe that the entire team learnt a big deal from it, and that it will make for an excellent portfolio piece.