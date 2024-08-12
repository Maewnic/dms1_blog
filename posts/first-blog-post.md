---
title: This is Munich's blog post!
published_at: 2022-11-04
snippet: An example of a blog post.
disable_html_sanitization: true
allow_math: true
---

# This is h1

![a drippy lemon](logo.svg)

**Scavenger Hunt**

![a group of students in front of the black box or a possible one?](scavenger_hunt_1.jpg)

![The disembodied hands of a great ape.](scavenger_hunt_2.jpg)

![Definitely the study place for Sith Lord](scavenger_hunt_3.jpg)

![The wide machine, dispensing beverages from a far away land... Thinking of it. It could be the flying turtle because it's from my home country, Thailand but nevermind.](scavenger_hunt_4.jpg)

![The golden globe atop a tower](scavenger_hunt_5.jpg)

![Some sort of net made by papers](scavenger_hunt_6.jpg)

**Selfie Design**

![Playing with Ps to edit my selfie](Selfie_design.png)

^ images are written like this: `![description](file_path/file_name.png)`

## This is h2

*This is italic.*[^1]

[^1]: This is a footnote, *which can also be italic*.

**This is bold.**

[Experiment on Pr transitions, keyframes and editing tools using three 30 seconds clip. Two clips from friends. Merged in to a single clips](https://youtu.be/jsR2qI64CJ0)

<iframe width="560" height="315" src="https://www.youtube.com/embed/jsR2qI64CJ0?si=yPa1CPU7nY27eI1m" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

Hyperlinks can be written like this: `[text](https://URL)`

You can find a markdown cheat-sheet [here](https://www.markdownguide.org/cheat-sheet/).

### This is h3

**Class activity storyboard**

![BladeRunner2049 Storyboard 1](Storyboard_P1.jpg)

![BladeRunner2049 Storyboard 2](Storyboard_P2.jpg)

![BladeRunner2049 Storyboard 3](Storyboard_P3.jpg)

**Task 1 Storyboard**

![Task1 Storyboard p1](T1_Storyboard_p1.jpg)
*Ambient sounds are present the whole video, giving a sense of realism.*
*A quite beeping sound from the pedestrian crossing. Beeping in a slow tempo.*
*Slow music playing.*

![Task1 Storyboard p2](T1_Storyboard_p2.jpg)
*Similar to the page 1.*

![Task1 Storyboard p3](T1_Storyboard_p3.jpg)
*This is the important part. The slow beep that has been present throughout the montarge switched to a faster beep. This time the video will give a sense of rush and busyness.*
*The music is also in a faster paste.*

![Task1 Storyboard p4](T1_Storyboard_p4.jpg)
*Continues from the previous page.*
*A little over midway through this page. The beep return back to normal tempo as the start.*

![Task1 Storyboard p5](T1_Storyboard_p5.jpg)
*The beep and the music stops once there's a ding sound from the lift. Stopping all the tension.*
*After the lift door opens, the music returns. This creates a really strong scene and a dramatic effect.*

#### This is h4
**Class activity 30 seconds sound design task has not been done due to sickness absence**

[Selfportrait video draft](https://youtu.be/0e1ywB-kRzA)

<iframe width="560" height="315" src="https://www.youtube.com/embed/0e1ywB-kRzA?si=HqiXUcyS9LuKVb4K" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

##### This is h5
![Class Activity Black Squares](blacksquares.png)

## Maths:

... which can be written inline, like this: $\{ x, y, z \} \in \N$

... or block, like this:

$$ x^2 + y^2 = z^2 $$

Visit [ $\KaTeX$ ](https://katex.org/docs/supported#fractions-and-binomials) for more information about writing maths.

## Embedding video:

<iframe id="coding_train_video" src="https://www.youtube.com/embed/rI_y2GAlQFM?si=RDgjkpunxk1mQzMI" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

<script type="module">

    console.log (`hello world! 🚀`)

    const iframe  = document.getElementById (`coding_train_video`)
    iframe.width  = iframe.parentNode.scrollWidth
    iframe.height = iframe.width * 9 / 16

</script>

## Embedding p5 sketches:

<iframe id="falling_falling" src="https://editor.p5js.org/capogreco/full/Fkg05m7aA"></iframe>

<script type="module">

    const iframe  = document.getElementById (`falling_falling`)
    iframe.width  = iframe.parentNode.scrollWidth
    iframe.height = iframe.width * 9 / 16 + 42

</script>

## Canvas API

<canvas id="canvas_example"></canvas>

<script type="module">
    const cnv = document.getElementById (`canvas_example`)
    cnv.width = cnv.parentNode.scrollWidth
    cnv.height = cnv.width * 9 / 16

    const ctx = cnv.getContext (`2d`)
    const pos = {
        x: -100,
        y: cnv.height / 2 - 50
    }
    
    function draw_frame () {
        ctx.fillStyle = `turquoise`
        ctx.fillRect (0, 0, cnv.width, cnv.height)

        ctx.fillStyle = `hotpink`
        ctx.fillRect (pos.x, pos.y, 100, 100)

        pos.x += 2

        if (pos.x > cnv.width) {
            pos.x = -100
        }

        requestAnimationFrame (draw_frame)
    }

    draw_frame ()
</script>


