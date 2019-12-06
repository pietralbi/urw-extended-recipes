# Pietralunga's extended recipes 
### Mod for UnReal World 3.60 
This is a set of modifications for the roguelike game [UnReal World](http://www.unrealworld.fi/) developed by Sami Maaranen and Erkka Lehmus.

This mod started as a simple modification of [Caethan's UnReal World self-sufficiency mod](https://github.com/caethan/urw-sufficiency), 
but it slowly grew to an extensive revision of the whole crafting system.  
The extended recipes mod aims at filling the gaps left by vanilla recipes, in a balanced and vanilla-style way. It allows you to live more self-sufficiently, crafting most needed tools and items without having to obtain the via trade. 
Not everything is available -- complex armor and weapons and foreign crafts and must still be traded. Some new recipes and items were also added, such like making arrows and weapons from bones and antlers.

The main focus of this mod is:

* Historical realism
	- No unrealistic/anachronistic/out-of-place recipes.  
	 Every recipe is based on the available historical sources on Finnish/Scandinavian iron age, which took me days to look and study. If anybody notices something unhistorical, please update me with a post in the urw forums. 
	 For example, the birch-bark canoe from Caethan's self-sufficiency mod has been removed, since it was made by Native Americans using a different kind of birch, not available in Finland.
* Balance 
	- Every recipe was tested and calculated to follow vanilla guidelines, and not to be overpowered or game-spoiling.  
	 For example, the nutrition value of the added flax plant was matched to the hemp plant that already is already present in game. They both have similar nutrition values in real life, albeit in-game they are about 30% less nutrient than they are in the real world. In this case, balance came first, after all that's why it is called *UnReal World*.
* Minimalism
	- There are already several mods that extend vanilla recipes, like the [BAC mod](https://www.unrealworld.fi/forums/index.php?topic=4712.0). However, many radically alter  even the vanilla recipes, complicating them with too many ingredients and steps, which introduces too much "bloat" to my taste. This mod instead, like Caethan's one, just fills the gaps left by vanilla and only adds a few new items. No entirely new sets of items, like pottery or decorative carpentry (which then would be available to the player only).

Also includes the updates to the in-game encyclopedia from Caethan's self-sufficiency mod, plus some more, with information about new items, as well as tile graphics for them.

## Installation instructions

The first step to installing the mod is to find where Unreal World is installed on your computer.
If you've installed it manually from the developer's website, just remember where you put it. On linux, it should be in `~/.config/urw3-Linux`.  
If you have installed it from Steam:
	
* Open up the game properties by right-clicking on the game from the Steam interface and selecting "Properties".
* Switch to the "Local Files" tab.
* Click on "Browse Local Files".  This will open up a window in Finder (for Macs) or Explorer (for Windows) at the root of the installation.

Copy the following files to the main game folder:

* biy_sufficiency.txt
* diy_sufficiency.txt
* diy_glossary.txt
* diy_ironworking.txt
* diy_weaving.txt
* flora_cultivated.txt
* flora_flax.txt
* cookery_glossary.txt
* menudef_sufficiency.txt
* GAME.NFO

The files

- diy_glossary.txt
- flora_cultivated.txt 
- cookery_glossary.txt
- GAME.NFO

will be overwritten, so backup them by prefixing "backup_" to their name (if they start with diy, flora or cookery they will be still loaded by the game).

There are two subfolders in both the Unreal World folder and the mod folder:
    - "truegfx":  pictures used in the encyclopedia and for various other purposes
    - "truetile": sprites for items and creatures in the game
* Copy over the contents of each of these folders in the mod into the Unreal World folders.
You shouldn't be copying over any existing files here.
* Start up the game and enjoy the new options!


## Vanilla recipes changes

* Except the very basic recipes, switched the relative skill from COMMON to CARPENTRY or TIMBERCRAFT

* Slender trunks replaced with staffs for several recipes.  This allows staff quality to affect the final item quality, enabling you to build high quality items with some effort:
	- Grainflail
		- removed +30% skill bonus to compensate
	- Ski stick
	- Sesta
		- reduced skill bonus to +20% to compensate
* [noquality] added for some ingredients of fixed quality to avoid negatively impacting finished quality:
	- Wooden cup and bowl: block of wood
		- removed +20% skill bonus to compensate
	- Wooden shovel: block of wood
		- removed +10% skill bonus to compensate
	- Wooden stake and staff: Slender trunk
		- reduced skill bonus by 30% each to compensate

## Vanilla buildings enabled for construction

* Well
    - Dig for water nearby your settlement
* Road
    - Organize your settlement with roads


## Flora

* New cultivated (and wild) flax plant, with balanced nutrition values
* Cultivated plants can be occasionally found in the wild


## New recipes 

* Sauna scoop
* Net
* Fishing rod
* Wooden tub
* Untie a loop snare and get the cord back
* Mine stones from big rocks
* Crush stones into rocks

* Make nettle, linen and woollen clothes using scraps of pre-existing clothes, just like you can do it with leather and fur clothes in the unmodded game. Everything was balanced following the material losses from vanilla fur and leather recipes. Alternatively, you can also make clothes from the raw materials.

### Spinning and weaving

#### Nettle and linen clothes

1. Harvest hemp, nettle and flax (do not thresh them)
2. Soak and ret the plants
3. Dry the retted plants
4. Extract the fibers
	+ You can also extract fibers from existing clothes
5. Spin the fibers into a yarn using the historical [spindle](https://en.wikipedia.org/wiki/Spindle) and [distaff](https://en.wikipedia.org/wiki/Distaff) method
6. Build a loom and weave the yarn into raw cloth.
7. Tailor the raw cloth to make clothes
	+ Alternatively, raw cloth is a profitable trade good, worth x1.5 the same weight in tailored clothes. Live off as a fabric artisan!

+ You can braid the fibers into cords, with some patience
+ Braid yarn into ropes or twist it into cord
+ No hemp clothes exist in-game, so hemp is only used for cords and ropes

#### Woollen clothes
1. In summer, shear each sheep once to obtain greasy wool
	- It's not possible to implement "Be next to a sheep" or "once per year" requirement in-game, so some roleplay is required here, sorry. I hope modding capabilities will be expanded in the future.
2. Scour the greasy wool
3. Card the wool into fibers
	+ You can also extract fibers from existing clothes
4. Follow the steps for linen and nettle


### Ironworking

1. Gather bog ore from open mires
	+ To gather the surface one, you need to find an open mire next to a spruce mire or another terrain that allows digging (*not* a pine mire or an open mire). 
		1. Dig a hole at the border of the spruce mire and
		2. Stand next to the hole, in the open mire
		- This is the only trick to prevent being able to collect bog ore from *anywhere*

2. Roast the bog ore

4. Make a [charcoal clamp](https://en.wikipedia.org/wiki/Charcoal_pile) to make charcoal from firewood for smelting and smithing

5. Build a stone bloomery and a forge

6. Craft tongs, anvil, hammer and bellows
	+ Wooden tongs, stone hammer and stone anvil are good for initial smithing and do not require pre-existing iron tools.

7. Smelt the raw ore into blooms

8. Refine the bloom into wrought iron
	+ Wrought iron is very malleable and not good for blades

9. Use wrought iron to smith:
	- Iron anvil
	- Iron tongs
	- Iron hammer
	- Pot

9. Hearth-refine the wrought iron into steel 

10. Smith steel into tools and weapons, including:
    - Axes
    - Spears
    - Knives
    - Shovel
    - Sickle
    - Fish hooks


## New items
* Small and large barrels

* Stone hammer
	- Good for basic ironworking and bashing skulls
		+ Two-handed and heavy, better than a club, not as good as a maul or mace

* Northern staff-bow
	- A combination of a bow and a ski-stick, in order to hunt bow and arrow while skying. Don't expect much accuracy, tough.
		+ [Watch a demonstration from Sami](https://www.youtube.com/watch?v=Ez1CUoz0tdQ)  

* Added bone and antler weapons
    - Bone knife
		+ Better than a stone knife, not as good as a broad or hunting knife
    - Bone-tipped javelin
		+ Slightly better than simple javellin 
	- Bone-tipped arrow
		+ In-between a normal arrow and a broadhead one
	- Antler-tipped arrow
		+ In-between a normal arrow and a blunt one
	
 * Birch-bark bandage
	- A simple bandage made from birch-bark strips
	
* New iron weapons and tools:
	- Iron hammer
		+ Best for smithing, but not bad as a weapon. A maul is still better, tough. Two-handed.
	- Throwing spear
		+ Basically, a javellin with an iron spearhead. The attack is as good as a spear, but the defense is as bad as a javellin. One-handed.

## Cooking

* Render fat to tallow
* Make hard biscuits
* Roast vegetables in the fire
* Dry berries and mushrooms
* Modified existing cookery recipes to make more useful


# Sources, credits, and inspiration

Many thanks to:

* The original developers Sami Maaranen and Erkka Lehmus for creating URW and its modding system.

* Caethan, for his self-sufficiency mod, without which this mod would have not been made.  
  The extended recipes mod is a direct evolution of his sufficiency mod, and includes many of his additions, albeit modified and re-worked. 
	* https://www.unrealworld.fi/forums/index.php?topic=147.0


* The mod authors whose original work inspired this mod's development:
	* Brygun for his BAC & the community mod
		* https://www.unrealworld.fi/forums/index.php?topic=4712.0
    * Stonelobber for his Primitive World mod
		*	https://www.unrealworld.fi/forums/index.php?topic=1808.0  
		
* And many others mod authors who inspired the above mods, whose work I have known only indirectly. The link to their mods has died with the old forum, but here are included anyway:
	* Rain for his Ironworking and Cloth mods which were used as the original base for the weaving and smithing sections
		* Ironworking - http://z3.invisionfree.com/UrW_forum/index.php?showtopic=2147
		* Cloth - http://z3.invisionfree.com/UrW_forum/index.php?showtopic=1839&st=0
	* Buoidda
		* http://z3.invisionfree.com/UrW_forum/index.php?showtopic=8043
	* Endive
		* http://z3.invisionfree.com/UrW_forum/index.php?showtopic=3071
	* Lasse & Weathereye
		* http://z3.invisionfree.com/UrW_forum/index.php?showtopic=5331
    * thefinn
        * http://z3.invisionfree.com/UrW_forum/index.php?showtopic=8082

* The artists who drew the sprites
	* Kaaven (many various sprites)
		* http://z3.invisionfree.com/UrW_forum/index.php?showtopic=7331&st=0
    * thefinn (barrel sprites)

* The photographers who provided the pictures for the encyclopedia entry from Caethan's self-sufficiency mod
    * Birch-bark cap - Fanny Schertzer, CC BY-SA 3.0, https://commons.wikimedia.org/w/index.php?curid=10890204
		
* Many thanks also the various sources for informations on historical weaving, ironworking and smithing. Here are only a few of the sources I have consulted:
	* http://www.haraldthesmith.com/a-week-of-iron-smelting/
	* http://www.hurstwic.org/history/articles/manufacturing/text/bog_iron.htm
	* https://en.wikipedia.org/wiki/Bog_iron
	* https://en.wikipedia.org/wiki/Charcoal_pile
	* https://en.wikipedia.org/wiki/Charcoal
	* https://web.archive.org/web/20040315062219/http://www.geoarch.co.uk/experimental/charcoal.html
	* https://www.youtube.com/watch?v=1yK0rLQa3j4
	* https://mypeculiarnature.blogspot.com/2018/04/oroshiganemaking-steel-1.html
