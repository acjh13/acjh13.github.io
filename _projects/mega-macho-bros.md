---
title: "Mega Macho Brothers"

# excerpt is what appears on the collections page
excerpt: "A 2D co-op action platformer where players fight off an alien invasion."

permalink: /projects/mega-macho-bros/

# the top overlay, contains a bg image, description and actions(links)
header:
  teaser:         /assets/images/projects/mmb/mmb.jpg
  overlay_image:  /assets/images/projects/mmb/mmb.jpg
  overlay_filter: 0.6 # the lower the more visible the image is
  #caption: "test caption" # appears at the bottom right of the overlay
  actions:
    - label:  "Download it at the DigiPen Games Gallery"
      url:    "https://games.digipen.edu/games/mega-macho-bros"
  #video:
  #  id: oB_Zaoc2pgY
  #  provider: youtube

# sidebar, holds info like Role(s), Responsibilities, Project Status
sidebar:
  - title:  "Role(s)"
    text:   "Producer, Programmer"

  - title:  "Responsibilities"
    text:   "Producer, Editor Programmer"
    
  - title:  "Project Status"
    text:   "Completed"

# gallery images
gallery:
    #- url:        /assets/images/projects/mmb/teaser.jpg
    #  image_path:  assets/images/projects/mmb/teaser.jpg
    #  alt: ""

    - url:        /assets/images/projects/mmb/title.png
      image_path:  assets/images/projects/mmb/title.png

    - url:        /assets/images/projects/mmb/1.png
      image_path:  assets/images/projects/mmb/1.png

    - url:        /assets/images/projects/mmb/2.png
      image_path:  assets/images/projects/mmb/2.png

    - url:        /assets/images/projects/mmb/3.png
      image_path:  assets/images/projects/mmb/3.png

    #- url:        /assets/images/projects/mmb/4.png
    #  image_path:  assets/images/projects/mmb/4.png

    #- url:        /assets/images/projects/mmb/5.png
    #  image_path:  assets/images/projects/mmb/5.png

# table of contents
toc: true

# for search function?
categories:
  - Projects

tags:
  - Action
  - Platformer
  - Shooter
  - GAM
  - DigiPen
  - Singapore
  - 2D

---

## Description

Mega Macho Brothers was a game developed as part of the GAM200/250 module at DigiPen Singapore. It was developed by a team of 7 full-time students over the course of ~ 6 months, including pre-production.

It is a 2D co-op action platformer where players take on the roles of Marko and Pedro as they fight off an alien invasion. Players can grab and throw their "Brothers" while defending the city from invading aliens.

## Gameplay Video

{% include video id="-3gB86JMQ-8" provider="youtube" %}

## Main Responsibilities

My main contributions to this project were as a Producer and Programmer.  

### Production

I managed a team of 7 members: 1 artist, 4 programmers and 2 designers. It was the first time I formally worked on a project as a Producer and while I learnt about about good practices, I also made a lot of mistakes along the way.

Initially, meetings were carried out in a "semi" *Agile* style, with entire team meetings only happening when a major feature/milestone was completed and I needed everyone's feedback on the next milestone. Once I realised that progress was difficult to track, I enforced weekly meetings that also served to keep members updated on progress of each department.

[HacknPlan](https://hacknplan.com/) was also used to help visualise the progress of features and bugs, helping tremendously in assessing how the project was progressing.

### Programming

On the Programming side, I worked on
- Entity manager
- Serialization
- Audio system
- Level editor, created with [Dear ImGui](https://github.com/ocornut/imgui) and had features like
    - Drag and drop for asset swapping
    - Nested tree view of the scene
    - AI editor interface for modifying enemy AI
- Gameplay mechanics

## Awards

### DigiPen Game Awards 2019

**Winner** - *Unity Best Sophomore Game*   
**Finalist** - *Best Music and Sound Design*   
**Finalist** - *Acronis Best Team Spirit* 

## Gallery

{% include gallery caption = "Screenshots from the game" %}

## Download

Check out the game at the [DigiPen Game Gallery](https://games.digipen.edu/games/mega-macho-bros).
