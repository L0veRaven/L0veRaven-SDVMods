# Manifest.json

For further clarification, check out [the Content Patcher documentation for more](https://github.com/Pathoschild/StardewMods/blob/develop/ContentPatcher/docs/author-guide.md) or join the [Stardew Valley Discord](https://discord.com/invite/StardewValley) to get additional modding advice.

Start your `manifest.json` with `{ }` and put all the code you're adding in between.

## Breakdown
`Name`: The mod's name (used in SMAPI and in Generic Mod Config Menu)
```
"Name": "(CP) Raven",
```
`Author`: The author name (can be anything)
```
"Author": "L0veRaven",
```
`Description`: A brief description of the mod (used in SMAPI)
```
"Description": "Adds a neko NPC",
```
`Version`: The current version of your mod. MUST be in the format `#.#.#`.
```
"Version": "1.0.0",
```
`DeleteOldVersion`: `true` or `false`, only used for Stardop compatability (OPTIONAL)
```
"DeleteOldVersion": true,
```
`UniqueID`: `<Author>.<ModName>` is the layout. Put your author name in `<Author>` without the `<>` and you can put what you want for the `<ModName>` without the `<>`.
```
"UniqueID": "L0veRaven.Raven",
```
`UpdateKeys`: (OPTIONAL) This is what SMAPI uses to check for updates on various platforms. Currently supported platforms are Nexus, ModDrop, Github, Chucklefish, and CurseForge. See [this page](https://stardewvalleywiki.com/Modding:Modder_Guide/APIs/Update_checks#Valid_sites) for more details on how to follow the proper syntax.
```
"UpdateKeys": ["Nexus:27407"],
```
`ContentPackFor`: (OPTIONAL) If your mod uses Content Patcher, ADD IT IN THERE. You'll have all kinds of errors if you don't. This is where DLL references go if your mod also uses C#.
```
"ContentPackFor": {
    "UniqueID": "Pathoschild.ContentPatcher",
},
```
`Dependencies`: (OPTIONAL) If your mod relies on another one to function, go ahead and pop it here! I put many of what I added as false so the code knows to still reference the mods if the player does have them installed.

`UniqueID` requires the Mod ID of the mod being referenced.
`IsRequired` tells SMAPI to not load your mod if the referenced mod isn't installed.
```
"Dependencies": [
    {
        "UniqueID": "Airyn.CPSolsticeWinterStar",
        "IsRequired": "false"
    },
    {
        "UniqueID": "CJBok.CheatsMenu",
        "IsRequired": "false"
    },
    {
        "UniqueID": "DTZ.DowntownZuzuDLL",
        "IsRequired": "false"
    },
    {
        "UniqueID": "FireRedLily.NPCApartments",
        "IsRequired": "true"
    },
    {
        "UniqueID": "FlashShifter.StardewValleyExpandedCP",
        "IsRequired": "false"
    },
    {
        "UniqueID": "L0veRaven.CoreCP",
        "IsRequired": "true"
    },
    {
        "UniqueID": "LenneDalben.PelicanTownPotluck",
        "IsRequired": "false"
    },
    {
        "UniqueID": "Rafseazz.RSVCP",
        "IsRequired": "false"
    },
    {
        "UniqueID": "Raspb3rryfields.NaturesBounty",
        "IsRequired": "false"
    },
    {
        "UniqueID": "spacechase0.SpaceCore",
        "IsRequired": "true"
    },
    {
        "UniqueID": "violetlizabet.CP.FireworksFestival",
        "IsRequired": "false"
    }
]
```