---
title: "Example Template"
excerpt: "For templating purposes"
permalink: /games/example/

header: 
  teaser: /assets/images/games/mayor_outbreak/teaser.png
  overlay_image: /assets/images/games/mayor_outbreak/teaser.png
  overlay_filter: 0.6 # the lower the more visible the image is
  # caption: "This is a caption: [**This is a Link**](https://unsplash.com)"
  actions:
    - label: "Example link"
      url: ""
    - label: "Example link 2"
      url: ""

# vscode auto format changes the - to + breaking the page, watch out for that
sidebar: 

  - title:  "Role(s)"
    # image: http://placehold.it/350x250 no image needed here
    # image_alt: "placehold alt text"
    text:   ""

  - title:  "Responsibilities"
    text:   ""

  - title:  "Project Status"
    text:   ""

  - title:  "Awards"
    text:   ""
    

gallery:

  - url:        /assets/images/games/mayor_outbreak/screenshot1.png
    image_path: assets/images/games/mayor_outbreak/screenshot1.png
    alt:        "Screenshot of game"

  - url:        /assets/images/games/mayor_outbreak/screenshot2.png
    image_path: assets/images/games/mayor_outbreak/screenshot2.png
    alt:        "Screenshot of game"

toc: true

categories:
  #- Games

tags:
  #- Haxe
  #- HaxeFlixel
  #- Arcade
  #- Retro
  #- Simulation
  #- Outbreak
  #- AloneTogether
  #- HaxeFlixelJam

---

Retro looking outbreak simulation prototype I made using [Haxe](https://haxe.org/) and [HaxeFlixel](https://haxeflixel.com/) for the [Newgrounds HaxeFlixel Game Jam](https://www.newgrounds.com/bbs/topic/1450269).

I started by following [this tutorial](https://haxeflixel.com/documentation/tutorial/) on the Flixel website, then branched off and added some stuff of my own.
My aim was to make a virus outbreak simulation where you could decided between surviving yourself or help other people survive too by giving them protection equipment like masks, gloves and hand sanitizer.
Unfortunately the Jam happened at the same time as my University exams, so I didn't have enough time to implement a proper tutorial or win/lose condition. At this stage winning equals reaching 0 infected and losing equals dying.

Development has stalled for now, the code got messy and I lost interest in the project after the Jam.

## Gallery

{% include gallery caption="Some screenshots from the game" %}

## Get the Source

The project is Open Source, the repository [can be found here](https://github.com/Gioele-Bencivenga/AloneTogether).

## Technologies Used

Here are the main technologies I used to make this game:

| Technology | Usage |
| ----------- | ----------- |
| [Haxe](https://haxe.org/) + [HaxeFlixel](https://haxeflixel.com/) | Language and Framework in which I programmed the game |
| [Visual Studio Code](https://code.visualstudio.com/) | IDE used for writing the code |
| [Ogmo Editor](https://ogmo-editor-3.github.io/) | Level editor used to design the city tilemap |
| [Piskel](https://www.piskelapp.com/) | PixelArt drawing tool used for minor edits on the image assets |
| [Audacity](https://www.audacityteam.org/) | Audio software used for minor edits on the audio assets |
