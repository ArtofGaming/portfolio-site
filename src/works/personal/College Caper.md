---
title: 'College Caper'
pubDate: 2024-04-28
description: 'Solo developer'
image:
    url: 'https://docs.astro.build/assets/rose.webp'
    alt: 'The Astro logo on a dark background with a pink glow.'
tags: ["Databases", "C#", "Unity", "SQL"]
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
        <source src="/College Caper Vid.mp4" type="video/mp4">
    </video>
    <p>
    </p>
    See code <a style="color: white"href='https://github.com/ArtofGaming/College-Caper'>here</a>

</p>

### Project Summary

This fashion game is a solo project that utilizes MVC architecture to create a simple dress up game experience. The view layer is inside of Unity, and all the clothes are kept inside a catalogue database as well as a list of their attributes. Each item has different emotion values based off of their attributes and styles.

<img width="506" alt="Screenshot 2024-04-27 123610" src="/database1.png">

<img width="250" alt="Screenshot 2024-04-27 123727" src="/database-table2.png">

The meshes were made in Blender and are linked with the databse by names so that whenever a certain item is selected the model that shares its name has its mesh renderer enabled on the model. 

The tabs on the side filter items by clothing category and only those are sortable in the application for now, but on the SQL side this is already possible. Meshes can be cleared with the clear button next to the model or the page can be refreshed. The filter feature works thanks to two main functions, one that reads the appropriate item names from the server and connects them to their models and generates a box for them to sit in front of and the other which looks at all the items that don't correspond with the appropriate filter and removes them and the box they're a child of.

### My Contribution Highlights
    - Handling clothing changes without any noticable slowdown
    - Loading remote images for display in real time
    - Quick filtering of items without noticable slowdown

### What I Learned

