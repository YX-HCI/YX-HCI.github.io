---
layout: page
title: Procedural Content Generation (PCG)
description: Fun projects! Randomly generate dungeons/buidings/spacecrafts via PCG.
img: assets/img/pcg/p3_3.png
importance: 1
category: Other
---

# Introduction
These are some Procedural Content Generation (PCG) projects, implemented with C# and simulated in Unity. Advised by professor [Greg Turk](https://faculty.cc.gatech.edu/~turk/). Github repo: [PCG-projects](https://github.com/YY-GX/PCG-projects).

Projects are as follows:
- Dungeons
- Buildings
- Vehicles


# Dungeons
Requirements:
- .Net: .Net 4.x
- Unity Editor: 2020.3.25f1
- Working on MACOS

Game Control:
- WASD | up/left/down/right for first person mode moving. (A & D for rotating, W & S for forwarding/backing)
- WASD | up/left/down/right for third person mode moving. (A & D for going left/right, W & S for forwarding/backing)
- Space for first and third person mode switch. (You'll be automatically transmitted to start point if switched from third person mode to first person mode)
- Press 'z' when nearing pillars whose top light is blue for transmitting you to the start point (where there's a pillar whose top light is green).

Script Parameters introduction:
- Seed: seed for random function.
- Grid_width: width of the whole dungeon.
- Grid_height: height of the whole dungeon.
- CA_iteration_num: number of iterations for running cellular automation.
- Init_fill_prob: initial ratio of filled grids for cellular automation.
- Grid_size: size of each grid.
- Wall_height: height of the dungeon walls.
- Chest_ratio: ratio of chests in the whole dungeon.
- Rock_ratio: ratio of piles of rocks in the whole dungeon.
- Teleportation_ratio: ratio of teleportation pillars in the whole dungeon.
- Human_height: height of camera for first person mode.
- Height_3: height of camera for third person mode.
- Is_collistion_detection: open collision detection or not.

Requirements: 
- All finished.
- Special explanation: the texture made by myself is used on the chests.

Efforts:
- When in first person mode, open the top of a treasure chest when the player comes near to it.
- When in first person mode, close the top of a treasure chest when the player leaves it.
- Create teleportation pillars for convenient teleportation.
- Designed 3 modes of piles of stones. Add much randomness to each mode, which makes piles of stones more diverse.
- Change movement method for third person mode.
- Add collision detection (only if Is_collistion_detection enabled): but currently with some bugs (you cannot press S/down when stopped by the wall, you should turn left or right first and then go forward.)



<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/pcg/pro1.gif" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Dungeon guidance.
</div>



# Buildings
Version I use:
- .Net: .Net 4.x
- Unity Editor: 2020.3.26f1
- Working on Ubuntu20

Run the code: No special demonstration, just run the code is enough. The Main.cs has been attached to the GameObject.

Script Parameters introduction:
- Seed: seed for random function.
- Num of Building: Number of buildings to be shown.
- Building Distance: Distance between shown buildings.
- Footprint Length: Used to decide the size of the building. 
- Cell Length: Used to decide the density of wall blocks, windows and doors.

Requirements: 
- All finished.

Efforts:
- Make some windows and doors opened in some random angles.
- Add windowsill.
- Add long steps for doors.
- Add porch for each door. Each porch has cylinder pillar and roof.
- Add bedroom and settingroom behind the windows and doors.
- Use random textures for different part of the building.
- Use diffent styles of windows and doors.



<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/pcg/1.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Several generated buildings from different angles.
</div>


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/pcg/2.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Several generated buildings from different angles.
</div>


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/pcg/3.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Several generated buildings from different angles.
</div>


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/pcg/4.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/pcg/5.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/pcg/6.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    More details of one building.
</div>






# Vehicles
Introduction:
I created spacecrafts (Vehicle) in this project.

Usage:
- The final.unity is the one can be run directly, I have attached the Main.cs to an EmptyObject (you only need to modify the seed to get different vehicles).

Details of my work:
1. All required parts completed
2. My efforts:
    - Used subdivision surface for nearly all surfaces.
    - Two main body parts(wing & tail) of the spacecraft are animated.
    - Two main body parts(wing & tail) of the spacecraft are swappable.
        1. Wing: Designed 3 variations for wing.
        2. Tail: Designed 4 variations for tail.
    - Add texture (steel material) to two types of wing.
    - Make camera moveable.
    - Many parts of the spacecraft shows variation in size(e.g., wings, tails, etc.). 
    - Make smooth joins between tail and body.




<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/pcg/pro3_1.gif" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Spacecrafts showcase.
</div>


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/pcg/pro3_2.gif" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Spacecrafts showcase.
</div>


<div class="row">
    <div class="col-sm mt-2 mt-md-0">
        {% include figure.html path="assets/img/pcg/p3_1.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-2 mt-md-0">
        {% include figure.html path="assets/img/pcg/p3_2.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-5 mt-md-0">
        {% include figure.html path="assets/img/pcg/p3_3.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    More spacecrafts!
</div>

