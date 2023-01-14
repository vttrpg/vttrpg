# vtt rpg

What is the goal of this repository and why might it matter? 
Currently a lot of people playing table top rpgs online use many different platforms with different methods of integrating content.
If you bought into a platform and a new module comes out and it is not supported on your platform you will just not be able to use it.
Additionally these platforms have strong corporate bonds.
This is mostly necessary to be able to use things that are trade marked liked logos and intellectual property.
Which means that if the core owner of these properties decides that they deserve to be payed more money it will indirectly impact all of the platforms having a legal binding with them.
The goal is to make a single fully free and open source virtual table top role playing game platform that is flexible enough to implement any system.
Focusing on very generic bits of logic required to fill a majority of the needs for an ttrpg.
Including a system independent extendability mechanism that allows module builders to support multiple systems from a single distribution.
While most modules would require additional effort to support multiple systems it would allow for sharing resources between all systems.

# how could this work

The most important piece to make this work is free hosting.
No one wants to have to work through technical complications just to relax and play.
So the approach here is to use github.io as host for the framework.
By creating git repositories it is possible to drive the database of the framework.
This organization is specifically made to allow anyone to play by just visiting vttrpg.github.io and being logged into their Github account.

By combining repositories it is possible to pick and choose what you want to play.
This repository contains the core framework.
You can select your own repository which contains your game information.
As part of the game information it will be pointing to a game mechanism repository and modules which support this game combining into your rule set.
Additionally it will point to your players their repository and which of their characters are being used.
While playing the framework will use git to store your progress.
So even without any Github knowledge a game repository can automatically be created and maintained.
For the majority of the time it will function like an interactive character sheet.
But it can also be used for realtime battles.
If you are familiar with Github.Io you might know it only hosts static resources.
So how could this static web application have realtime battles?
This can be achieved by simply opening a pull request and using Github its own websockets to get notifications when another player has taken an action.
Allowing the application to update its state after every players turn.
Am unique feature you get from this approach is that you have complete logs of everything that happened in your games.
Also as the game repository gets new updates that you might not like it is possible to keep playing the version you like as it is using git.

# plan

There currently is a very limited plan. Setup a proof of concept and add an open source game system that already exists with a very basic module that can be used for an adventure.
Not focusing on UX until it is proven that this can work and the owner of the open source game system gives their full approval.

If you are interested in helping out please get in contact.
