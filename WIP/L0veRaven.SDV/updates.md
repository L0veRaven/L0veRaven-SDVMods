# content.json

## Modder Settings

    "ConfigSchema": {
        //Modder Settings
        //## TODO: Delete on release
            //Index - Shows NPCs with index numbers for sprites and portraits
                "RavenIndex": {
                    "Default": "false",
                    "AllowValues": "true, false",
                    "AllowBlank": false,
                    "Section": "ModderSettings",
                    "Description": null
                },
                "ZaydenIndex": {
                    "Default": "false",
                    "AllowValues": "true, false",
                    "AllowBlank": false,
                    "Section": "ModderSettings",
                    "Description": null
                },
            //Event Excludes: Toggle
                "EventExcludes": {
                    "Default": "None",
                    "AllowBlank": false,
                    "AllowValues": "Raven, Zayden, None",
                    "Section": "ModderSettings",
                    "Description": null
                }
    },

## Halloween Costumes

    "ConfigSchema": {
        "RavenCactusCostumeSE": {
            "Default": "false",
            "AllowBlank": false,
            "AllowValues": "true, false",
            "Section": "RavenSpiritsEveCostumes",
            "Description": null
        },
        "RavenDaisyCostumeSE": {
            "Default": "false",
            "AllowBlank": false,
            "AllowValues": "true, false",
            "Section": "RavenSpiritsEveCostumes",
            "Description": null
        },
        "RavenSunflowerCostumeSE": {
            "Default": "false",
            "AllowBlank": false,
            "Section": "RavenSpiritsEveCostumes",
            "AllowValues": "true, false",
            "Description": null
        },
        "RavenWeedCostumeSE": {
            "Default": "false",
            "AllowBlank": false,
            "Section": "RavenSpiritsEveCostumes",
            "AllowValues": "true, false",
            "Description": null
        },
    }

## Clean Language

    "ConfigSchema": {
        "CleanLanguage": {
            "Default": "false",
            "AllowValues": "true, false",
            "AllowBlank": false,
            "Section": "GeneralSettings",
            "Description": null
        },
    }

## DynamicTokens

### ModCompat

    "DynamicTokens": [
        {"Name": "NB","Value": "Raspb3rryfields.NaturesBounty"},
        {"Name": "DTZ","Value": "DTZ.DowntownZuzuDLL"},
        {"Name": "PTP","Value": "LenneDalben.PelicanTownPotluck"},
        {"Name": "SWS","Value": "Airyn.CPSolsticeWinterStar"},
        {"Name": "FF","Value": "violetlizabet.CP.FireworksFestival"},
    ]

    //Mod Compat: Nature's Bounty
        //Town
            {"Name": "RavenRelaxBushTown","Value": "{{Random:Town 47 77 2,Town 47 77 2 {{RavenLC}}_blunt,Town 47 77 2 {{RavenLC}}_edible}}",
                "When": {"HasMod |contains={{SVE}}": "false","HasMod |contains={{NB}}": "true"}},
            {"Name": "RavenRelaxBushTown","Value": "{{Random:Town 47 77 2,Town 47 77 2 {{RavenLC}}_blunt,Town 47 77 2 {{RavenLC}}_edible}}",
                "When": {"HasMod |contains={{SVE}}": "true","HasMod |contains={{NB}}": "true"}},

### Animation Names

    //Raven
        {"Name": "Raven_Animation_Sweep","Value": "l0veraven_raven_sweep"},
        {"Name": "Raven_Animation_Stand","Value": "l0veraven_raven_stand"},
    //Zayden
        {"Name": "Zayden_Animation_Sweep","Value": "l0veraven_zayden_sweep"},
        {"Name": "Zayden_Animation_Sleep","Value": "l0veraven_zayden_sleep"},

### Dialogue Tokens
    //Medication Pickup
        {"Name": "RavenMedicationPickupDialogue","Value": "{{i18n:dialogue.raven.medicationPickup.dayOf}}","When": {"Query: '{{Season}}' = 'Winter'": false}},
        {"Name": "RavenMedicationPickupDialogue","Value": "{{i18n:dialogue.raven.medicationPickup.dayOf_birthday}}","When": {"Query: '{{Season}}' = 'Winter'": true}},

### Custom Locations (SVE)
    {"Name": "RavenTentInside","Value": "Custom_L0veRaven_RavenTentInsideSVE","When": {"HasMod |contains={{SVE}}": "true"}},

### Make a complex schedule system for Raven
    //Vanilla
        //Bus Stop
        {"Name": "Raven_Animation_StandBusStop","Value": "BusStop 20 22 2"},

        {"Name": "RavenRelaxForest","Value": "Forest 56 81 3","When": {"HasMod |contains={{SVE}}": "false","HasMod |contains={{NB}}": "false"}},
        {"Name": "Raven_Animation_StandRiverForest","Value": "Forest 39 75 3","When": {"HasMod |contains={{SVE}}": "false","HasMod |contains={{NB}}": "false"}},

    //Stardew Valley Expanded
        {"Name": "RavenRelaxForest","Value": "Forest 90 89 3","When": {"HasMod |contains={{SVE}}": "true","HasMod |contains={{NB}}": "false"}},
        {"Name": "Raven_Animation_StandRiverForest","Value": "Forest 64 89 3","When": {"HasMod |contains={{SVE}}": "true","HasMod |contains={{NB}}": "false"}},

    //Nature's Bounty
        {"Name": "RavenRelaxForest","Value": "{{Random:Forest 56 81 3,Forest 56 81 3 {{RavenLC}}_blunt,Forest 56 81 3 {{RavenLC}}_edible}}","When": {"HasMod |contains={{SVE}}": "false","HasMod |contains={{NB}}": "true"}},
        {"Name": "RavenRelaxForest","Value": "{{Random:Forest 90 89 3,Forest 90 89 3 {{RavenLC}}_blunt,Forest 90 89 3 {{RavenLC}}_edible}}","When": {"HasMod |contains={{SVE}}": "true","HasMod |contains={{NB}}": "true"}},
        
        {"Name": "Raven_Animation_StandRiverForest","Value": "{{Random:Forest 39 75 3,Forest 39 75 3 {{RavenLC}}_blunt,Forest 39 75 3 {{RavenLC}}_edible}}","When": {"HasMod |contains={{SVE}}": "false","HasMod |contains={{NB}}": "true"}},
        {"Name": "Raven_Animation_StandRiverForest","Value": "{{Random:Forest 64 89 3,Forest 64 89 3 {{RavenLC}}_blunt,Forest 64 89 3 {{RavenLC}}_edible}}","When": {"HasMod |contains={{SVE}}": "true","HasMod |contains={{NB}}": "true"}},

    //Schedule Randomizers
        //Clinic Day
            {"Name": "RavenGoToClinic","Value": "{{610am}} {{Raven_Animation_StandMeds}}"},
            {"Name": "RavenPostClinic","Value": "{{Random:{{Raven_Animation_StandMountain}},{{RavenRelaxBeach}},{{Raven_Animation_StandBookcase}},{{Raven_Animation_StandCC}}}}"},
        //Morning/Night
            {"Name": "RavenGoodMorning","Value": "{{610am}} {{Raven_Animation_StandStove}}"},
            {"Name": "RavenGoodMorningBus","Value": "{{610am}} {{Raven_Animation_StandBusStop}}"},
            {"Name": "RavenGoodNight","Value": "{{10pm}} {{Raven_Animation_StandStove}}/{{130am}} {{RavenInBed}}"},
        //Job Schedules (Arrive at 9:50 from Tent)
            {"Name": "Raven_Animation_StandNearHome","Value": "{{Raven_Animation_StandMountain}}","When": {"HasReadLetter": "{{Raven}}_Apartment"}},
            {"Name": "Raven_Animation_StandNearHome","Value": "{{Random:{{RavenRelaxForest}},{{Raven_Animation_StandRiverForest}}}}","When": {"HasFlag: |contains={{Raven}}_Apartment": false}},
        //Free Days
            {"Name": "RavenFreeDay1","Value": "{{RavenGoodMorning}}/{{7am}} {{Raven_Animation_StandRiverForest}}/{{1130am}} {{RavenRelaxBeach}} {{Raven_Animation_Read}}/{{6pm}} {{Raven_Animation_StandStove}}/{{10pm}} {{RavenInBed}}"},
            {"Name": "RavenFreeDay2","Value": "{{RavenGoodMorning}}/{{7am}} {{RavenRelaxBushTown}}/{{1130am}} {{Raven_Animation_StandTableSaloon}}/{{6pm}} {{Raven_Animation_StandStove}}/{{10pm}} {{RavenInBed}}"},
            {"Name": "RavenFreeDay3","Value": "{{2pm}} {{Raven_Animation_StandStove}}/{{4pm}} {{RavenRelaxBushTown}}/{{8pm}} {{RavenRelaxBeach}}/{{10pm}} {{RavenInBed}}"},
            {"Name": "RavenFreeDay4","Value": "{{4pm}} {{Raven_Animation_StandTableSaloon}}/{{8pm}} {{Raven_Animation_StandCC}}/{{10pm}} {{RavenInBed}}"},

            {"Name": "RavenFreeDays","Value": "{{Random:{{RavenFreeDay1}},{{RavenFreeDay2}},{{RavenFreeDay3}},{{RavenFreeDay4}}}}"},
            {"Name": "RavenFreeDay","Value": "{{RavenFreeDays}}"},//USE THIS COMMAND
        //Free Day - Shopping
            {"Name": "RavenFreeDayShop1","Value": "{{7am}} {{Raven_Animation_StandRiverForest}}/{{11am}} {{RavenShoppingSS}}/{{1pm}} {{Raven_Animation_StandMountain}}/{{5pm}} {{RavenRelaxForest}}/{{9pm}} {{Raven_Animation_StandStove}}/{{12am}} {{RavenInBed}}"},
            {"Name": "RavenFreeDayShop2","Value": "{{7am}} {{Raven_Animation_StandCC}}/{{11am}} {{RavenShoppingSS}}/{{1pm}} {{Raven_Animation_StandBusStop}}/{{5pm}} {{RavenRelaxBushTown}}/{{9pm}} {{Raven_Animation_StandStove}}/{{12am}} {{RavenInBed}}"},
            {"Name": "RavenFreeDayShopRandom","Value": "{{Random:{{RavenFreeDayShop1}},{{RavenFreeDayShop2}}}}"},
            {"Name": "RavenFreeDayShop","Value": "{{RavenFreeDayShopRandom}}"},
        //Job Randomizers
            {"Name": "RavenJobTasksSaloon","Value": "{{7am}} {{Raven_Animation_SweepJobSaloon1}}/{{1250pm}} {{Raven_Animation_SweepJobSaloon2}}/{{350pm}} {{Raven_Animation_SweepJobSaloon3}}"},
            {"Name": "RavenJobTasksSaloon_married","Value": "{{8am}} {{Raven_Animation_SweepJobSaloon1}}/{{1250pm}} {{Raven_Animation_SweepJobSaloon2}}/{{350pm}} {{Raven_Animation_SweepJobSaloon3}}"},
            {"Name": "RavenPostJobSaloon","Value": "{{6pm}} {{Random:{{Raven_Animation_StandNearHome}},{{RavenRelaxBeach}},{{Raven_Animation_StandBusStop}},{{Raven_Animation_StandCC}}}}"},
        //Work and Meds
            {"Name": "RavenWorkDay","Value": "{{RavenGoodMorning}}/{{RavenJobTasksSaloon}}/{{RavenPostJobSaloon}}/{{RavenGoodNight}}"},
            {"Name": "RavenMedsDay","Value": "{{RavenGoToClinic}}/{{10am}} {{RavenPostClinic}}/{{RavenGoodNight}}"},

    //Positions
        //Custom_L0veRaven_RavenTentInside
            {"Name": "Raven_Animation_StandStove","Value": "{{RavenTentInside}} 3 2 0 \"Strings\\schedules\\{{Raven}}:Custom_L0veRaven_RavenTentInside.001\"","When": {"HasMod |contains={{SVE}}": "false","HasFlag: |contains={{Raven}}_Apartment": false}},
            {"Name": "RavenInBed","Value": "{{RavenTentInside}} 3 4 1 l0veraven_raven_sleep"},
        //FRL_NPCApt_Floor1
            {"Name": "Raven_Animation_StandStove","Value": "FRL_NPCApt_Floor1 13 13 0 \"Strings\\schedules\\L0veRaven_Raven:Custom_L0veRaven_RavenTentInside.001\"",
                "When": {"HasReadLetter": "{{Raven}}_Apartment"}},
            {"Name": "RavenInBed","Value": "FRL_NPCApt_Floor1 7 13 0 l0veraven_raven_sleep",
                "When": {"HasReadLetter": "{{Raven}}_Apartment"}},
        //Town
            {"Name": "Raven_Animation_StandCC","Value": "Town 60 17 2"},

            {"Name": "RavenRelaxBushTown","Value": "Town 47 77 2",
                "When": {"HasMod |contains={{NB}}": "false"}},
            {"Name": "RavenRelaxBushTown","Value": "{{Random:Town 47 77 2,Town 47 77 2 {{RavenLC}}_blunt,Town 47 77 2 {{RavenLC}}_edible}}",
                "When": {"HasMod |contains={{NB}}": "true"}},
        //Hospital
            {"Name": "Raven_Animation_StandMeds","Value": "Hospital 5 17 0"},
        //SeedShop
            {"Name": "RavenShoppingSS","Value": "SeedShop 16 28 3 \"Strings\\schedules\\{{Raven}}:SeedShop.001\""},
        //Saloon
            {"Name": "Raven_Animation_SweepJobSaloon1","Value": "Saloon 5 17 2 {{Raven_Animation_Sweep}} \"Strings\\schedules\\{{Raven}}:Saloon.002\""},
            {"Name": "Raven_Animation_SweepJobSaloon2","Value": "Saloon 23 22 2 {{Raven_Animation_Sweep}} \"Strings\\schedules\\{{Raven}}:Saloon.002\""},
            {"Name": "Raven_Animation_SweepJobSaloon3","Value": "Saloon 33 8 2 {{Raven_Animation_Sweep}} \"Strings\\schedules\\{{Raven}}:Saloon.002\""},
            {"Name": "Raven_Animation_StandTableSaloon","Value": "Saloon 43 22 2"},
        //ArchaeologyHouse
            {"Name": "Raven_Animation_StandBookcase","Value": "ArchaeologyHouse 8 13 1",
                "When": {"HasMod |contains={{SVE}}": "false"}},
            {"Name": "Raven_Animation_StandBookcase","Value": "ArchaeologyHouse 7 18 3",
                "When": {"HasMod |contains={{SVE}}": "true"}},
        //Beach
            {"Name": "RavenRelaxBeach","Value": "Beach 43 23 2"},
        //Mountain
            {"Name": "Raven_Animation_StandMountain","Value": "Mountain 57 33 1"},

### Make a complex schedule system for Zayden
    //Animations
        {"Name": "Zayden_ScheduleDialogue_JojaSweep","Value": "\"Strings\\schedules\\{{Zayden}}:JojaMart.001\""},

    //Schedule
        {
            "Name": "Zayden_Schedule_JojaSweep_1",
            "Value": "JojaMart 3 7 2 {{Zayden_Animation_Sweep}} {{Zayden_ScheduleDialogue_JojaSweep}}"
        },
        {
            "Name": "Zayden_Schedule_JojaSweep_2",
            "Value": "JojaMart 1 21 2 {{Zayden_Animation_Sweep}} {{Zayden_ScheduleDialogue_JojaSweep}}"
        },
        {
            "Name": "Zayden_Schedule_JojaSweep_3",
            "Value": "JojaMart 5 15 2 {{Zayden_Animation_Sweep}} {{Zayden_ScheduleDialogue_JojaSweep}}"
        },
        {
            "Name": "Zayden_Schedule_JojaSweep_4",
            "Value": "JojaMart 10 12 2 {{Zayden_Animation_Sweep}} {{Zayden_ScheduleDialogue_JojaSweep}}"
        },
        {
            "Name": "Zayden_Schedule_JojaSweep_5",
            "Value": "JojaMart 13 15 2 {{Zayden_Animation_Sweep}} {{Zayden_ScheduleDialogue_JojaSweep}}"
        },
        {
            "Name": "Zayden_Schedule_JojaSweep_6",
            "Value": "JojaMart 16 25 2 {{Zayden_Animation_Sweep}} {{Zayden_ScheduleDialogue_JojaSweep}}"
        },
        {
            "Name": "Zayden_Schedule_JojaSweep_7",
            "Value": "JojaMart 18 16 2 {{Zayden_Animation_Sweep}} {{Zayden_ScheduleDialogue_JojaSweep}}"
        },
        {
            "Name": "Zayden_Schedule_JojaSweep_8",
            "Value": "JojaMart 21 15 2 {{Zayden_Animation_Sweep}} {{Zayden_ScheduleDialogue_JojaSweep}}"
        },
        {
            "Name": "Zayden_Schedule_JojaSweep_9",
            "Value": "JojaMart 22 12 2 {{Zayden_Animation_Sweep}} {{Zayden_ScheduleDialogue_JojaSweep}}"
        },
        {
            "Name": "Zayden_Schedule_JojaSweep_10",
            "Value": "JojaMart 26 6 2 {{Zayden_Animation_Sweep}} {{Zayden_ScheduleDialogue_JojaSweep}}"
        }

# data/locations/apartment.json
    //Zayden
        {
            "LogName": "[StringsFromMaps] - Zayden's Apartment",
            "Action": "EditData",
            "Target": "Strings/StringsFromMaps",
            "Entries": {
                "L0veRavenZaydenApartment.1": "{{i18n:mapString.fridge}}"
            }
        },
        {
            "LogName": "[Map] - Patch Zayden's Apartment",
            "Action": "EditMap",
            "Target": "Maps/FRL_NPCApt_Floor1",
            "FromFile": "data/maps/{{Zayden}}Apartment.tmx",
            "PatchMode": "Replace",
            "ToArea": {
                "X": 49, "Y": 27, "Width": 11, "Height": 11
            },
            "When": {
                "HasMod |contains={{NPCA}}": "true"
            }
        },