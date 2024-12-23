# [CP] Raven
A neko lives in a tent in Cindersap Forest, hoping to save up enough money to have a home again.

TODO:

GENERAL - FOCUS ON VANILLA MECHANICS FIRST

i18n/default.json
    "addDialogue"
    "//portraitBookmark" -> Assign portraits
    "//ADD" -> Find referenced code and remove flag once added
    "//review" -> Keep in code(?)
    "//DELETE" -> Delete when it's confirmed it won't break the mod

data/festivals.json
    Add festival compats

assets/Characters/L0veRaven.Raven png
    //ADD animations
        _beach_towel
        _beach_dance
        _beach_drink
        _beach_umbrella
        _handheld_game
        _gardening
        _sweep
        _drink
        _sing
        _laugh
        _sit
        _read
        _jump
        _fishing

data/maps/z_L0veRaven_Tent png
    Turn tent into a Joja tent

data/dialogue/dialogue.json
    //ADD -> Conversation Topics: Custom

data/events.json
    Event 27407000
        Does end dialogue work correctly
        Does BGM match
        Check i18n dialogue
    Event 27407001
        Does BGM match
        Check i18n dialogue
    Event 27407002
        Does BGM match
        Check i18n dialogue
    Event 27407003 CleansingFarmer
        Does BGM match
        Check i18n dialogue
    Event 27407004 CleansingFarmer2
        Does BGM match
        Check i18n dialogue
    Event 274070## JobInterview
        //Raven wants more hours so they can move back to Zuzu City

modCompat/naturesBounty.json
    Event 27407100 {{NB}} GusEdibles
        Does BGM match
        Check i18n dialogue
    Event 27407101 {{NB}} SmokeSession
        Does BGM match
        Check i18n dialogue

data/quests.json
    //ADD
        "{{ModId}}_StonerLetter"

data/triggerActions.json
    //ADD

data/animationFrames.json
    //Create frames for the animations

data/outfits.json
    Halloweeen Costumes