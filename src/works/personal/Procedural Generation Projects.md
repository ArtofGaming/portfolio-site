---
title: 'Adventures in Procedural Generation'
pubDate: 2025-04-04
description: 'Solo developer'
image:
    url: 'https://docs.astro.build/assets/rose.webp'
    alt: 'The Astro logo on a dark background with a pink glow.'
tags: ["Unity","Godot","GDScript","C#"]
theme:
    back-color: "white"
---

<style is:global>
    div{
        background-color: var(back-color);

    }
    h4{
        color: rgb(228, 157, 126);
        margin-bottom: -.5ch;
        text-align: center;
    }
</style>
<p style="border-color: rgb(228, 157, 126); border-width: 7px; border-style: dashed;  text-align: center">
    <video width="426" height="240" controls>
        <source src="/cellular automata demonstration.mp4" type="video/mov">
    </video>
    <p>
    </p>
    See code <a style="color: white"href='https://github.com/ArtofGaming/mystery-platformer'>here</a> and <a style="color: white"href='https://github.com/ArtofGaming/LD57-Depths'>here</a>

</p>

### Project Summary
I created two types of dungeon generation systems for a hypothetical game using two different methods. First with cellular automata in Godot, then with BSP in Unity.

### My Contribution Highlights
    - implementation of cellular automata
    - implementation of binary spatial partitioning

### Cellular Automata
For the generated environment, I want it to be cave-like so I chose cellular automata as my method for generation. The type of neighborhood I used for my cellular automata was a Moore neighborhood (where each cell in the grid surrounding the target cell is in the neighborhood so it is influenced by the cell on its N, E, S, and W edges and NE,NW,SE,SW corners as well as itself) as I thought that would give a more natural look.

The cells could have three states: INVALID, WALL, FLOOR. The enum had a 4th state: MAX which no cell was ever set to. 
After the cellular automata had run, I eliminated spare wall and floor tiles that were in the way of a potential path to make the cavern more navigable.

### Binary Spatial Partioning
The purpose of this procedural generation experiment was to create a convincing dungeon of manmade origin. I created a large filled in room that got split into sections recursively either horizontally or vertically. Then when rooms cannot be split anymore without going below the minimum size limit, the rooms get filled with floor tiles with some randomness for variation. Then the rooms were connected.

### What I Learned
I was able to learn more about procedural generation which had been a subject I'd been interested in since being introduced to it in college. I also learned how to better make use of hashsets (for room connections in the BSP dungeon) as well as got better at doing new things within a time limit as the BSP project was done for Ludum Dare.
