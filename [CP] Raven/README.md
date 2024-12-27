# [CP] Raven
A neko lives in a tent in Cindersap Forest, hoping to save up enough money to have a home again.

## Keys

| Key | Meaning |
| ------------- | ------------- |
| //portraitBookmark | Assign portraits (i18n only) |
| //ADD | Find referenced code and remove flag once added |
| //review | Check if code is worth keeping |
| //DELETE | Delete when it's confirmed it won't break the mod |

## File Directory

GENERAL - FOCUS ON VANILLA MECHANICS FIRST


| File & Focus | Notes |
| ------------- | ------------- |
| data/maps/L0veRaven.Raven_TentInside.tmx | Colors are too intense in-game; Fix layers |
| data/outfits.json: Spirit's Eve Costumes - Vampire | Not started |
| data/animationFrames.json | Create animations/poses -> _beach_towel, _beach_dance, _beach_drink, _beach_umbrella, _handheld_game, _gardening, _sweep, _drink, _sing, _laugh, _sit, _read, _jump, _fishing |
| data/festivals.json | Test festivals |
| data/mail.json: {{ModId}}_marriageTalk_1 | Add letter content |
| data/mail.json: {{ModId}}_marriageTalk_2 | Add letter content |
| data/mail.json: {{ModId}}_marriageTalk_3 | Add letter content |
| i18n/default.json | "addDialogue"; "//portraitBookmark" -> Assign portraits; "//ADD" -> Find referenced code and remove flag once added; "//review" -> Keep in code(?); "//DELETE" -> Delete when it's confirmed it won't break the mod |
| data/dialogue/dialogue.json | //ADD -> Conversation Topics: Custom |
| data/naturesBounty.json: "{{ModId}}_StonerLetter" | WIP |
| modCompat/naturesBounty.json: Event 100 | Does BGM match; Review i18n |
| modCompat/naturesBounty.json: Event 101 | Does BGM match; Review i18n |
| content.json: GMCM {{CleanLanguage}} | WIP; clean i18n not started |
| content.json: GMCM {{RavenIndex}} | Delete when mod is complete |
| content.json: GMCM | Reorganize |
| ___ | ___ |

## Mod Compats

| Festivals | Notes |
| ------------- | ------------- |
| data/modCompat/fireworksFestival.json | Test |
| data/modCompat/pelicanTownPotluck.json | Test |
| data/modCompat/ridgesideVillage.json | Test |
| data/modCompat/solsticeWinterStar.json | Test |


| Conversation Topics | Notes |
| ------------- | ------------- |
| data/modCompat/downtownZuzu.json | Test |
| data/modCompat/naturesBounty.json | Test |

| data/modCompat/naturesBounty.json | Notes |
| ------------- | ------------- |
| {{ModId}}_StonerLetter | WIP |
| Event 100 | Does BGM match; Review i18n |
| Event 101 | Does BGM match; Review i18n |

| data/mail.json | Notes |
| ------------- | ------------- |
| {{ModId}}_marriageTalk_1 | Add letter content |
| {{ModId}}_marriageTalk_2 | Add letter content |
| {{ModId}}_marriageTalk_3 | Add letter content |

| data/events.json | Notes |
| ------------- | ------------- |
| Event 1590166: CatAdoption | Complete |
| Event 0: CatLover | Does end dialogue work correctly; Does BGM match; Check i18n dialogue |
| Event 1: CheckIn | Does BGM match; Check i18n dialogue |
| Event 2: WildClans | Does BGM match; Check i18n dialogue |
| Event 3: CleansingFarmer | Does BGM match; Check i18n dialogue |
| Event 4: CleansingFarmer2 | Does BGM match; Check i18n dialogue |
| Event 5: jobInterview | WIP |
| Event 6: marriageTalk | Test |
| Event 7: ravenApartment | WIP |

| i18n/default.json | Notes |
| ------------- | ------------- |
| "addDialogue" | Remove from code |

| data/dialogue/dialogue.json | Notes |
| ------------- | ------------- |
| Conversation Topics: Custom | //ADD |

| content.json.json | Notes |
| ------------- | ------------- |
| {{CleanLanguage}} | i18n not started (all keys prefixed with "clean_") |
| {{RavenIndex}} | Delete when mod is complete |