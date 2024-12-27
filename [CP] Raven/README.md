# [CP] Raven
A neko lives in a tent in Cindersap Forest, hoping to save up enough money to have a home again.

## Keys

| Key | Meaning |
| ------------- | ------------- |
| //portraitBookmark | Assign portraits (i18n only) |
| //ADD | Find referenced code and remove flag once added |
| //review | Check if code is worth keeping |
| //DELETE | Delete when it's confirmed it won't break the mod |
| #T | Test code |
| #C | Don't touch the code |
| #NS | Not Started |
| WIP | Work In Progress |

## File Directory

GENERAL - FOCUS ON VANILLA MECHANICS FIRST


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

| data/maps | Notes |
| ------------- | ------------- |
| L0veRaven_RavenTentInside.tmx | Swap bed and book positions |

| data/outfits.json | Notes |
| ------------- | ------------- |
| Spirit's Eve Costumes - Vampire | #NS |

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
| {{CactusCostumeSE}} | #T |
| {{DaisyCostumeSE}} | #T |
| {{SunflowerCostumeSE}} | #T |
| {{WeedCostumeSE}} | #T |
| {{RavenIndex}} | Delete when mod is done |
| {{EventExcludes}} | Delete when mod is done |

| content.json: CustomLocations | Notes |
| ------------- | ------------- |
| Custom_L0veRaven_RavenTentInside | #C |

| content.json: Changes | Notes |
| ------------- | ------------- |
| Blank Loads | ```Characters/Dialogue/{{ModId}}```, ```Characters/Dialogue/MarriageDialogue{{ModId}}```, ```Characters/schedules/{{ModId}}```, ```Strings/Schedules/{{ModId}}```, ```Data/Events/Custom_L0veRavenRaven_TentInside``` |
| NPC Data | ```data/animationFrames.json```, ```data/concessionTastes.json```, ```data/NPCGiftTastes.json```, ```data/schedule.json```, ```data/events.json```, ```data/festivals.json```, ```data/mail.json```, ```data/character.json```, ```data/outfits.json```, ```data/triggerActions.json``` |
| Dialogue | ```data/dialogue/dialogue.json```, ```data/dialogue/marriageDialogue.json```, ```data/dialogue/giftResponses.json```, ```data/dialogue/moviesReactions.json```, ```data/StringsFromCSFiles.json```, ```data/maps/StringsFromMaps.json```, ```data/dialogue/scheduleDialogue.json``` |
| Spouse Patio | ```data/maps/{{Raven}}SpousePatio.tmx``` |
| Spouse Room | ```data/maps/{{Raven}}SpouseRoom.tmx``` |
| Locations | ```data/locations/WorldMap.json```, ```data/locations/MapPatches.json```, ```data/locations/LocationsData.json``` |
| ModCompat | ```data/modCompat/CJBWarps.json```, ```data/modCompat/naturesBounty.json```, ```data/modCompat/eventExcludesDELETE.json```, ```data/modCompat/downtownZuzu.json```, ```data/modCompat/ridgesideVillage.json```, ```data/modCompat/pelicanTownPotluck.json```, ```data/modCompat/fireworksFestival.json```, ```data/modCompat/solsticeWinterStar.json``` |

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

| Festivals | Notes |
| ------------- | ------------- |
| data/modCompat/fireworksFestival.json | #T |
| data/modCompat/pelicanTownPotluck.json | #T |
| data/modCompat/ridgesideVillage.json | #T |
| data/modCompat/solsticeWinterStar.json | #T |

| Conversation Topics | Notes |
| ------------- | ------------- |
| data/modCompat/downtownZuzu.json | #T |
| data/modCompat/naturesBounty.json | #T |

| data/modCompat/naturesBounty.json | Notes |
| ------------- | ------------- |
| {{ModId}}_StonerLetter | WIP |
| Event 100 | Does BGM match; Review i18n |
| Event 101 | Does BGM match; Review i18n |