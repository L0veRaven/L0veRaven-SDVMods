# content.json

## Add CJB Warps for Cafe stand

## Add Cafe stand to map

## Add snow to Cafe stand for snow patch

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

### Schedule ModCompat

    //Nature's Bounty
        {"Name": "RavenRelaxForest","Value": "{{Random:Forest 56 81 3,Forest 56 81 3 {{RavenLC}}_blunt,Forest 56 81 3 {{RavenLC}}_edible}}","When": {"HasMod |contains={{SVE}}": "false","HasMod |contains={{NB}}": "true"}},
        {"Name": "RavenRelaxForest","Value": "{{Random:Forest 90 89 3,Forest 90 89 3 {{RavenLC}}_blunt,Forest 90 89 3 {{RavenLC}}_edible}}","When": {"HasMod |contains={{SVE}}": "true","HasMod |contains={{NB}}": "true"}},
        
        {"Name": "Raven_Animation_StandRiverForest","Value": "{{Random:Forest 39 75 3,Forest 39 75 3 {{RavenLC}}_blunt,Forest 39 75 3 {{RavenLC}}_edible}}","When": {"HasMod |contains={{SVE}}": "false","HasMod |contains={{NB}}": "true"}},
        {"Name": "Raven_Animation_StandRiverForest","Value": "{{Random:Forest 64 89 3,Forest 64 89 3 {{RavenLC}}_blunt,Forest 64 89 3 {{RavenLC}}_edible}}","When": {"HasMod |contains={{SVE}}": "true","HasMod |contains={{NB}}": "true"}},