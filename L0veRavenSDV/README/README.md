# [CP] Raven
A neko lives in a tent in Cindersap Forest, hoping to save up enough money to have a home again.

## Troubleshooting Tips

If you encounter any bugs, even if it only occurs once, get your SMAPI log report [by following this tutorial](https://www.youtube.com/watch?v=za-4YvJZVYg), then send it to me.

Contact me at support@l0veraven.com or Discord at L0veRaven where I'll look at it within 24 hours.

## Keys

| Key | Meaning |
| ------------- | ------------- |
| //portraitBookmark | Assign portraits (i18n only) |
| //ADD | Find referenced code and remove flag once added |
| //review | Check if code is worth keeping |
| //DELETE | Delete when it's confirmed it won't break the mod |
| ###Delete | Delete when mod if complete |
| #T | Test code |
| #C | Don't touch the code |
| #NS | Not Started |
| WIP | Work In Progress |

## Animation Keys (in i18n)

| Key | Meaning |
| ------------- | ------------- |
| aniSweep | ```l0veraven_raven_sweep``` |
| aniRead | ```l0veraven_raven_read``` |
| aniStand | ```l0veraven_raven_stand``` |
| aniBlunt | ```l0veraven_raven_blunt``` |

## Destination Times

| Location ```Token``` | Duration (HH:MM) |
| ------------- | ------------- |
| (Vanilla) Tent ```{{RavenStandStove}}``` to Saloon ```{{RavenSweepJobSaloon1}}``` | 1:50 |
| (Vanilla) Tent ```{{RavenInBed}}``` to Beach ```{{RavenRelaxBeach}}``` | 2:00 |
| (Vanilla) Tent ```{{RavenInBed}}``` to Bus Stop ```{{RavenStandBusStop}}``` | 3:00 |
| ------------------------------------------------------------------------------- | ----- |
| (SVE) Tent ```{{RavenStandStove}}``` to ___ ```{{___}}``` | ___ |
| (SVE) Tent ```{{RavenInBed}}``` | ___ |
| ------------------------------------------------------------------------------- | ----- |
| Apartment ```{{RavenStandStove}}``` to ___ ```{{___}}``` | ___ |
| Apartment ```{{RavenInBed}}``` | ___ |
| ------------------------------------------------------------------------------- | ----- |
| Beach ```{{RavenRelaxBeach}}``` to (Vanilla) Tent ```{{RavenStandStove}}``` | 3:00 |
| ------------------------------------------------------------------------------- | ----- |
| (Vanilla) Forest ```{{pissBush}}``` | ___ |
| (SVE) Forest ```{{pissBush}}``` | ___ |
| ------------------------------------------------------------------------------- | ----- |
| (Vanilla) ```{{RavenRelaxForest}}``` | ___ |
| (SVE) ```{{RavenRelaxForest}}``` | ___ |
| ------------------------------------------------------------------------------- | ----- |
| (Vanilla) ```{{RavenStandRiverForest}}``` | ___ |
| (SVE) ```{{RavenStandRiverForest}}``` | ___ |
| ------------------------------------------------------------------------------- | ----- |
| Town ```{{RavenStandCC}}``` | ___ |
| Town ```{{RavenRelaxBushTown}}``` | ___ |
| ------------------------------------------------------------------------------- | ----- |
| Clinic ```{{RavenStandMeds}}``` | ___ |
| ------------------------------------------------------------------------------- | ----- |
| Saloon ```{{RavenSweepJobSaloon1}}``` | ___ |
| Saloon ```{{RavenSweepJobSaloon2}}``` | ___ |
| Saloon ```{{RavenSweepJobSaloon3}}``` to Bus Stop ```{{RavenStandBusStop}}``` | 1:30 |
| Saloon ```{{RavenSweepJobSaloon3}}``` to (Vanilla) Tent ```{{RavenStandStove}}``` | 2:00 |
| Saloon ```{{RavenStandTableSaloon}}``` | ___ |
| ------------------------------------------------------------------------------- | ----- |
| (Vanilla) ArchaeologyHouse ```{{RavenStandBookcase}}``` | ___ |
| (SVE) ArchaeologyHouse ```{{RavenStandBookcase}}``` | ___ |
| ------------------------------------------------------------------------------- | ----- |
| Beach ```{{RavenRelaxBeach}}``` | ___ |
| ------------------------------------------------------------------------------- | ----- |
| Mountain ```{{RavenStandMountain}}``` | ___ |

## Schedule Keys (in i18n)

| Key | Meaning |
| ------------- | ------------- |
| RavenStandBusStop | ```BusStop 20 22 2``` |
| ___ | ___ |
| RavenStandRiverForest | ```Forest 39 75 3``` |
| RavenStandRiverForest_SVE | ```Forest 64 89 3``` |
| ___ | ___ |
| RavenRelaxForest | ```Forest 56 81 3``` |
| RavenRelaxForest_SVE | ```Forest 90 89 3``` |
| ___ | ___ |
| standStove | ```Custom_L0veRaven_RavenTentInside 2 3 0 \"Strings\\schedules\\L0veRaven_Raven:Custom_L0veRaven_RavenTentInside.001\"``` |
| standStoveSVE | ```Custom_L0veRaven_RavenTentInsideSVE 2 3 0 \"Strings\\schedules\\L0veRaven_Raven:Custom_L0veRaven_RavenTentInside.001\"``` |
| standStoveApt | ```FRL_NPCApt_Floor1 13 13 0 \"Strings\\schedules\\L0veRaven_Raven:Custom_L0veRaven_RavenTentInside.001\"``` |
| ___ | ___ |
| inBed | ```Custom_L0veRaven_RavenTentInside 3 4 1 l0veraven_raven_sleep``` |
| inBed_SVE | ```Custom_L0veRaven_RavenTentInsideSVE 3 4 1 l0veraven_raven_sleep``` |
| inBedApt | ```FRL_NPCApt_Floor1 7 13 0 l0veraven_raven_sleep``` |
| ___ | ___ |
| standCC_SVE | ```Town 60 17 2``` |
| ___ | ___ |
| standBushTown_SVE | ```Town 47 77 2``` |
| ___ | ___ |
| standCheckUp_SVE | ```Hospital 4 6 1``` |
| ___ | ___ |
| standJobSaloon1 | ```Saloon 5 17 2``` |
| standJobSaloon2 | ```Saloon 23 22 2``` |
| standJobSaloon3 | ```Saloon ___ ___ ___``` |
| standTableSaloon | ```Saloon 43 22 2``` |
| ___ | ___ |
| standBookcase | ```ArchaeologyHouse --- --- ---``` |
| standBookcase_SVE | ```ArchaeologyHouse 7 18 3``` |
| ___ | ___ |
| relaxBeach_SVE | ```Beach 43 23 2``` |
| ___ | ___ |
| standMountain | ```Mountain 57 33 1``` |

## File Directory

GENERAL - FOCUS ON VANILLA MECHANICS FIRST

#### Move custom tilesheets into L0veRaven.CoreCP
#### Fix map patch (Check for if {{Raven}}Apartment has not been changed to {{Raven}}_Apartment)


| assets/Characters | Notes |
| ------------- | ------------- |
| index.png | #C |
| L0veRaven_Raven.png | #C |
| L0veRaven_RavenBeach.png | #C |
| L0veRaven_RavenCactus.png | #C |
| L0veRaven_RavenDaisy.png | #C |
| L0veRaven_RavenFall.png | #C |
| L0veRaven_RavenFlowerDance.png | #C |
| L0veRaven_RavenNeutral.png | #C |
| L0veRaven_RavenNude.png | #C |
| L0veRaven_RavenSpring.png | #C |
| L0veRaven_RavenSummer.png | #C |
| L0veRaven_RavenSunflower.png | #C |
| L0veRaven_RavenWeed.png | #C |
| L0veRaven_RavenWinter.png | #C |

| assets/Portraits | Notes |
| ------------- | ------------- |
| index.png | #C |
| L0veRaven_Raven.png | #C |
| L0veRaven_RavenBeach.png | #C |
| L0veRaven_RavenCactus.png | #C |
| L0veRaven_RavenDaisy.png | #C |
| L0veRaven_RavenFall.png | #C |
| L0veRaven_RavenFlowerDance.png | #C |
| L0veRaven_RavenNeutral.png | #C |
| L0veRaven_RavenNude.png | #C |
| L0veRaven_RavenSpring.png | #C |
| L0veRaven_RavenSummer.png | #C |
| L0veRaven_RavenSunflower.png | #C |
| L0veRaven_RavenWeed.png | #C |
| L0veRaven_RavenWinter.png | #C |

| data/dialogue/dialogue.json | Notes |
| ------------- | ------------- |
| First of Season Dialogue | #C |
| Birthday & Checkup Dialogue | #C |
| Festival Dialogue (Yesterday, Today, Tomorrow) | #C |
| Seasons (May Not Appear In-Game) | #C |
| Generic Seasonal Dialogue (Mon, Thu) | #C |
| Generic Dialogue (Tue, Sun) | #C |
| Heart Dialogue (Wed, Fri, Sat) | #C |
| 8 Hearts - Dating | #C |
| Weather - Green Rain | #C |
| Weather - Spring Rain | #C |
| Weather - Spring Storm | #C |
| Weather - Spring Wind | #C |
| Weather - Summer Rain | #C |
| Weather - Summer Storm | #C |
| Weather - Fall Rain | #C |
| Weather - Fall Storm | #C |
| Weather - Fall Wind | #C |
| Weather - Winter Rain | #C |
| Weather - Snow | #C |
| Festival Dialogue - In Events | #C |
| Conversation Topics - Default | #C |
| Conversation Topics - Custom | WIP ```//ADD``` |
| Movies Invitation/Rejection | #C |
| Island Dialogue | #C |
| Location Entry Dialogue | #C |
| Dating | #C |
| Divorced | #C |
| Engaged | #C |
| Marriage Topics | #C |
| Summit Dialogue | #C |

| data/dialogue/giftResponses.json | Notes |
| ------------- | ------------- |
| ___ | ___ |

| data/dialogue/marriageDialogue.json | Notes |
| ------------- | ------------- |
| ___ | ___ |

| data/dialogue/moviesReactions.json | Notes |
| ------------- | ------------- |
| ___ | ___ |

| data/dialogue/scheduleDialogue.json | Notes |
| ------------- | ------------- |
| ___ | ___ |

| data/locations/LocationsData.json | Notes |
| ------------- | ------------- |
| ___ | ___ |

| data/locations/mapPatches.json | Notes |
| ------------- | ------------- |
| ___ | ___ |

| data/locations/WorldMap.json | Notes |
| ------------- | ------------- |
| ___ | ___ |

| data/maps | Notes |
| ------------- | ------------- |
| L0veRaven_RavenApartment.tmx | #C |
| L0veRaven_RavenSpousePatio.tmx | #C |
| L0veRaven_RavenSpouseRoom.tmx | #C |
| L0veRaven_RavenTentInside.tmx | Swap bed and book positions |
| L0veRaven_RavenTentOutdoors.tmx | Patch over SDVE's nature spawn |
| L0veRaven_RavenTentSnow.tmx | #T |
| stringsFromMaps.json | WIP |
| z_L0veRaven_Tent.png | WIP |

| data/outfits.json | Notes |
| ------------- | ------------- |
| Spirit's Eve Costumes - Vampire | #NS |

| data/home.json | Notes |
| ------------- | ------------- |
| Tent Spawn (Vanilla) | #C |
| Tent Spawn (SVE) | #C |
| Apartment Spawn | WIP |

| data/animationFrames.json | Notes |
| ------------- | ------------- |
| _beach_towel | #NS |
| _beach_dance | #NS |
| _beach_drink | #NS |
| _beach_umbrella | #NS |
| _handheld_game | #NS |
| _gardening | #NS |
| _sweep | #NS |
| _drink | #NS |
| _sing | #NS |
| _laugh | #NS |
| _sit | #NS |
| _read | #NS |
| _jump | #NS |
| _fishing | #NS |

| data/festivals.json | Notes |
| ------------- | ------------- |
| ___ | ___ |

| data/mail.json | Notes |
| ------------- | ------------- |
| {{ModId}}_marriageTalk_1 | Add letter content |
| {{ModId}}_marriageTalk_2 | Add letter content |
| {{ModId}}_marriageTalk_3 | Add letter content |

| data/events.json | Notes |
| ------------- | ------------- |
| Event 1590166: CatAdoption | #C |
| Event 0: CatLover | Does end dialogue work correctly; Does BGM match; Check i18n dialogue |
| Event 1: CheckIn | Does BGM match; Check i18n dialogue |
| Event 2: WildClans | Does BGM match; Check i18n dialogue |
| Event 3: CleansingFarmer | Does BGM match; Check i18n dialogue |
| Event 4: CleansingFarmer2 | Does BGM match; Check i18n dialogue |
| Event 5: jobInterview | WIP |
| Event 6: marriageTalk | #T |
| Event 7: ravenApartment | WIP |

| i18n/default.json | Notes |
| ------------- | ------------- |
| "addDialogue" | Remove from code |

| data/dialogue/dialogue.json | Notes |
| ------------- | ------------- |
| Conversation Topics: Custom | //ADD |

| content.json: ConfigSchema | Notes |
| ------------- | ------------- |
| {{CleanLanguage}} | i18n #NS (all keys prefixed with "clean_") |
| {{RavenNude}} | #C |
| {{VampireCostumeSE}} | #NS |
| {{RavenCactusCostumeSE}} | #T |
| {{RavenDaisyCostumeSE}} | #T |
| {{RavenSunflowerCostumeSE}} | #T |
| {{RavenWeedCostumeSE}} | #T |
| {{RavenIndex}} | ###Delete |
| {{RavenEventExcludes}} | ###Delete |

| content.json: CustomLocations | Notes |
| ------------- | ------------- |
| Custom_L0veRaven_RavenTentInside | #C |

| content.json: Changes | Notes |
| ------------- | ------------- |
| Blank Loads | ```Characters/Dialogue/{{ModId}}```, ```Characters/Dialogue/MarriageDialogue{{ModId}}```, ```Characters/schedules/{{ModId}}```, ```Strings/Schedules/{{ModId}}```, ```Data/Events/Custom_L0veRavenRaven_TentInside``` |
| Locations | ```data/locations/WorldMap.json```, ```data/locations/MapPatches.json```, ```data/locations/warps.json```, ```data/locations/LocationsData.json``` |
| Spouse Patio | ```data/maps/{{Raven}}SpousePatio.tmx``` |
| Spouse Room | ```data/maps/{{Raven}}SpouseRoom.tmx``` |
| NPC Data | ```data/animationFrames.json```, ```data/concessionTastes.json```, ```data/NPCGiftTastes.json```, ```data/schedule.json```, ```data/events.json```, ```data/festivals.json```, ```data/mail.json```, ```data/character.json```, ```data/outfits.json```, ```data/home.json```, ```data/winterStarGifts.json```, ```data/triggerActions.json``` |
| Dialogue | ```data/dialogue/dialogue.json```, ```data/dialogue/marriageDialogue.json```, ```data/dialogue/giftResponses.json```, ```data/dialogue/moviesReactions.json```, ```data/StringsFromCSFiles.json```, ```data/maps/StringsFromMaps.json```, ```data/dialogue/scheduleDialogue.json``` |
| ModCompat | ```data/modCompat/CJBWarps.json```, ```data/modCompat/naturesBounty.json```, ```data/modCompat/RavenEventExcludesDELETE.json```, ```data/modCompat/downtownZuzu.json```, ```data/modCompat/ridgesideVillage.json```, ```data/modCompat/pelicanTownPotluck.json```, ```data/modCompat/fireworksFestival.json```, ```data/modCompat/solsticeWinterStar.json```, ```data/modCompat/stardewValleyExpanded.json``` |

| manifest.json | Notes |
| ------------- | ------------- |
| Name | (CP) Raven |
| Author | L0veRaven |
| Nexus ID | 27407 |
| UniqueID / ModId | L0veRaven.Raven |

| manifest.json: Dependencies | Notes |
| ------------- | ------------- |
| Airyn.CPSolsticeWinterStar | #T |
| CJBok.CheatsMenu | #C |
| DTZ.DowntownZuzuDLL | WIP |
| FireRedLily.NPCApartments | #C |
| FlashShifter.StardewValleyExpandedCP | #C |
| L0veRaven.Core | #C |
| LenneDalben.PelicanTownPotluck | #T |
| Rafseazz.RSVCP | WIP |
| Raspb3rryfields.NaturesBounty | WIP |
| spacechase0.SpaceCore | #C |
| violetlizabet.CP.FireworksFestival | #T |

## Mod Compats

| data/modCompat/stardewValleyExpanded.json | Notes |
| ------------- | ------------- |
| ___ | ___ |

| data/modCompat/solsticeWinterStar.json | Notes |
| ------------- | ------------- |
| Event Dialogue | #T |

| data/modCompat/ridgesideVillage.json | Notes |
| ------------- | ------------- |
| Ridgeside Gathering | #T |
| Ridgeside Gathering - Dialogue | #T |
| Ember of Resolutions | #T |
| Ember of Resolutions - Dialogue | #T |

| data/modCompat/pelicanTownPotluck.json | Notes |
| ------------- | ------------- |
| Dialogue (Yesterday, Today, Tomorrow) | #T |

| data/modCompat/fireworksFestival.json | Notes |
| ------------- | ------------- |
| Festival | #T |

| data/modCompat/downtownZuzu.json | Notes |
| ------------- | ------------- |
| Conversation Topics | #C |

| data/modCompat/naturesBounty.json | Notes |
| ------------- | ------------- |
| Gift Dialogue | #T |
| Generic Dialogue | #C |
| Schedule Dialogue | #T |
| Love Letters | WIP |
| Quest Letters | WIP |
| Quests | WIP |
| Event 100 | Does BGM match; Review i18n |
| Event 101 | Does BGM match; Review i18n |