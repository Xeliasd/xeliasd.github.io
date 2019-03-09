---
layout: project
title: "Chess"
date: 2018-12-01
categories: Project
typefilt: chess
---

## 3D Animated chess

I created a 3D chess as a school project for Principles of computer graphics.
It was based on OpenGL, written in C++. It works according to internationally recognised rules of chess.

### Controls
The selector moves around the playing field using keyboard arrows. Spacebar is used to either select a figure, or select a place where you want your piece to move.
If you try to make an illegal move, or press spacebar in the same spot as the piece already is, you have to make a different move. 

### Graphic goals reached
<ul>
<li>Unique 3D meshes</li>
<li>Unique texturing using uv coordinates</li>
</ul>

This was accomplished by using custom meshes for chess pieces.

<ul>
<li>Animated or interactive camera with perspective projection.</li>
</ul>	
Camera coordinates change after each move, so that players view playing field from their respective sides. Also, when a piece gets removed from the game,
the camera does shaking "earthquake-like" effect.

<ul>
<li>Use of hierarchical transformations in the game scene.</li>
</ul>
Selector has 2 parts. A circle undearneath the pieces and an arrow floating above them. The bottom circle moves using hierarchical transformation of the arrow.

<ul>
<li>Use of multiple camera view presets</li>
</ul>
There are 3 basic camera angle presets as shown in the pictures to the left.

<ul>
<li>Implementation of basic game logic, game has multiple scenes, is playable and has an ending.</li>
</ul>
Achieved by the fact that the whole game works according to usual rules of chess.

<ul>
<li>Effective object to object collisions and interactions.</li>
</ul>
As pieces move smoothly towards their location, piece removal is triggered when pieces collide.

<ul>
<li>Dynamic scene with game objects being created and destroyed during gameplay.</li>
</ul>
When a piece gets removed from the game, it flies away, creating a stream of small "explosions" behind it.

<ul>
<li>Basic simulated animation eg. gravity.</li>
</ul>
Gravity is used during the start of the game, when pieces fall down to the playing field from above, also when they they get removed, after 
they initially fly away, gravity pulls them back down.

<ul>
<li>Procedurally driven animations.</li>
</ul>
Multiple different animations, from smooth piece moving to selector arrow rotation.

<ul>
<li>Diffuse scene lighting with materials</li>
</ul>
Achieved by using simplet lighting from 2 sources.


