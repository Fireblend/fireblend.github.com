---
layout: post
title: "Destroy All Humans: A Postmortem"
---

{{ page.title }}
================

<b>Notice</b>: This is a post originally posted in April of last year. I'm moving it here to give this blog some extra content.

So, since they're all the rage now and my "conclusion" post right after the development time ran out was pretty short, I thought I'd do a more fleshed out postmortem, so that I could reflect on the experience so far, and put on (virtual) paper what I think I've learned from this edition of LD.

In case you haven't played my game, you can find it right here: [Disregard All Humans](http://www.ludumdare.com/compo/ludum-dare-23/?action=preview&amp;uid=10166); I guess it's a requirement if you want some parts of this post to make sense :P

<strong>Background:</strong>

<img style="float:right" src="http://www.ludumdare.com/compo/wp-content/compo2/thumb/6707c3d9accc425323613aacd7a76cc7.jpg" alt="" width="270" height="183" />

So, my name is Sergio, and I'm a 23 years old Costa Rican software engineer getting his CS master degree. Even though I do enjoy them greatly, and I've developed a couple of demos throughout my career, I've never actually embarked on the adventure of creating a game, much less in 48 hours and all by myself! In January I participated in the Global Game Jam, but it was with help from a very skilled team which had let me to play to my strengths and just help out with development. The challenge a LD posed was uncharted territory!

Not satisfied with not having enough experience with 48-hour development cycles, I decided I would also learn a new programming language and game-making framework throughout the weekend: Lua and Love2D. I consider myself pretty language-agnostic, and since I didn't really have experience in game making other than with SDL (and I knew I wouldn't finish in time if I went with that), I decided to take a risk and after browsing around I settled with those two tools as my weapons of choice. I set up a new github repository with a mostly blank Lua file, and waited for the compo to start...

<strong>The theme:</strong>

"Tiny World" wasn't exactly the theme I was expecting (to be fair, I wasn't really expecting anything. I'd glanced at the final round of voting, but didn't think much of it trying not to settle on anything before the theme was decided); I spent around 2 hours thinking about the theme, throwing ideas around with my girlfriend and brother, and that's how we came up with the basic idea I would pursue, to which the finished product is actually pretty close.

I figured many people would think of the "oversized character moving around a tiny world represented as a circle" mechanic (and I was right), but I figured the specific "destroying cities, eating humans" gameplay would be unique enough to differentiate my game from others, and this being my first LD, it seemed simple enough to be finished by the time the compo ended. I was clear in that I wanted an intro an ending screen to go with the game, and an arcade-ish feel for the actual gameplay.

<img src="http://www.ludumdare.com/compo/wp-content/compo2/123793/10166-shot1.png" alt="" width="420" height="361" />

<strong>What went right:</strong>

Mostly everything. Using Lua and Love2D allowed for me to do very rapid development; Love2D being insanely intuitive and straightforward, and Lua having a syntax as easy as a syntax can be. I chose Geany as my IDE, being my usual choice for mostly everything I do, and I couldn't have made a better choice.

From there, I went at a pretty stable pace; by the end of the first day (7PM-1am) I had a main character who could walk and jump. By the end of the second day (6am-10pm) I had all of the game's mechanics implemented and working, and that allowed me to focus the rest of my time on a title screen and an ending sequence, which I think gave a nice level of polish to the final product.

Regarding graphics and music: I'm no artist. Graphics were made with Inkscape which allowed me to do clean vectorized assets that at least looked consistent, while the music and sounds were auto-generated and modified slightly using Autotracker-Bu and sfxr, respectively.

<div><img style="float:left"  wp-image-141428" src="http://www.ludumdare.com/compo/wp-content/uploads/2012/04/rect43072.png" alt="" width="127" height="480" /></div>
<strong>What went wrong:</strong>

I don't think I regret many of my decisions. I should have asked for more feedback from people so that I could realize that bullets being fired from buildings had a sort of "cheap shot" feel to them, and I should have considered shrinking buildings along with the world to make it feel more like the main character was growing, and not that the world was shrinking.

Regardless, considering life got in the way of my development time, I don't think I could have squeezed many more features before it ran out. I think the scope was just right and I planned ahead well enough to get things done by the end of the 48 hour limit.

<strong>Conclusion:</strong>

This being my first LD and arguiably my first finished game, I'm extremely proud. It's gotten a really great reception and received more attention than I could've asked for or remotely expected. This has given me a "developer high" and the crave to learn more so I can get better results on my next entries (currently learning HTML5+js); LD is a remarkable testing ground.

Speaking of which, I'd like to add that an unexpected and yet awesome part of this whole experience has been the time after the 48-hour limit. Rating games and getting your games rated by other, waaay more experienced developers from all around has been amazing, and the good reception my game's had has proved to be a huge ego boost :D

All in all, a great experience, and I'm already looking forward to the next LD!
