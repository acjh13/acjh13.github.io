---
title: "Kindred"

# excerpt is what appears on the collections page
excerpt: "A 3D narrative platformer where players relive old memories as Father and Son."

permalink: /projects/kindred/

# the top overlay, contains a bg image, description and actions(links)
header:
  teaser:         /assets/images/projects/kindred/teaser.jpg
  overlay_image:  /assets/images/projects/kindred/1.png
  overlay_filter: 0.6 # the lower the more visible the image is
  #caption: "test caption" # appears at the bottom right of the overlay
  actions:
    - label:  "Download it at the DigiPen Games Gallery"
      url:    "https://games.digipen.edu/games/kindred"
  #video:
  #  id: oB_Zaoc2pgY
  #  provider: youtube

# sidebar, holds info like Role(s), Responsibilities, Project Status
sidebar:
  - title:  "Role(s)"
    text:   "Producer, Programmer, Designer"

  - title:  "Responsibilities"
    text:   "Producer, Editor Programmer, Gameplay Designer / Programmer and Cinematics Designer"
    
  - title:  "Project Status"
    text:   "Completed"

# gallery images
gallery:
    #- url:        /assets/images/projects/kindred/teaser.jpg
    #  image_path:  assets/images/projects/kindred/teaser.jpg
    #  alt: ""

    - url:        /assets/images/projects/kindred/kindred.png
      image_path:  assets/images/projects/kindred/kindred.png

    - url:        /assets/images/projects/kindred/1.png
      image_path:  assets/images/projects/kindred/1.png

    - url:        /assets/images/projects/kindred/2.png
      image_path:  assets/images/projects/kindred/2.png

    - url:        /assets/images/projects/kindred/3.png
      image_path:  assets/images/projects/kindred/3.png

    - url:        /assets/images/projects/kindred/4.png
      image_path:  assets/images/projects/kindred/4.png

    - url:        /assets/images/projects/kindred/5.png
      image_path:  assets/images/projects/kindred/5.png

# table of contents
toc: true

# for search function?
categories:
  - Projects

tags:
  - Narrative
  - Platformer
  - GAM
  - DigiPen
  - Local Stories
  - Singapore
  - 3D

---

## Description

Kindred was a game developed as part of the GAM300/350 module at DigiPen Singapore. It was developed by a team of 11 full-time students over the course of ~9 months, including pre-production and post-production.

It is a 3D narrative platformer where players relive old memories as Father and Son. Playing as each character, they journey through old and warped memories and relive moments of their lives with one another.

## Gameplay Video

{% include video id="oB_Zaoc2pgY" provider="youtube" %}

## Main Responsibilities

My main contributions to this project were as a Producer and a Programmer/Designer.  

### Production

Production-wise I managed a team of 11: 3 artists, 6 programmers and 2 designers. It was a bigger team than I had previously managed and I had to quickly learn how to delegate tasks and responsibilities to the leads rather than tracking them myself.

I followed an *Agile and Scrum* management style, with weekly team meetings to discuss progress, prioritise upcoming tasks and generally as a sync-up point so the team was aware of the project's progress. I also integrated a *Kanban* approach to breaking down and viewing the various tasks of the different departments via Trello.

With a large team, I sought to setup pipelines between each departments, linking them to members of importance in other departments. For example, I worked with the Technical Lead/Scripting Programmer to setup a bug reporting system when the Design team would encounter issues with scripting behaviours.

I also ensured that each milestone's submission was of high quality and as bug-free as possible, QA testing the project at every submission.

### Programming

On the Programming side, I worked on
- Level editor, created with ImGui and had features like
  - Drag and drop for asset swapping
  - Undo/Redo manager
  - Nested tree view of the scene
- Locating and debugging engine-specific bugs.

### Design

On the Design side, I worked on
- Scripting gameplay mechanics
- Creating a dialogue and cinematics system
- Assisting with level design
- Designing all cutscenes

I also assisted in editing and providing feedback for the in-game dialogue and audio.

## Gallery

{% include gallery caption = "Screenshots from the game" %}

## Download

Check out the game at the [DigiPen Game Gallery](https://games.digipen.edu/games/kindred).
