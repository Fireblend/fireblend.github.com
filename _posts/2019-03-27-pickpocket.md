---
layout: post
title: Aah! Pickpocket! - A Game Design Post-Mortem
---
{{page.title}}
================

This is a quick writeup on the game Aah! Pickpocket!, developed for a 17kb Javascript game challenge at <a href="https://www.growthaccelerationpartners.com/">GAP</a>.

As stated, the competition required that the game occupied a space of 17kb or less when zipped, presenting an interesting challenge in terms of space optimization and game design. This is a variation of the popular <a href="https://js13kgames.com/">js13kGames Game Jam challenge</a>, which occurs regularly and invites participants to develop a game under 13kbs in size.

For my entry, and given that I have participated in a number of game jams before, I decided I wanted to create the sort of game that I believe does well as such events, that is one that:

- Is optionally or by design playable by more than 1 player at the same time.
- Can be played in under 2 minutes.
- Fosters interaction between the participants.
- Can be explained and understood quickly.

In addition to those requirements, I decided I wanted to pay tribute to a design element that is rarely seen in videogame design: asymmetric gameplay. This refers to games (either collaborative or competitive in nature) in which all players have different win conditions and different mechanisms with which to achieve them. This is not that rare in boardgames, interestingly enough, with examples such as Cosmic Encounter(2008), Android: Netrunner (2012), Scythe(2016) and Root (2018).

Asymmetric gameplay design in competitive games poses a big challenge because of the balancing effort required to make it so opposing players have an approximately equal chance of winning. Seeing how each player (in a hypothetical 2 player game) have different resources, actions and win conditions, there's an expectation of these being balanced in a way that makes both roles fun.

In addition, a pitfall that is common in these sort of games is that of not adding enough interaction between the roles to occur. An asymmetric game may be perfectly balanced with various different roles, but if there are no mechanics that intertwine those different resources and actions between the players, then the game will seem like 2 separate solo games rather than a single, competitive one.

For Aah! Pickpocket! I decided to simplify the main mechanics of Spy Party (2018), a 2-player competitive game in which a player plays as a sniper tasked with shooting a spy in a social setting, while the second player, playing the role of the spy, is tasked with completing a checklist of actions in that social setting without being detected.

The social setting is populated with NPCs (non-playable characters) that the spy player will have to mimic in order to either fool the sniper into shooting an NPC instead, or buy enough time to complete their tasks. It is important to note that Spy Party is an online game, which allows for different information to be shown in the screen for the players, which Aah! Pickpocket! is a single-screen game.

In Aah! Pickpocket!, the role distribution mimics that of Spy Party, with a player playing as "the sheriff" and another playing as the "thief". The sheriff is tasked with identifying the thief (by using the mouse and clicking on their suspect), while the thief has to pickpocket 3 of the NPCs moving across the screen (this player uses the keyboard exclusively). Next, I mention some of the balancing decisions taken into account for both roles:

<b>Thief</b>:

- Their win condition is to pickpocket 3 strangers. A pickpocket event will mark the location of the event on the screen, while giving the thief time to escape from the sheriff's attention.

- Each pickpocket event can only be triggering after talking to an NPC for 3 seconds. Conversation happens automatically when in proximity to the NPC. In order to provide the thief with a visual aid, the speech bubble that signals conversation has an animation cycle that lasts 1 second exactly.

<b>Sheriff</b>:

- Their win condition is to identify the thief. They only have one chance to do it, however they can choose to wait until 2 pickpocket events have occurred to aid in their detection.

<b>Both</b>:

- The number of NPCs on screen has been set to 20 (21 with the assassin). This amount could be tweaked to help the sheriff (decrease it) or the thief (increase it).
- Both NPCs as well as the thief can wrap around the screen, which is helpful to the thief. This could be disabled in order to help the sheriff instead.

In general, I believe the game is reasonably balanced. I didn't get much time to play-test it, but it can be easily tweaked as explained above.

In conclusion, this was an interesting exercise in game prototyping and design. Much can be accomplished with low requirements when the design of the game takes center stage rather than its visual attributes or systems complexity.

<a href="http://www.fireblend.com/js17/game.html">You can play the game here</a>.
