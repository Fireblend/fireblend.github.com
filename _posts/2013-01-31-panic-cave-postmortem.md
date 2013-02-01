---
layout: post
title: "Twisted Shotgun Panic Cave: A Postmortem"
---

{{ page.title }}
================

To say that this last Global Game Jam surpassed last year's would be a gross understatement. Although this post is supposed to be mostly about the game I helped make, I think not commenting on the success of the jam would mean detracting from the whole thing by not providing some context on the environment it was created in. The space and work areas were great, the organization was pretty much flawless, attendance nearly quadrupled from last year, we had sponsors and a host that actively interacted with the jammers, and (I can't stress this enough) <b>the quality of the resulting games reflected these conditions</b>. I really doubt games as good as the ones that were made during this jam would have been created had it not been for the great working environment we had going.

<strong>Background:</strong>

The game was made for the Costa Rican 2013 Global Game Jam, a 48-hour game development "marathon" in which teams (usually created randomly from the pool of attending jammers, as in this case) create a game from scratch, including its code, music, sound effects, graphics, and any other asset that might have to be created for the game to work. Having participated in the previous one, and in a couple of Ludum Dares (which are solo), I can vouch for the effectiveness of jamming for learning game development principles, time and scope management, improvisation and countless other very valuable skills, as well as for having a good time and making new friends. It's a win-win situation.

For this occassion, I teamed up with 3 other very skilled individuals: Eduardo (a programmer), Markus (a composer) and Gustavo (a graphic designer). I couldn't have asked for a better distribution; just knowing that we had access to both graphics and music was very encouraging, and promising in regards to the odds of having a polished game by the end of the jam.

Alright, now we can discuss Twisted Shotgun Panic Cave.

<center><img src="http://globalgamejam.org/sites/default/files/styles/large/public/screenshots/2013/Funciones.png" alt="" width="510" height="250" /></center>

<strong>Concept:</strong>

Twisted Shotgun Panic Cave is a game in the vein of other arcade "single-screen" platformers such as Super Crate Box. Using that same type of gameplay, we added various twists which we considered relevant to the jam's theme (the sound of a beating heart): being a sound, and having someone willing to dabble in music, we inmediately though of incorporating it into the gameplay through 2 means: The music would change according to the state of the game, and most of the screen would be obscured, leaving the player dependant on sound cues to build a mental model of the state of the game by themselves.

The beating heart also alludes to tension and increased heart rates, a theme picked up by pretty much every other jammer in the competition, and thus we settled on a "dark", almost sarcastic graphic style, with a little girl having to gun her way through the screen to reach light orbs and thus increase the time available to the player to amass a high score.

<strong>Development:</strong>

Although I intended to use Actionscript for my jam entry, Eduardo was quick to suggest Game Maker, and since I had never used it before (plus the fact that it would be easier to teach than Actionscript), we decided to go with that. I have my reservations about using proprietary technology in jam projects, since the source code to these projects is usually posted online, and it's somewhat contradictory that not everyone will be able to compile it, but at the same time many solutions such as Unity and Game Maker are pretty much unmatched in terms of ease of use and have no viable open source alternatives, so I really have no comeback for this scenario :P

<img style="float:left; border:12px solid white" src="http://globalgamejam.org/sites/default/files/styles/large/public/P1271207.JPG" width="400" class="alignleft" />

Game Maker allowed us to make some considerable progress in the first few hours of the jam. By midnight the core of the game was done: a Super Crate Box clone with limited vision (provided by some great light-related code Eduardo kept handy).

This allowed us to move into some of the most (in my opinion) inventive aspects of the game, first among them the enemies. We settled on having four types of enemies. Markus argued that they ought to each have their own sound, so that skilled players could recall which sound corresponded with which enemy and thus could gain more information from the audio cues than a novice player. Enemy behavior was also put into consideration, and we ended up with what I think is a pretty good enemy roster: A classic "sentry" that stays in the platform in which it spawns, a "ghost" that can move through platforms but whose movement is entirely random, a "seeker" that went straight for the player but for whose platforms were an obstacle and a "jumper", which, along with some level design decisions, would move from one side of the screen to the other, jumping between platforms.

Another interesting part of the development process was the sound-related mechanics. In the first place we thought about only distinguishing between enemies spawning left and right of the character, with two separate sound files for each enemy. This would give the player 2 bits of information on every spawning enemy: What it was, and (vaguely) where it had spawned. Fortunately, however, we hit upon a Game Maker function that allowed us to play sound bites within a 3D space relative to a listener point that we could determine, allowing us to also provide the distance from the player's avatar to each spawning enemy within the audio cues.

Finally, towards the last stages of development, another key aspect we focused on was level design. We wanted a stage that both allowed for a variety of strategies in regards to player movement, and forced the player to constantly move from one platform to the other (for example, we avoided making it possible for the player to jump from the top of the screen to the bottom). I think the design we arrived at was pretty successful at both things.

Overall, development was pretty smooth. Game Maker is a surprisingly versatile tool at which Eduardo is very skilled, and I thought we were a pretty good team, suggesting alternate solutions and strategies when appropriate and managing task division seamlessly. I thought I'd end up doing menial tasks seeing how he had progressed at the beginning of the jam, but by the end I thought the tasks had balanced out and was pretty satisfied with my contributions.

<strong>Audio & Graphics:</strong>

As I said, we hoped that by having both a graphic designer and a musician in our team would allow us to achieve a high level of polish for our game. Needless to say, we undoubtedly did, with the resulting game having both superb audio and a unique and enjoyable visual identity. 

<img style="float:right; border:12px solid white" src="http://globalgamejam.org/sites/default/files/styles/large/public/screenshots/2013/screen_3_0.png" width="300" class="alignleft" />

Sound was pretty integral to the gameplay, as we relied on it to communicate both a sense of constant urgency as well as a good portion of the game state to the player. Markus more than came through with this task, composing over 5 songs and providing an impressive amount of audio effects that were both incredibly good (the music is catchy and there were more than a couple of requests for an extended version of the game's "theme") and surprisingly coherent with the rest of the game.

Visually, Gustavo made an impressive job out of creating a visual identity for the game. We were impressed more than once by his attention to detail: when we expected a simple 3-tile platform, he provided custom tiles for unique, detailed platforms. When we expected enemies that would be color variations from one another, he provided brilliant interpretations of the behaviors we had added for each enemy, leading to a visual identity that really gave life to the game. Even the quirky game intro that is shown at the start of the game matches the style brilliantly.

<strong>Conclusions:</strong>

Even though the game and the jam itself were a success, there are always observations to be made in regards to improvements for the next jam. I think the game could have been more inventinve in regards with how the theme was interpreted, maybe by aiming for more ambitious mechanics. As it stands, the scope was pretty relaxed and allowed us some good sleep hours, but I don't think the extra twists were enough to completely separate ourselves from the obvious Super Crate Box comparisons.

<img style="float:left; border:12px solid white" src="http://transformative-step.gesi.org/static/css/images/android.png" width="90" class="alignleft" />

It had a pretty good reception though, mostly due to the music and the way it was incorporated into the gameplay, which I think taught us all a pretty good lesson about the importance of sound in making a game effective and supporting its gameplay.

Finally I have to say that, as all jams, this was an enlightening learning experience, and I hope to continue participating in these for a pretty good time. I hope my teammates had as good a time as I did during the jam, and I should probably learn to write shorter post-mortems :P

Twisted Shotgun Panic Cave is available for [Android](https://play.google.com/store/apps/details?id=com.gamejam.paniccave) and [Windows](http://globalgamejam.org/2013/twisted-shotgun-panic-cave)
