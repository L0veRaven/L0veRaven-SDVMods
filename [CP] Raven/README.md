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

| content.json | Notes |
| ------------- | ------------- |
| {{CleanLanguage}} | i18n #NS (all keys prefixed with "clean_") |
| {{RavenIndex}} | Delete when mod is done |

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