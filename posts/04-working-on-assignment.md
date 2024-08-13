---
title: Working on Assignment 1
published_at: 2024-8-13
snippet: -W4- Planning ideas and recording
disable_html_sanitization: true
allow_math: true
---

<h2 style="color:CornflowerBlue;">Class</h2>

**Super** short lecture.

Then I had some class time to work on my assignment.

<h2 style="color:CornflowerBlue;">Assignment</h2>

Still no progress on the assignment but I will get it done. I'm sure.

<h2 style="color:CornflowerBlue;">Homework</h2>

- Pre-reading
    - First I read "David Byrne - Technology Shapes Music [How Music Works]"
        - Really fascinating, the psoychlogy and philosophy of truth are always interesting 😋 also interesting to think about the way technologies have shaped the way we play music(and act). 
    - Then I read "The Man And The Woman And The Edison Phonograph - Bruce Watson AJE: Australasian Journal of Ecocriticism and Cultural Ecology, Vol. 1, 2011/2012"
        - Also interesting, I think Byrne said somthing in the previous text about the paths of history. with one small change we could be living in a completely differant world. Its great to see tht this mistake was corrected

- Think about Assignment 
???

---
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
        <a href="/03-learning-reaper-pt2" class="button left">
            <img src="/Images/white/2.png" width="30" height="30" alt="Page 1">
        </a>
        <a href="/" class="button middle">
            <img src="/Images/white/3.png" width="40" height="40" alt="Page 2">
        </a>
        <a
            <img src="/Images/white/1.png" width="30" height="30" alt="Page 3">
        </a>
    </div>
</body>


<script>

    const icon_elements = Array.from (document.getElementsByTagName (`img`))
    icon_elements.forEach ((element, index) => {

        element.onpointerover = () => {
            element.src = `Images/dark/${ index }.png`
        }
        element.onpointerleave = () => {
            element.src = `Images/white/${ index }.png`
        }
    })


</script>