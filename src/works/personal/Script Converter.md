---
title: 'Script Converter'
pubDate: 2026-05-22
description: "A C++ tool I'm currently creating to convert game scenario scripts into .nani scripts for use with Naninovel"
image:
    url: 'https://docs.astro.build/assets/rose.webp'
    alt: 'The Astro logo on a dark background with a pink glow.'
tags: ["C++","Tool Dev"]
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
</p>

### Project Summary
In order to make a usable nani script file, each line aside from comments must be prefixed with a command such as @char or marked as dialogue. In order to avoid having to reformat scripts by hand, I wanted to create a tool to create a new nani file including commands without wasting time reformatting.

### Current Progress
I have the file being read and it recognizing each line. Next will be separating each part of a line for the sake of knowing where to place commands.

### What I Learned
I learned more about converting to custom file types. 
