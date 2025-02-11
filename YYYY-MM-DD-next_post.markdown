---
layout: post
title:  "This Month in Minetest 1"
description: >
  A new minetest version and new content
hero: /_posts/img/pig.png
overlay: White
published: true
---
---
# Table of contents
*  [Briefing](#overview)
*  [Engine](#engine)
*  [Games](#games)
*  [Mods](#mods)
*  [Art/Builds](#art)
*  [Server News](#s-news)
*  [In Other News](#o-news)


## Briefing <a name="overview"></a>
------------------------------------------------
Minetest 5.5 was released last month, with some significant improvements. Colour Hop has received some major updates. Creatura has joined minetest's collection of performant mob apis.

## Engine News <a name="engine"></a>
------------------------------------------------
<sup>Written by MisterE and Rubenwardy</sup>

Minetest 5.5.0 has been released! 

While you may not see many visible changes, there's been a considerable amount of work under the hood to improve the rendering system. Minetest now uses its own fork of the Irrlicht rendering library, which will make further improvement easier. It's already allowed several longstanding bugs to be fixed. 

Be warned: when you update to 5.5, it'll upgrade worlds to a new map encoding. This is irreversible, and will prevent you from running those worlds on older Minetest versions. If you aren't sure about the upgrade, then backup your map beforehand. 

There were some interesting changes to the modding API. Various features have been de-hardcoded, allowing mods and games more control. For example, liquid features have been decoupled from liquid drawtypes (making it easier to make things like spiderwebs). Player fall damage is also changeable using armor groups; you can avoid red flashes from disabled fall damage. 

Possibly the most interesting change to the API was an upgrade to the dynamic media API. Modders and game creators can now send media to individual clients, and label it as "ephemeral", meaning the client will forget it when they disconnect. Previously, dynamic media was sent to all clients, and became part of the media sent to clients on when they joined. With the new version, individualized media is finally possible! The applications are huge, especially regarding background music (BGM), which used to extend login times enormously. BGM can now be sent one track at a time after the player has joined. 

As always, you can check out [the full changelog](https://dev.minetest.net/Changelog#5.4.0_.E2.86.92_5.5.0). Also see the [official announcement](https://forum.minetest.net/viewtopic.php?f=18&t=27754).


## Game News <a name="games"></a>
------------------------------------------------

![A New Place](/_posts/img/a_new_place.png?raw=true "A New Place")
![The Royal Blob](/_posts/img/the_royal_blog.png?raw=true "The Royal Blob")

Talas has just released version 1.2 of Colour Hop! 
This includes some fundamental changes to the game, giving each player colour an activated ability.
The story (or lack of) has been expanded upon and a completely new boss was added.
There are some new advanced buildings that players can build, most are unrelated to the dragons.
As usual, things are hidden and finding the new boss will take much exploration.
The game is still a work-in-progress, but it's getting closer to a complete game.

![SuperSam](https://content.minetest.net/uploads/38591f9f94.png "Super Sam Adventures")

Super Sam Adventures is a WIP jump'n'run game by BuckarooBanzai that seems to promise fun platforming for minetest. While it is obviously in early stages of development, it is already  playable, and even slightly engaging, with secret areas, moving platforms, and several levels.


## Mod News <a name="mods"></a>
------------------------------------------------

ElCeejo has released a trio of updates to his animal mods, as well as a new mob api to base them on. 

![The Monster Invades](/_posts/img/the_monster_invades.png?raw=true "The Monster InvadesBlob")

Draconis improves the gameplay of multiple Minetest games, like Minetest Game, Voxelgarden, and MineClone. It gives more incentive to traverse your worlds' mountains and caves, and provides engaging mini-boss fights. After defeating a Dragon, you may find an Egg. The mysterious Egg-hatching process can be puzzling, but it rewards you with a new, destructive companion with which you can take to the skies when its old enough, and it unlocks a new tier of weaponry and armor. The Libri Draconis book can help you discover elements of the mod by unlocking certain objectives with the book in your inventory.


Animalia adds life and depth to experiences with livestock, pets, and ambient creatures. You can create farms for eggs, milk, and meat. You can use a Horse to quickly traverse ground, perhaps with a Wolf companion at your side. And you can enjoy ambient sounds of in-game Animals throughout most biomes. The builtin documentation, Libri Animalia, acts as a journal which you expand by clicking on animals with the book. There is currently a vote underway on the forums for which set of animals to add next to Animalia.

Creatura makes creating a new mob relatively easy, while not cutting corners on features. You can take advantage of the Utility Stack system for smooth decision making, enchance behaviors using Theta* Pathfinding for lifelike paths, and even use the implemented boids algorithm for realistic flocks and swarms. 


Loosewheel has been updating lw_components with more mesecons devices. The latest additions were digilines-controlled storage, and a security camera that can actually take "photos"- rough representations of the scene in front of it that remind you of early maze graphics. One of the most exciting recent additions is a force field generator:
![Force Field](https://i.ibb.co/sbRcL9v/force-field-demo.png?raw=true "Force Field")
lw_components seems to be a real contender to other mesecons-compatible automation mods, and without the high entity-count, it may be a lower lag option. 

OgelGames has released a mod that adds a wearable headlamp on Content Database (CDB).

Zughy is back at modding again! He recently updated Arena_lib, adding the ability to control the sky to minigames made with the library. It allows you to tweak clouds, sky colors, skybox backgrounds, and more!
![Pink Sky](/_posts/img/pink_sky.png?raw=true "Pink Sky")

Apercy is back at it again, making more great vehicle mods. This time its cars. These cars are two-seaters. They have working headlights. They have wheels and steering wheels that turn. They run on fuel. They detect elevation and tilt to match the elevation under them. Best of all, they are low-lag and extremely playable. The latest addition to the fleet is the coupe below:
![Apercy's Coupe](/_posts/img/apercycars.png?raw=true "Apercy's Coupe")

## Art and Builds <a name="art"></a>
------------------------------------------------


![An Essay in Dwarf-Sculpture](/_posts/img/essay_in_dwarf.png?raw=true "An Essay in Dwarf-Sculpture")

The Dwarves of the YourLand server show off stonework: "An Essay in Dwarf-Sculpture", built by debian44.

temhotaokeaha has been making cool banners for games:
![Blockbomber Banner](https://content.minetest.net/thumbnails/2/09924ef1ef.png?raw=true "Blockbomber Banner")
![FarLands Reloaded Banner](https://content.minetest.net/thumbnails/2/cb60513e6c.png "FarLands Reloaded Banner")


## Server News <a name="s-news"></a>
------------------------------------------------

runs' server is back online; this time running the development version of his new game "The Samz". Its limited to 3 players currently.

## In Other News <a name="s-news"></a>
------------------------------------------------
This is the first post of our blog, y'all! We are actively looking for content submission for the next post, which will be in about a month, maybe sooner. Let us know what you are doing! If you are working on something great for Minetest in any of the following categories, please follow the easy instructions in the About page to submit content or contact MisterE on discord, matrix, or the forums to submit content without the hassle of the issue tracker (please use the issue tracker if you can, though!)

Categories:
* Engine
* Games
* Mods
* Art/Builds
* Server Spotlight
* Server News
* In Other News

The "In Other News" is the place for basically anything else minetest related, so theres a place for everything here. Submissions must meet the submission guidelines on the About page, and are subject to editor review and revision.





