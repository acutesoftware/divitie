# Mods
There are several ways to customise the game

### In Game Modifications
Each player has a home base they can modify. 
From any land |  take a boat to "Home Town" and turn left into the glowing portal saying "Home"
(you should also be able to use a Hearthstone)

The players home base is a reasonably size flat block of land |  surrounded by cliffs that you can modify as you see fit.

You can place any buildings on there once you get the materials |  and add the following features
- Rocks
- Fishing pool(s)
- Trees
- plants
- random forage spawns (Ore |  Herbs |  etc)


### External Mods

For external mods |  you create data files and import them with a script.

The following mods will be supported
- Items - define a new item: name |  material |  texture [not 100% sure if full static mesh will be importable - may need to use existing termplate]
- Crafting Recipes - using existing items in the world (including ones you add) |  make your own recipes
- NPC's - customise the look of an NPC with the character creator |  give them a back story and goals
- Quests - quests for players to try out |  using in game or generated items
- Biomes - add tree spawners |  plants |  rocks |  fishing spots |  animal spawners to the land

Each set of definitions lives in a CSV file in the mods folder of the game.

#### Environment Spawners (env_spawn.csv)
Use this table to generate rocks and plants in the map

| Spawner Name | Spawn Type | X_pos | Y_pos | radius | number to spawn |
|--------------|------------|-------|-------|--------|-----------------|
| trees near start | BP_Tree | 300 | 200 | 5000 | 20 |
| ores at mine | BP_Ore | 900 | 1000 | 2000 | 30 |

#### Built items (built_items.csv)
Generate new items by combining existing parts

Bookshelf example

| num | item_id | loc_X | loc_Y | loc_Z | rot_X | rot_Y | rot_Z | 
| 1 | SM_wood_plank_oak | 366.925568 | 66.458923 | 66.263763 | 0.0 | 0.0 | 0.0 | 
| 2 | SM_wood_plank_oak | 366.925568 | 66.458923 | 136.263763 | 0.0 | 0.0 | 0.0 | 
| 3 | SM_wood_plank_oak | 366.925568 | -53.198631 | 148.420074 | 90.000015 | 0.0 | 0.0 | 
| 4 | SM_wood_plank_oak | 366.925568 | 186.801361 | 148.420013 | 90.000015 | 0.0 | 0.0 | 
| 5 | SM_wood_plank_oak | 366.925568 | 66.458923 | 266.263763 | 0.0 | 0.0 | 0.0 | 
| 6 | SM_wood_plank_oak | 366.925568 | 66.458923 | 206.263763 | 0.0 | 0.0 | 0.0 | 
| 7 | SM_wood_plank_oak | 366.925568 | 66.458923 | 104.263763 | 0.0 | 0.0 | 0.0 | 
| 8 | SM_wood_plank_oak | 366.925568 | 294.458923 | 177.263763 | 0.0 | 0.0 | 0.0 | 
| 9 | SM_wood_plank_oak | 366.925568 | 403.801361 | 148.420013 | 90.000015 | 0.0 | 0.0 | 
| 10 | SM_wood_plank_oak | 366.925568 | 302.458923 | 116.263763 | 0.0 | 0.0 | 0.0 | 
| 11 | SM_wood_plank_oak | 366.925568 | 302.458923 | 265.263763 | 0.0 | 0.0 | 0.0 | 
| 12 | SM_wood_plank_oak | 366.925568 | 302.458923 | 64.263763 | 0.0 | 0.0 | 0.0 | 

