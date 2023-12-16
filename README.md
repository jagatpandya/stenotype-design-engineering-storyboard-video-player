# Stenotype Storyboard Video Player

Designed a video player as part of a Design Engineering proposal to introduce Stenotype - a user-friendly note-taking platform inspired by the open-source Django project, Firepad. The aim is to make Stenotype even better, offering new features and an appealing UI. Stenotype, a device-based note-taking platform, is envisioned to be built on the Firepad, with the vision to replace traditional school notebooks with a modern, cutting-edge solution.

Click the badge below to explore Firepad in action. Near to that, there is a badge linking to the open-source GitHub repository of Firepad - check it out!

[![Firepad](badges/firepad.svg?raw=true&sanitize=true)](https://firepad.io/) [![Github](badges/github.svg?raw=true&sanitize=true)](https://github.com/FirebaseExtended/firepad)

![Screenshot](stenotype-storyboard-1.gif?raw=true)

To watch it on a mobile device, change the screen orientation to landscape! 

![Screenshot](stenotype-storyboard-2.gif?raw=true)

![Badge](badges/badge-1.svg?raw=true&sanitize=true)&emsp;![Badge](badges/badge-2.svg?raw=true&sanitize=true)&emsp;![Badge](badges/badge-3.svg?raw=true&sanitize=true)

> **Note:** To view the code in the GitHub repository with proper formatting, make sure to change the tab size from the default **8** to **4**. You can adjust this setting in `GitHub > Settings > Appearance > Tab Size Preference`.

The HTML hierarchy below represents a video player structure, encapsulated within a main element with the class wrapper, consisting of a div with the class player and various nested elements, including controls, buttons and a video element with associated classes and attributes for styling and functionality.
```
main.wrapper
└── div.player
    └── div.player-hover[data-fullscreen="false"]
        ├── a.github-corner
        │   └── svg
        ├── div.container
        │   ├── div.watermark-container
        │   │   └── img
        │   └── div.player-container
        │       ├── div.video-progress
        │       │   └── div.video-progress-bar
        │       ├── div.player-controls
        │       │   ├── div.player-buttons
        │       │   │   ├── button.button.play
        │       │   │   ├── button.button.pause[hidden]
        │       │   │   ├── button.button.backward
        │       │   │   ├── button.button.forward
        │       │   │   ├── button.button.volume
        │       │   │   ├── button.button.mute[hidden]
        │       │   │   ├── div.volume-progress
        │       │   │   │   └── div.volume-progress-bar
        │       │   │   └── div.time-container
        │       │   │       ├── p.current-time
        │       │   │       ├── p.time-separator
        │       │   │       └── p.duration
        │       │   └── div.full-screen-container
        │       │       ├── button.button.full-screen
        │       │       └── button.button.exit-full-screen[hidden]
        │       └── video.video[poster="src/images/thumbnail.png"]
        │           └── source[src="src/videos/stenotype-storyboard.mp4" type="video/mp4"]
        └── script[src="src/scripts/script.js"]
```
Take a look at the layout design of this video player. It's created using a mix of a grid and flex boxes, as shown in the screenshot below:

![Screenshot](layout/layout.png?raw=true)

## License
Please refer to the [LICENSE](LICENSE) file for information on the license terms and any associated rights and limitations (MIT).
