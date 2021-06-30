# Stuff

**NOTE:** I'll just use this spare space to write about things that I think about but dont come up in conversations often.
Sometimes my thoughts aren't elaborate enough to warrant a blog post in on itself.

### #1 On CRT screens and shaders.
<details>
<summary>Click to read</summary>

I find it very interesting that video games today often try to emulate artifacts of the past that 
then developers would kill to get rid of.
The CRT screen shader is one of them. 
I wrote one for one of my (~~now abandoned~~) side projects, and I remember being happy about the way it turned out.
Here is an old gif of the said game:

<img src="./bullet_hell.gif" width="50%" height="50%" />

The above shader displays two of my favorite effects that can be impressive when done correctly:
1. The [CRT](https://en.wikipedia.org/wiki/Cathode-ray_tube) screen bend.
2. [Chromatic Abberation.](https://en.wikipedia.org/wiki/Chromatic_aberration)

It also has some scanlines going on, but they're not tuned as well as I'd like, and are a trivial
effect to implement.

### Why did older displays have curved screens you ask?

To my knowledge, CRT screens worked by shooting a cathode ray that would traverse the phospor screen horizontally and
vertically at the same time.
There is an interesting tidbit about this movement that is largely misunderstood, mentioned 
[here](https://en.wikipedia.org/wiki/Raster_scan#Scanning_pattern) on wikipedia. I highly recommend this article.

If CRT screens weren't curved in shape, different points on the screen would be at different distances from
the origin of the cathode ray, and hence the image would be distorted heavily. The screens had to be curved at very precise
angles to perfectly offset the distortion. 

This challenge in production and engineering from the gone era is now an artifact video games introduce overhead to emulate!
Retro and otherwise. Pretty neat, right?

Since It's getting pretty late in the night at the time of me writing this, 
I'll leave this great explanation on chromatic aberration by an underrated youtuber, Pixel Prophecy:
- [What is Chromatic Abberation? (And why?)](https://www.youtube.com/watch?v=oE8Zjr5NJrM)

If you're wondering how it's implemented in the gif I showed above, I just offset the Red Green and Blue channels for
each pixel somewhat.

As for scanlines, they're just periodically occuring horizontal lines timed with a sine wave.

I used LSL and Lua (LOVE) to build the game in that screenshot, but the same can be done in any shading language and any game
engine.
 
</details>

Handy counter to gauge the number of eyes on this page:

![](https://komarev.com/ghpvc/?username=your-github-username)
