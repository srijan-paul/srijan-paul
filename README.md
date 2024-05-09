## injuly

<video autoplay loop muted>
    <source src="https://user-uploads.perchance.org/file/da1bf91d3531f0c92e59e6db38e44176.webm">
</video>


I like systems programming and functional languages.
Professionally, I've worked on **web servers (and pages)**, **compilers**, **static analyzers**, and other miscellany.

Interests:
- Game development
- Pixel art
- Shin Honkaku
- Functional programming



## Microblog

A list of thoughts that aren't not elaborate enough to warrant a blog post, but interesting enough to be written down.

<details style="margin-left: 15px">
    <summary>Click to read</summary>

<details>
<summary>
    <h3>1. CRT displays and retro shaders</h3>
</summary>

I find it very interesting that video games today often try to emulate artifacts of the past that 
older developers would kill to get rid of.
The CRT screen shader is one of them. 
I wrote one for one of my (~~now abandoned~~) side projects, and was happy with how it turned out.
Here is an old GIF of the effect:

<img src="./bullet_hell.gif" width="50%" height="50%" />

The above shader displays two of my favorite effects that nail the "retro" feel when done well:
1. The [CRT](https://en.wikipedia.org/wiki/Cathode-ray_tube) screen bend.
2. [Chromatic Abberation](https://en.wikipedia.org/wiki/Chromatic_aberration).

It also has a scanline effect, but that's off topic.

CRT screens would shoot a cathode ray that would traverse the screen row-by-row.
If the screens weren't curved in shape, different points on the surface would be at different distances from the origin of the cathode ray, resulting in a distorted image.
The screens had to be curved at very precise angles to perfectly offset the distortion.

Since It's getting pretty late in the night at the time of me writing this, 
I'll leave this great explanation on chromatic aberration by an underrated youtuber, Pixel Prophecy:
- [What is Chromatic Abberation? (And why?)](https://www.youtube.com/watch?v=oE8Zjr5NJrM)

If you're wondering how it's implemented in the gif I showed above, I just offset the Red, Green, and Blue channels for every on-screen pixel. As for the scanlines, they're just periodically occuring horizontal lines timed with a sine wave.
</details>

</details>
