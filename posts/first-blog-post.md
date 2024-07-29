---
title: This is a blog post!
published_at: 2022-11-04
snippet: An example of a blog post.
disable_html_sanitization: true
allow_math: true
---

# This is h1

![a drippy lemon](logo.svg)

![a group of students in front of the black box or a possible one?](scavenger_hunt_1.jpg)

![The disembodied hands of a great ape.](scavenger_hunt_2.jpg)

![Definitely the study place for Sith Lord](scavenger_hunt_3.jpg)

![The wide machine, dispensing beverages from a far away land... Thinking of it. It could be the flying turtle because it's from my home country, Thailand but nevermind.](scavenger_hunt_4.jpg)

![The golden globe atop a tower](scavenger_hunt_5.jpg)

![Some sort of net made by papers](scavenger_hunt_6.jpg)

^ images are written like this: `![description](file_path/file_name.png)`

## This is h2

*This is italic.*[^1]

[^1]: This is a footnote, *which can also be italic*.

**This is bold.**

[Experiment on Pr transitions, keyframes and editing tools using three 30 seconds clip. Two clips from friends. Merged in to a single clip](https://youtu.be/jsR2qI64CJ0)

<iframe width="560" height="315" src="https://www.youtube.com/embed/jsR2qI64CJ0?si=yPa1CPU7nY27eI1m" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

Hyperlinks can be written like this: `[text](https://URL)`

You can find a markdown cheat-sheet [here](https://www.markdownguide.org/cheat-sheet/).

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


