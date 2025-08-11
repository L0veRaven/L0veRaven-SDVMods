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