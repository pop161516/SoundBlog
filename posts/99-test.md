---
title: Test
published_at: 1-1-1
snippet: just a test... nothin to see here
disable_html_sanitization: true
allow_math: true
---

<img style="border:10px outset silver;" src="test/ferris.gif" width="800" alt="ferris"

<!--

collapes all of this, its just the intro stuff from the master copy of the site.


# This is h1 

![a drippy lemon](logo.svg)

^ images are written like this: `![description](file_path/file_name.png)`

## This is h2

*This is italic.*[^1]

[^1]: This is a footnote, *which can also be italic*.

**This is bold.**

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




Buttons with changing colours

I just copyed the hover code from DMS assignment 2 but took away the lines about sound. (I also added + 1 to the index, dont remember why. maybe becasue there is a blank png at 0.png so I might have needed to pushed up the others) and CSS from ChatGTP🧎‍♂️‍➡️

Currently works perfectly when there are no other images on the page. when I add images in the page they are included and they change when hovered.

Commented out below are some images, when un-commented the script includes them insted of just the buttons on the bottom. how can I make the script only apply to the bottom three images... do it have somthing to do with the id's? I dont remember why I had to add id's.

![Emperor Tamarin](/Images/test/emperor-tamarin.JPG)
<img src="/Images/test/golden-tamarin.png">


<style>
.container {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 0 10px; /* Optional: Add some padding if needed */
}

.button {
    display: flex;
    align-items: center;
    /* Add additional styling for buttons if needed */
}

.button img {
    display: block;
}
</style>


<body>
    <div class="container">
        <a href="/01-first-blog-post" class="button left">
            <img id= "back_id" src="/Images/white/1.png" width="30" height="30">
        </a>
        <a href="/" class="button middle">
            <img id= "home_id" src="/Images/white/2.png" width="40" height="40">
        </a>
        <a href="/03-learning-reaper-pt2" class="button right">
            <img id= "next_id" src="/Images/white/3.png" width="30" height="30">
        </a>
    </div>
</body>


<script>

    const icon_elements = Array.from (document.getElementsByTagName (`img`))
    icon_elements.forEach ((element, index) => {

        element.onpointerover = () => {
            element.src = `Images/dark/${ index + 1}.png`
        }
        element.onpointerleave = () => {
            element.src = `Images/white/${ index + 1}.png`
        }
    })


</script>


-->