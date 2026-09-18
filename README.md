# Dino Meteor 3D

[Play the game](https://jackrichardlawson.github.io/dino-meteor-3d/)

A browser game with 18 creatures, meteor upgrades, boss battles, and skeleton quests. Built iteratively in ChatGPT and packaged for GitHub Pages with the original game JavaScript unchanged.

## How to play

Choose a dinosaur, then press **PLAY**. Use the up/down arrow keys or onscreen arrow buttons to change lanes. Press **Space** or **METEOR** to fire. Use **Pause** to pause or resume.

Defeat the 200-fossil boss with a creature to unlock that creature's skeleton form. Progress lasts for the current page session.

## Run locally

Serve this directory with any static web server, for example:

```sh
python -m http.server 8000
```

Then open http://localhost:8000. No build step is required. The game requires WebGL and an internet connection to load Three.js 0.180.0 from jsDelivr.

## Packaging

`index.html` contains the game, its original styles, and the styles needed outside ChatGPT. ChatGPT frame messaging and already-running preview state were removed so the game starts correctly as a standalone page. Gameplay and dinosaur models are unchanged.
