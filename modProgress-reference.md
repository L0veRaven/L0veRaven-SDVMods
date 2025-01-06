# Mod Progress Reference

```mermaid
graph TD;
    Content Patcher-->Change Mechanics;
    Change Mechanics-->Buffs;
        Buffs-->Data/Buffs;
            Data/Buffs-->Persistent Buffs;
    Change Mechanics-->Combat;
            Combat-->OOOOOOOOOOOOOOO;
    Change Mechanics-->Farm Cave;
            Farm Cave-->OOOOOOOOOOOOOOO;
    Change Mechanics-->Farmhouse;
            Farmhouse-->OOOOOOOOOOOOOOO;
    Change Mechanics-->Fishing Treasure;
            Fishing Treasure-->OOOOOOOOOOOOOOO;
    Change Mechanics-->Forage Spawn;
            Forage Spawn-->OOOOOOOOOOOOOOO;
    Change Mechanics-->Mine Ore / Chests;
            Mine Ore / Chests-->OOOOOOOOOOOOOOO;
    Change Mechanics-->Museum Rewards;
            Museum Rewards-->OOOOOOOOOOOOOOO;
    Change Mechanics-->Panning;
            Panning-->OOOOOOOOOOOOOOO;
    Change Mechanics-->Train Loot;
            Train Loot-->OOOOOOOOOOOOOOO;
    Change Mechanics-->Trigger Actions & GSQs;
            Trigger Actions & GSQs-->OOOOOOOOOOOOOOO;
    
    Content Patcher-->Change Visuals;
    
    Content Patcher-->Add New Content;
```

## Content Patcher

### Change mechanics

| Area of Focus | Directory | Existing Mods |
| --- | --- | --- |
| Combat | ```Data/Monsters```, ```Data/MonsterSlayerQuests```| ```___``` |
| Farm Cave | ```___``` | ```Modifiable Fruit Region```, ```Mushroom Box Location Framework``` |
| Farmhouse | ```Data/HomeRenovations``` | ```Personal Indoor Farm``` |
| Fishing Treasure | ```___``` | ```Item Extensions``` |
| Forage Spawn | ```___``` | ```Farm Type Manager```, ```SpaceCore``` |
| Mine Ore / Chests | ```___``` | ```Farm Type Manager```, ```Mine Treasure Framework```, ```SpaceCore``` |
| Museum Rewards | ```Data/MuseumRewards``` | ```___``` |
| Panning | ```___``` | ```Item Extensions``` |
| Train Loot | ```___``` | ```___```, ```Item Extensions``` |
| Trigger Actions & GSQs | ```Data/TriggerActions``` | ```Button's Extra Trigger Action Stuff (BETAS)```, ```SpaceCore``` |

### Change visuals

| Area of Focus | Directory | Existing Mods |
| --- | --- | --- |
| Animated Textures | ```___``` | ```SpaceCore: TextureOverrides```, ```Prismatic Valley Framework```, ```Content Patcher Animations``` |
| Editing Text / Translations | ```Data/___```, ```Data/___```, ```Data/WorldMap```, ```Data/WildTrees```, ```Data/Weddings```, ```Data/Weapons```, ```Data/Trinkets```, ```Data/TriggerActions```, ```Data/Tools```, ```Data/TailoringRecipes```, ```Data/SpecialOrders```, ```Data/Shops```, ```Data/Shirts```, ```Data/SecretNotes```, ```Data/RandomBundles```, ```Data/Quests```, ```Data/Powers```, ```Data/Pets```, ```Data/PassiveFestivals```, ```Data/Pants```, ```Data/PaintData```, ```Data/Objects```, ```Data/NPCGiftTastes```, ```Data/MuseumRewards```, ```Data/MoviesReactions```, ```Data/Movies```, ```Data/MonsterSlayerQuests```, ```Data/Monsters```, ```Data/Minecarts```, ```Data/Mannequins```, ```Data/MakeoverOutfits```, ```Data/mail```, ```Data/Machines```, ```Data/Locations```, ```Data/LocationContexts```, ```Data/JukeboxTracks```, ```Data/IncomingPhoneCalls```, ```Data/HomeRenovations```, ```Data/hats```, ```Data/HairData```, ```Data/GiantCrops```, ```Data/GarbageCans```, ```Data/Furniture```, ```Data/FruitTrees```, ```Data/FloorsAndPaths```, ```Data/FishPondData```, ```Data/Fish```, ```Data/Fences```, ```Data/FarmAnimals```, ```Data/ExtraDialogue```, ```Data/EngagementDialogue```, ```Data/Crops```, ```Data/CraftingRecipes```, ```Data/CookingRecipes```, ```Data/ConcessionTastes```, ```Data/Concessions```, ```Data/Characters```, ```Data/ChairTiles```, ```Data/Bundles```, ```Data/Buildings```, ```Data/Buffs```, ```Data/Boots```, ```Data/BigCraftables```, ```Data/AudioChanges```, ```Data/AquariumFish```, ```Data/animationDescriptions```, ```Data/AdditionalLanguages```, ```Data/AdditionalWallpaperFlooring```, ```Data/AdditionalFarms```, ```Data/Achievements```, ```Data/TV/TipChannel```, ```Data/TV/CookingChannel```, ```Data/Festivals/FestivalDates```, ```Data/Festivals/{{season}}dd```, ```Data/Events/_locationName_```, ```Strings/WorldMap```, ```Strings/Weapons```, ```Strings/UI```, ```Strings/StringsFromMaps```, ```Strings/StringsFromCSFiles```, ```Strings/SpeechBubbles```, ```Strings/SpecialOrderStrings```, ```Strings/SimpleNonVillagerDialogues```, ```Strings/Shirts```, ```Strings/Quests```, ```Strings/Pants```, ```Strings/Objects```, ```Strings/NPCNames```, ```Strings/Notes```, ```Strings/Movies```, ```Strings/MovieReactions```, ```Strings/MovieConcessions```, ```Strings/Locations```, ```Strings/Lexicon```, ```Strings/Furniture```, ```Strings/FarmAnimals```, ```Strings/Events```, ```Strings/EnchantmentNames```, ```Strings/Characters```, ```Strings/BundleNames```, ```Strings/Buildings```, ```Strings/BigCraftables```, ```Strings/animationDescriptions```, ```Strings/M_D_Strings```, ```Characters/Dialogue/{{NPC}}```, ```Strings/schedules/{{NPC}}``` | ```Project Fluent``` |
| Recolors | Any game sprite | ```Theme Manager``` |
| Texture Scaling | ```___``` | ```Sprites in Detail```, ```Portraiture``` , ```SpaceCore``` , ```Scale Up``` |
| Variety in Textures | ```___``` | ```Alternative Textures```, ```Toggle Items Framework```, ```Even Better Artisan Goods Icons``` |

### Add New Content

#### Farmer Attire

| Area of Focus | Directory | Existing Mods |
| --- | --- | --- |
| Accessories | ```___``` | ```Fashion Sense``` |
| Clothing | ```Data/Hats```, ```Data/Shirts```, ```Data/Pants```, ```Data/Boots```, ```Data/TailoringRecipes```, | ```Fashion Sense``` |
| Hair | ```Data/HairData``` | ```Fashion Sense``` |

#### Story

| Area of Focus | Directory | Existing Mods |
| --- | --- | --- |
| Bundles | ```Data/Bundles```, ```Data/RandomBundles``` Edit with caution | ```Unlockable Bundles``` |
| Dialogue | ```Characters/Dialogue```, etc. | ```___```, ```___``` |
| Events | ```Data/Events```, etc. | ```More Nightly Events```, ```Expanded Preconditions Utility``` |
| Festivals | ```Data/Festivals```, ```Data/PassiveFestivals``` | ```___``` |
| Mail | ```Data/Mail``` | ```Mail Framework Mod``` |
| Powers | ```Data/Powers``` | ```Special Power Utilities``` |
| Quests | ```Data/Quests``` | ```___```, ```___``` |
| Secret Notes | ```___``` | ```Secret Note Framework``` |
| Special Orders | ```Data/SpecialOrders``` | ```Untimed Special Orders```, ```Esca's Modding Plugins``` |

#### NPCs

| Area of Focus | Directory | Existing Mods |
| --- | --- | --- |
| Dateable NPCs | ```Data/EngagementDialogue```, ```Characters/Dialogue/MarriageDialogue```, ```Data/Weddings``` | ```___``` |
| Friendable NPCs | ```Data/Characters```, ```Data/NPCGiftTastes```, ```Characters/{{NPC}}```, ```Portraits/{{NPC}}```, ```Characters/schedules/{{NPC}}``` | ```___``` |
| Non-Friendable NPCs | ```___``` | ```Custom Companions```, ```Custom NPC Exclusions``` |

#### Animals

| Area of Focus | Directory | Existing Mods |
| --- | --- | --- |
| Critters | ```___``` | ```Custom Companions``` |
| Farm Animals | ```Data/FarmAnimals``` | ```Extra Animal Configs``` |
| Monsters | ```___``` | ```Farm Type Manager``` |
| Pets | ```Data/Pets``` | ```Hats on Pets Plus```, ```Pet Store``` , ```Baby Pets``` |

#### Maps

| Area of Focus | Directory | Existing Mods |
| --- | --- | --- |
| Buildings | ```Data/Buildings``` | ```Solid Foundations```, ```Robin Build Position``` |
| Farms | ```Data/AdditionalFarms``` | ```Spacecorw: Buildings, Fences```, ```Custom Farm Loader``` |
| Garbage Cans | ```Data/GarbageCans``` | ```___``` |
| Locations | ```Data/Locations```, ```Data/LocationContexts```, ```Data/WorldMap``` | ```Buildings Included```, ```Extra Map Actions```, ```Bush Bloom Mod```, ```Esca's Modding Plugins```, ```Mapping Extensions and Extra Properties (MEEP))```, ```Misc Map Action Properties```, ```Cloudy Skies``` |
| Minecarts | ```Data/Minecrarts``` | ```Transport Framework``` |
| Mines | ```___``` | ```SpaceCore``` |
| Music | ```Data/AudioChanges``` | ```___``` |
| Shops | ```Data/Shops``` | ```Livestock Bazaar```, ```Shop Tile Framework``` |

#### Objects

| Area of Focus | Directory | Existing Mods |
| --- | --- | --- |
| Crops | ```Data/Crops```, ```Data/GiantCrops``` | ```Custom Bush```, ```Item Extensions```, ```Forage Crops``` |
| Fences | ```Data/Fences``` | ```___``` |
| Fish | ```Data/Objects```, ```Data/AquariumFish```, ```Data/Fish```, ```Data/FishPondData``` | ```Colorful Fish Ponds``` |
| Furniture | ```Data/Furniture``` | ```Furniture Framework```, ```Calcifer```, ```SpaceCore```, ```Expanded Storage```, ```Custom TV Channel```, ```Catalogue Framework``` |
| Machines | ```Data/BigCraftables```, ```Data/Machines``` | ```Extra Machine Configs```, ```Producer Framework Mod```, ```Machine Terrain Framework```, ```Custom Crafting Stations``` |
| Minerals / Artifacts / Fruits / Vegetables / Foods | ```Data/Objects``` | ```SpaceCore```, ```Json Assets``` |
| Ore Nodes | ```___``` | ```Item Extensions``` |
| Recipes | ```Data/CookingRecipes```, ```Data/CraftingRecipes``` | ```Better Crafting```, ```Craft Anything Framework``` |
| Rings | ```Data/Objects``` | ```SpaceCore``` |
| Trees | ```Data/FruitTrees```, ```Data/WildTrees``` | ```Tree Size Framework```, ```Custom Moss``` |
| Trinkets | ```Data/Trinkets``` | ```Trinket Tinker``` |
| Wallpaper / Floors / Paths | ```Data/AdditionalWallpaperFlooring```, ```Data/FloorsAndPaths``` | ```___``` |
| Weapons | ```Data/Weapons``` | ```Slingshot Framework``` |

## C# Mods

| Area of Focus | Directory | Existing Mods |
| --- | --- | --- |
| Advanced Audio | ```___``` | ```___``` |
| Changing Game Code | ```___``` | ```___``` |
| Custom Monsters | ```Data/Monsters``` | ```___``` |
| Custom Ring Effects | ```Data/Objects``` | ```___``` |
| Edit Hardcoded Data | ```___``` | ```___``` |
| Menus / UI | ```___``` | ```Stardew UI```, ```SpaceCore```, ```UI Helper``` |
| New Achievements | ```Data/Achievements``` | ```___``` |
| New Minigames | ```___``` | ```___``` |
| New Skills | ```___``` | ```___``` |
| New Tools | ```Data/Tools``` | ```___``` |
| Special Buffs | ```Data/Buffs``` | ```___``` |
| Special Object Behavior | ```Data/Objects``` | ```___``` |