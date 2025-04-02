# Content.json

The document starts with `{ }` and all the code will be sandwiched in between.

## Content Patcher: Complete

| Tokens | Values |
| --- | --- |
|`"Format": "2.4.4",` | Current version of Content Patcher |

<details>
    <summary>Expand Code</summary>
    
```
"Format": "2.4.4",
```
</details>

## ConfigSchema: Add

### Formatting: Complete

```
"ConfigSchema": {
    {
        
    },
}
```

The config does not interact with other mods, so all tokens can be written written as desired as long as it doesn't conflict with existing Global Tokens. Here's how the settings are formatted

| Name | Default | AllowValues | AllowBlank | Section | Description |
| --- | --- | --- | --- | --- | --- |
| `<custom value>` | `true`, `false`, `<custom value>` | `true`, `false`, `<custom value>` | `true`, `false` | `<custom_value>` | `<custom string>` |
| Use as token or condition; `{{<custom_value>}}` when used in code | Default setting | Multiple values allowed | Allow the field to be blank | (Optional) Section title | Description displayed when hovering in GMCM settings |

### Raven Settings: Add

| Name | Default | AllowValues | AllowBlank | Section | Description | Meaning |
| --- | --- | --- | --- | --- | --- | --- |
| (ADD) `CleanLanguage` | `false` | `true, false` | `false` | `RavenSettings` | `null` | Raven uses clean language |
| `RavenNude` | `false` | `true, false` | `false` | `RavenSettings` | `null` | Raven goes nude except at festivals |

<details>
    <summary>Expand Code</summary>
    
```
"CleanLanguage": {
    "Default": "false",
    "AllowValues": "true, false",
    "AllowBlank": false,
    "Section": "RavenSettings",
    "Description": null,
},
"RavenNude": {
    "Default": "false",
    "AllowValues": "true, false",
    "AllowBlank": false,
    "Section": "RavenSettings",
    "Description": null,
},
```
</details>

### Spirit's Eve Costumes: Add

| Name | Default | AllowValues | AllowBlank | Section | Description | Meaning |
| --- | --- | --- | --- | --- | --- | --- |
| (ADD) `VampireCostumeSE` | `true` | `true, false` | `false` | `SpiritsEveCostumes` | `null` | Wear vampire costume for Spirit's Eve |
| `RavenCactusCostumeSE` | `false` | `true, false` | `false` | `SpiritsEveCostumes` | `null` | Wear cactus costume for Spirit's Eve |
| `RavenDaisyCostumeSE` | `false` | `true, false` | `false` | `SpiritsEveCostumes` | `null` | Wear daisy costume for Spirit's Eve |
| `RavenSunflowerCostumeSE` | `false` | `true, false` | `false` | `SpiritsEveCostumes` | `null` | Wear sunflower costume for Spirit's Eve |
| `RavenWeedCostumeSE` | `false` | `true, false` | `false` | `SpiritsEveCostumes` | `null` | Wear weed costume for Spirit's Eve |

<details>
    <summary>Expand Code</summary>
    
```
"VampireCostumeSE": {
    "Default": "true",
    "AllowValues": "true, false",
    "AllowBlank": false,
    "Section": "SpiritsEveCostumes",
    "Description": null,
},
"RavenCactusCostumeSE": {
    "Default": "false",
    "AllowValues": "true, false",
    "AllowBlank": false,
    "Section": "SpiritsEveCostumes",
    "Description": null,
},
"RavenDaisyCostumeSE": {
    "Default": "false",
    "AllowValues": "true, false",
    "AllowBlank": false,
    "Section": "SpiritsEveCostumes",
    "Description": null,
},
"RavenSunflowerCostumeSE": {
    "Default": "false",
    "AllowValues": "true, false",
    "AllowBlank": false,
    "Section": "SpiritsEveCostumes",
    "Description": null,
},
"RavenWeedCostumeSE": {
    "Default": "false",
    "AllowValues": "true, false",
    "AllowBlank": false,
    "Section": "SpiritsEveCostumes",
    "Description": null,
},
```
</details>

### Modder Settings: Complete

| Name | Default | AllowValues | AllowBlank | Section | Description | Meaning |
| --- | --- | --- | --- | --- | --- | --- |
| `RavenIndex` | `false` | `true, false` | `false` | `ModderSettings` | `null` | Raven's sprites and portraits show index numbers instead |
| `RavenEventExcludes` | `false` | `true, false` | `false` | `ModderSettings` | `null` | Exclude other NPCs from participating in the Flower Dance and Winter Star |

<details>
    <summary>Expand Code</summary>
    
```
"RavenIndex": {
    "Default": "false",
    "AllowValues": "true, false",
    "AllowBlank": false,
    "Section": "ModderSettings",
    "Description": null,
},
"RavenEventExcludes": {
    "Default": "false",
    "AllowValues": "true, false",
    "AllowBlank": false,
    "Section": "ModderSettings",
    "Description": null,
},
```
</details>

## DynamicTokens: WIP

Think of DynamicTokens as ZIP file names, and when the game reads the code, the file is "unzipped" and all the data goes into the code as if it were already written there. This is very handy for using as a shortcut for repetitive code.

In my code, I use Dynamic Tokens as a shortcut for repetitive code and to perform complex randomization for dialogues and schedules.

```
"Dynamic Tokens": [
    {
        
    }
]
```
### Basic Information: Complete

| Name | Value | Meaning |
| --- | --- | --- |
|`"Raven"` | `"L0veRaven_Raven"` | Raven's internal name |
|`"displayName"` | `"{{i18n:displayName.Raven}}"` | Toggle Raven's sprites and portraits to display only their index number |
|`"Nexus"` | `"27407"` | Nexus ID |

<details>
    <summary>Expand Code</summary>
    
```
{
    "Name": "Raven",
    "Value": "L0veRaven_Raven",
},
{
    "Name": "displayName",
    "Value": "{{i18n:displayName.Raven}}",
},
{
    "Name": "Nexus",
    "Value": "27407",
},
```
</details>

### Mod Compat Nicknames: Complete

| Name | Value | Meaning |
| --- | --- | --- |
|`NPCA` | `FireRedLily.NPCApartments` | FireRedLily's Pelican Valley Loft: NPC Apartments |
|`NB` | `Raspb3rryfields.NaturesBounty` | Nature's Bounty |
|`DTZ` | `DTZ.DowntownZuzuDLL` | Downtown Zuzu |
|`PTP` | `LenneDalben.PelicanTownPotluck` | Pelican Town Potluck |
|`SVE` | `FlashShifter.StardewValleyExpandedCP` | Stardew Valley Expanded |
|`SWS` | `Airyn.CPSolsticeWinterStar` | Solstice Winter Star |
|`FF` | `violetlizabet.CP.FireworksFestival` | Fireworks Festival |

<details>
    <summary>Expand Code</summary>
    
```
{
    "Name": "NPCA",
    "Value": "FireRedLily.NPCApartments",
},
{
    "Name": "NB",
    "Value": "Raspb3rryfields.NaturesBounty",
},
{
    "Name": "DTZ",
    "Value": "DTZ.DowntownZuzuDLL",
},
{
    "Name": "PTP",
    "Value": "LenneDalben.PelicanTownPotluck",
},
{
    "Name": "SVE",
    "Value": "FlashShifter.StardewValleyExpandedCP",
},
{
    "Name": "SWS",
    "Value": "Airyn.CPSolsticeWinterStar",
},
{
    "Name": "FF",
    "Value": "violetlizabet.CP.FireworksFestival",
},
```
</details>

### Directions: Complete

| Name | Value |
| --- | --- |
| `up` | `0` |
| `right` | `1` |
| `down` | `2` |
| `left` | `3` |

<details>
    <summary>Expand Code</summary>
    
```
{
    "Name": "up",
    "Value": "0",
},
{
    "Name": "right",
    "Value": "1",
},
{
    "Name": "down",
    "Value": "2",
},
{
    "Name": "left",
    "Value": "3",
},
```
</details>

### Emotes: Complete

The `Name` corresponds with the emote I want to use. Rather than me memorizing the index numbers for each emote, I use a naming convention that easily matches what I want.

| Name | Value | Meaning |
| --- | --- | --- |
|`emoteEmptyCan` |  `4` | Empty Watering Can |
|`emoteQuestion` | `8` | Question Mark |
|`emoteAngry` | `12` | Angry |
|`emoteExclaim` | `16` | Exclaim |
|`emoteHeart` | `20` | Heart |
|`emoteSleep` | `24` | Sleepy / Tired |
|`emoteSweat` | `28` | Sweatdrop |
|`emoteHappy` | `32` | Happy |
|`emoteX` | `36` | X |
|`emotePause` | `40` | Pause / Silence |
|`emoteVideoGame` | `52` | Video Game Controller |
|`emoteMusic` | `56` | Music Note |
|`emoteBlush` | `60` | Blush |

<details>
    <summary>Expand Code</summary>
    
```
{
    "Name": "emoteEmptyCan",
    "Value": "4",
},
{
    "Name": "emoteQuestion",
    "Value": "8",
},
{
    "Name": "emoteAngry",
    "Value": "12",
},
{
    "Name": "emoteExclaim",
    "Value": "16",
},
{
    "Name": "emoteHeart",
    "Value": "20",
},
{
    "Name": "emoteSleep",
    "Value": "24",
},
{
    "Name": "emoteSweat",
    "Value": "28",
},
{
    "Name": "emoteHappy",
    "Value": "32",
},
{
    "Name": "emoteX",
    "Value": "36",
},
{
    "Name": "emotePause",
    "Value": "40",
},
{
    "Name": "emoteVideoGame",
    "Value": "52",
},
{
    "Name": "emoteMusic",
    "Value": "56",
},
{
    "Name": "emoteBlush",
    "Value": "60",
},
```
</details>

### Time: Complete

6am

<details>
<summary>Expand Code</summary>
 
| Name | Value |
| --- | --- |
| `6am` | `600` |
| `610am` | `610` |
| `620am` | `620` |
| `630am` | `630` |
| `640am` | `640` |
| `650am` | `650` |

```
{
    "Name": "6am",
    "Value": "600",
},
{
    "Name": "610am",
    "Value": "610",
},
{
    "Name": "620am",
    "Value": "620",
},
{
    "Name": "630am",
    "Value": "630",
},
{
    "Name": "640am",
    "Value": "640",
},
{
    "Name": "650am",
    "Value": "650",
},
```
</details>

7am
<details>
<summary>Expand Code</summary>
 
| Name | Value |
| --- | --- |
| `7am` | `700` |
| `710am` | `710` |
| `720am` | `720` |
| `730am` | `730` |
| `740am` | `740` |
| `750am` | `750` |

```
{
    "Name": "7am",
    "Value": "700",
},
{
    "Name": "710am",
    "Value": "710",
},
{
    "Name": "720am",
    "Value": "720",
},
{
    "Name": "730am",
    "Value": "730",
},
{
    "Name": "740am",
    "Value": "740",
},
{
    "Name": "750am",
    "Value": "750",
},
```
</details>

8am
<details>
<summary>Expand Code</summary>
 
| Name | Value |
| --- | --- |
| `8am` | `800` |
| `810am` | `810` |
| `820am` | `820` |
| `830am` | `830` |
| `840am` | `840` |
| `850am` | `850` |

```
{
    "Name": "8am",
    "Value": "800",
},
{
    "Name": "810am",
    "Value": "810",
},
{
    "Name": "820am",
    "Value": "820",
},
{
    "Name": "830am",
    "Value": "830",
},
{
    "Name": "840am",
    "Value": "840",
},
{
    "Name": "850am",
    "Value": "850",
},
```
</details>

9am
<details>
<summary>Expand Code</summary>
 
| Name | Value |
| --- | --- |
| `9am` | `900` |
| `910am` | `910` |
| `920am` | `920` |
| `930am` | `930` |
| `940am` | `940` |
| `950am` | `950` |

```
{
    "Name": "9am",
    "Value": "900",
},
{
    "Name": "910am",
    "Value": "910",
},
{
    "Name": "920am",
    "Value": "920",
},
{
    "Name": "930am",
    "Value": "930",
},
{
    "Name": "940am",
    "Value": "940",
},
{
    "Name": "950am",
    "Value": "950",
},
```
</details>

10am
<details>
<summary>Expand Code</summary>
 
| Name | Value |
| --- | --- |
| `10am` | `1000` |
| `1010am` | `1010` |
| `1020am` | `1020` |
| `1030am` | `1030` |
| `1040am` | `1040` |
| `1050am` | `1050` |

```
{
    "Name": "10am",
    "Value": "1000",
},
{
    "Name": "1010am",
    "Value": "1010",
},
{
    "Name": "1020am",
    "Value": "1020",
},
{
    "Name": "1030am",
    "Value": "1030",
},
{
    "Name": "1040am",
    "Value": "1040",
},
{
    "Name": "1050am",
    "Value": "1050",
},
```
</details>

11am
<details>
<summary>Expand Code</summary>

| Name | Value |
| --- | --- |
| `11am` | `1100` |
| `1110am` | `1110` |
| `1120am` | `1120` |
| `1130am` | `1130` |
| `1140am` | `1140` |
| `1150am` | `1150` |

```
{
    "Name": "11am",
    "Value": "1100",
},
{
    "Name": "1110am",
    "Value": "1110",
},
{
    "Name": "1120am",
    "Value": "1120",
},
{
    "Name": "1130am",
    "Value": "1130",
},
{
    "Name": "1140am",
    "Value": "1140",
},
{
    "Name": "1150am",
    "Value": "1150",
},
```
</details>

12pm
<details>
<summary>Expand Code</summary>

| Name | Value |
| --- | --- |
| `12pm` | `1200` |
| `1210pm` | `1210` |
| `1220pm` | `1220` |
| `1230pm` | `1230` |
| `1240pm` | `1240` |
| `1250pm` | `1250` |

```
{
    "Name": "12pm",
    "Value": "1200",
},
{
    "Name": "1210pm",
    "Value": "1210",
},
{
    "Name": "1220pm",
    "Value": "1220",
},
{
    "Name": "1230pm",
    "Value": "1230",
},
{
    "Name": "1240pm",
    "Value": "1240",
},
{
    "Name": "1250pm",
    "Value": "1250",
},
```
</details>

1pm
<details>
<summary>Expand Code</summary>
    
| Name | Value |
| --- | --- |
| `1pm` | `1300` |
| `110pm` | `1310` |
| `120pm` | `1320` |
| `130pm` | `1330` |
| `140pm` | `1340` |
| `150pm` | `1350` |

```
{
    "Name": "1pm",
    "Value": "1300",
},
{
    "Name": "110pm",
    "Value": "1310",
},
{
    "Name": "120pm",
    "Value": "1320",
},
{
    "Name": "130pm",
    "Value": "1330",
},
{
    "Name": "140pm",
    "Value": "1340",
},
{
    "Name": "150pm",
    "Value": "1350",
},
```
</details>

2pm
<details>
<summary>Expand Code</summary>
    
| Name | Value |
| --- | --- |
| `2pm` | `1400` |
| `210pm` | `1410` |
| `220pm` | `1420` |
| `230pm` | `1430` |
| `240pm` | `1440` |
| `250pm` | `1450` |

```
{
    "Name": "2pm",
    "Value": "1400",
},
{
    "Name": "210pm",
    "Value": "1410",
},
{
    "Name": "220pm",
    "Value": "1420",
},
{
    "Name": "230pm",
    "Value": "1430",
},
{
    "Name": "240pm",
    "Value": "1440",
},
{
    "Name": "250pm",
    "Value": "1450",
},
```
</details>

3pm
<details>
<summary>Expand Code</summary>
    
| Name | Value |
| --- | --- |
| `3pm` | `1500` |
| `310pm` | `1510` |
| `320pm` | `1520` |
| `330pm` | `1530` |
| `340pm` | `1540` |
| `350pm` | `1550` |

```
{
    "Name": "3pm",
    "Value": "1500",
},
{
    "Name": "310pm",
    "Value": "1510",
},
{
    "Name": "320pm",
    "Value": "1520",
},
{
    "Name": "330pm",
    "Value": "1530",
},
{
    "Name": "340pm",
    "Value": "1540",
},
{
    "Name": "350pm",
    "Value": "1550",
},
```
</details>

4pm
<details>
<summary>Expand Code</summary>
    
| Name | Value |
| --- | --- |
| `4pm` | `1600` |
| `410pm` | `1610` |
| `420pm` | `1620` |
| `430pm` | `1630` |
| `440pm` | `1640` |
| `450pm` | `1650` |

```
{
    "Name": "4pm",
    "Value": "1600",
},
{
    "Name": "410pm",
    "Value": "1610",
},
{
    "Name": "420pm",
    "Value": "1620",
},
{
    "Name": "430pm",
    "Value": "1630",
},
{
    "Name": "440pm",
    "Value": "1640",
},
{
    "Name": "450pm",
    "Value": "1650",
},
```
</details>

5pm
<details>
<summary>Expand Code</summary>
    
| Name | Value |
| --- | --- |
| `5pm` | `1700` |
| `510pm` | `1710` |
| `520pm` | `1720` |
| `530pm` | `1730` |
| `540pm` | `1740` |
| `550pm` | `1750` |

```
{
    "Name": "5pm",
    "Value": "1700",
},
{
    "Name": "510pm",
    "Value": "1710",
},
{
    "Name": "520pm",
    "Value": "1720",
},
{
    "Name": "530pm",
    "Value": "1730",
},
{
    "Name": "540pm",
    "Value": "1740",
},
{
    "Name": "550pm",
    "Value": "1750",
},
```
</details>

6pm
<details>
<summary>Expand Code</summary>
    
| Name | Value |
| --- | --- |
| `6pm` | `1800` |
| `610pm` | `1810` |
| `620pm` | `1820` |
| `630pm` | `1830` |
| `640pm` | `1840` |
| `650pm` | `1850` |

```
{
    "Name": "6pm",
    "Value": "1800",
},
{
    "Name": "610pm",
    "Value": "1810",
},
{
    "Name": "620pm",
    "Value": "1820",
},
{
    "Name": "630pm",
    "Value": "1830",
},
{
    "Name": "640pm",
    "Value": "1840",
},
{
    "Name": "650pm",
    "Value": "1850",
},
```
</details>

7pm
<details>
<summary>Expand Code</summary>
    
| Name | Value |
| --- | --- |
| `7pm` | `1900` |
| `710pm` | `1910` |
| `720pm` | `1920` |
| `730pm` | `1930` |
| `740pm` | `1940` |
| `750pm` | `1950` |

```
{
    "Name": "7pm",
    "Value": "1900",
},
{
    "Name": "710pm",
    "Value": "1910",
},
{
    "Name": "720pm",
    "Value": "1920",
},
{
    "Name": "730pm",
    "Value": "1930",
},
{
    "Name": "740pm",
    "Value": "1940",
},
{
    "Name": "750pm",
    "Value": "1950",
},
```
</details>

8pm
<details>
<summary>Expand Code</summary>
    
| Name | Value |
| --- | --- |
| `8pm` | `2000` |
| `810pm` | `2010` |
| `820pm` | `2020` |
| `830pm` | `2030` |
| `840pm` | `2040` |
| `850pm` | `2050` |

```
{
    "Name": "8pm",
    "Value": "2000",
},
{
    "Name": "810pm",
    "Value": "2010",
},
{
    "Name": "820pm",
    "Value": "2020",
},
{
    "Name": "830pm",
    "Value": "2030",
},
{
    "Name": "840pm",
    "Value": "2040",
},
{
    "Name": "850pm",
    "Value": "2050",
},
```
</details>

9pm
<details>
<summary>Expand Code</summary>
    
| Name | Value |
| --- | --- |
| `9pm` | `2100` |
| `910pm` | `2110` |
| `920pm` | `2120` |
| `930pm` | `2130` |
| `940pm` | `2140` |
| `950pm` | `2150` |

```
{
    "Name": "9pm",
    "Value": "2100",
},
{
    "Name": "910pm",
    "Value": "2110",
},
{
    "Name": "920pm",
    "Value": "2120",
},
{
    "Name": "930pm",
    "Value": "2130",
},
{
    "Name": "940pm",
    "Value": "2140",
},
{
    "Name": "950pm",
    "Value": "2150",
},
```
</details>

10pm
<details>
<summary>Expand Code</summary>
    
| Name | Value |
| --- | --- |
| `10pm` | `2200` |
| `1010pm` | `2210` |
| `1020pm` | `2220` |
| `1030pm` | `2230` |
| `1040pm` | `2240` |
| `1050pm` | `2250` |

```
{
    "Name": "10pm",
    "Value": "2200",
},
{
    "Name": "1010pm",
    "Value": "2210",
},
{
    "Name": "1020pm",
    "Value": "2220",
},
{
    "Name": "1030pm",
    "Value": "2230",
},
{
    "Name": "1040pm",
    "Value": "2240",
},
{
    "Name": "1050pm",
    "Value": "2250",
},
```
</details>

11pm
<details>
<summary>Expand Code</summary>

| Name | Value |
| --- | --- |
| `11pm` | `2300` |
| `1110pm` | `2310` |
| `1120pm` | `2320` |
| `1130pm` | `2330` |
| `1140pm` | `2340` |
| `1150pm` | `2350` |

```
{
    "Name": "11pm",
    "Value": "2300",
},
{
    "Name": "1110pm",
    "Value": "2310",
},
{
    "Name": "1120pm",
    "Value": "2320",
},
{
    "Name": "1130pm",
    "Value": "2330",
},
{
    "Name": "1140pm",
    "Value": "2340",
},
{
    "Name": "1150pm",
    "Value": "2350",
},
```
</details>

12am
<details>
<summary>Expand Code</summary>

| Name | Value |
| --- | --- |
| `12am` | `2400` |
| `1210am` | `2410` |
| `1220am` | `2420` |
| `1230am` | `2430` |
| `1240am` | `2440` |
| `1250am` | `2450` |

```
{
    "Name": "12am",
    "Value": "2400",
},
{
    "Name": "1210am",
    "Value": "2410",
},
{
    "Name": "1220am",
    "Value": "2420",
},
{
    "Name": "1230am",
    "Value": "2430",
},
{
    "Name": "1240am",
    "Value": "2440",
},
{
    "Name": "1250am",
    "Value": "2450",
},
```
</details>

1am
<details>
<summary>Expand Code</summary>

| Name | Value |
| --- | --- |
| `1am` | `2500` |
| `110am` | `2510` |
| `120am` | `2520` |
| `130am` | `2530` |
| `140am` | `2540` |
| `150am` | `2550` |

```
{
    "Name": "1am",
    "Value": "2500",
},
{
    "Name": "110am",
    "Value": "2510",
},
{
    "Name": "120am",
    "Value": "2520",
},
{
    "Name": "130am",
    "Value": "2530",
},
{
    "Name": "140am",
    "Value": "2540",
},
{
    "Name": "150am",
    "Value": "2550",
},
```
</details>

### Dialogue: WIP

#### First of Season

| Name | Value |
| --- | --- |
| `springFirst` | `{{i18n:dialogue.raven.spring.first_{{Random:{{Range:1,4}}}}}}` |
| `summerFirst` | `{{i18n:dialogue.raven.summer.first_{{Random:{{Range:1,4}}}}}}` |
| `fallFirst` | `{{i18n:dialogue.raven.fall.first_{{Random:{{Range:1,4}}}}}}` |
| `winterFirst` | `{{i18n:dialogue.raven.winter.first_{{Random:{{Range:1,4}}}}}}` |
| `Raven_firstOfSeason` | `{{i18n:dialogue.raven.winter.first_{{Random:{{Range:1,4}}}}}}` |

<details>
    <summary>Expand Code</summary>
    
```
{
    "Name": "springFirst",
    "Value": "{{i18n:dialogue.raven.spring.first_{{Random:{{Range:1,4}}}}}}",
},
{
    "Name": "summerFirst",
    "Value": "{{i18n:dialogue.raven.summer.first_{{Random:{{Range:1,4}}}}}}",
},
{
    "Name": "fallFirst",
    "Value": "{{i18n:dialogue.raven.fall.first_{{Random:{{Range:1,4}}}}}}",
},
{
    "Name": "winterFirst",
    "Value": "{{i18n:dialogue.raven.winter.first_{{Random:{{Range:1,4}}}}}}",
},
{
    "Name": "Raven_firstOfSeason",
    "Value": "{{springFirst}}",
    "When": {
        "Season": "spring",
    }
},
{
    "Name": "Raven_firstOfSeason",
    "Value": "{{summerFirst}}",
    "When": {
        "Season": "summer",
    }
}, 
{
    "Name": "Raven_firstOfSeason",
    "Value": "{{fallFirst}}",
    "When": {
        "Season": "fall",
    }
}, 
{
    "Name": "Raven_firstOfSeason",
    "Value": "{{winterFirst}}",
    "When": {
        "Season": "winter",
    }
},
```
</details>

#### Doctor: Complete

| Name | Value | When |
| --- | --- | --- |
| `medsDialogue` |  `{{i18n:dialogue.raven.medicationPickup.dayOf_{{Random:{{Range:1,2}}}}}}` |  |
| `medsDialogue` | `{{i18n:dialogue.raven.medicationPickup.dayOf_birthday_{{Random:{{Range:1,3}}}}}}` | `"Season": "winter"`, `"Day": "18",` |

<details>
    <summary>Expand Code</summary>
    
```
{
    "Name": "medsDialogue",
    "Value": "{{i18n:dialogue.raven.medicationPickup.dayOf_{{Random:{{Range:1,2}}}}}}",
},
{
    "Name": "medsDialogue",
    "Value": "{{i18n:dialogue.raven.medicationPickup.dayOf_birthday_{{Random:{{Range:1,3}}}}}}",
    "When": {
        "Season": "winter",
        "Day": "18",
    }
},
```
</details>

#### Festivals

Egg Festival

| Name | Value |
| --- | --- |
| --- | --- |

<details>
    <summary>Expand Code</summary>
     
```
{"Name": "Raven_eggFestival_dayBefore","Value": "{{i18n:Raven_eggFestival_dayBefore{{Random:{{Range:1,4}}}}}}",},
{"Name": "Raven_eggFestival_dayOf","Value": "{{i18n:dialogue.raven.eggFestival.dayOf_{{Random:{{Range:1,4}}}}}}",},
{"Name": "Raven_eggFestival_dayAfter","Value": "{{i18n:dialogue.raven.eggFestival.dayAfter_{{Random:{{Range:1,5}}}}}}",},
```
</details>

Flower Dance

| Name | Value |
| --- | --- |
| --- | --- |

<details>
    <summary>Expand Code</summary>
     
```
{"Name": "Raven_flowerDance_dayBefore","Value": "{{i18n:dialogue.raven.flowerDance.dayBefore_{{Random:{{Range:1,4}}}}}}",},
{"Name": "Raven_flowerDance_dayOf","Value": "{{i18n:dialogue.raven.flowerDance.dayOf_{{Random:{{Range:1,3}}}}}}",},
{"Name": "Raven_flowerDance_dayAfter","Value": "{{i18n:dialogue.raven.flowerDance.dayAfter_{{Random:{{Range:1,3}}}}}}",},
{"Name": "flowDanAccept","Value": "{{i18nfestival.raven.flowerDance.accept_{{Random:{{Range:1,3}}}}}}",},
{"Name": "flowDanAcceptSpouse","Value": "{{i18nfestival.raven.flowerDance.spouse.accept_{{Random:{{Range:1,3}}}}}}",},
```
</details>

Luau

| Name | Value |
| --- | --- |
| --- | --- |

<details>
    <summary>Expand Code</summary>
     
```
{"Name": "Raven_luau_dayBefore","Value": "{{i18n:dialogue.raven.luau.dayBefore_{{Random:{{Range:1,3}}}}}}",},
{"Name": "Raven_luau_dayOf","Value": "{{i18n:dialogue.raven.luau.dayOf_{{Random:{{Range:1,3}}}}}}",},
{"Name": "Raven_luau_dayAfter","Value": "{{i18n:dialogue.raven.luau.dayAfter_{{Random:{{Range:1,3}}}}}}",},
```
</details>

Potluck

| Name | Value |
| --- | --- |
| --- | --- |

<details>
    <summary>Expand Code</summary>
     
```
{"Name": "potluckYest","Value": "{{i18n:Raven_luauPotluck_dayBefore_{{Random:{{Range:1,3}}}}}}",},
{"Name": "potluckToday","Value": "{{i18n:potluck_dayOf_{{Random:{{Range:1,3}}}}}}",},
{"Name": "potluckTomo","Value": "{{i18n:potluck_dayAfter_{{Random:{{Range:1,3}}}}}}",},
```
</details>

Dance of the Moonlight Jellies

| Name | Value |
| --- | --- |
| --- | --- |

<details>
    <summary>Expand Code</summary>
     
```
{"Name": "MooJellYest","Value": "{{i18n:dialogue.raven.moonlightJellies.dayBefore_{{Random:{{Range:1,3}}}}}}",},
{"Name": "MooJellToday","Value": "{{i18n:dialogue.raven.moonlightJellies.dayOf_{{Random:{{Range:1,3}}}}}}",},
{"Name": "MooJellTomo","Value": "{{i18n:dialogue.raven.moonlightJellies.dayAfter_{{Random:{{Range:1,3}}}}}}",},
```
</details>

Stardew Valley Fair

| Name | Value |
| --- | --- |
| --- | --- |

<details>
    <summary>Expand Code</summary>
     
```
{"Name": "FairYest","Value": "{{i18n:dialogue.raven.stardewValleyFair.dayBefore_{{Random:{{Range:1,3}}}}}}",},
{"Name": "FairToday","Value": "{{i18n:dialogue.raven.stardewValleyFair.dayOf_{{Random:{{Range:1,3}}}}}}",},
{"Name": "FairTomo","Value": "{{i18n:dialogue.raven.stardewValleyFair.dayAfter_{{Random:{{Range:1,3}}}}}}",},
{"Name": "FairJudging","Value": "{{i18n:festival.raven.stardewValleyFair.judging_{{Random:{{Range:1,3}}}}}}",},
{"Name": "FairJudgeSkip","Value": "{{i18n:festival.raven.stardewValleyFair.judged_Skipped{{Random:{{Range:1,3}}}}}}",},
{"Name": "FairJudgeLost","Value": "{{i18n:festival.raven.stardewValleyFair.judged.playerLost.{{Random:{{Range:1,3}}}}}}",},
{"Name": "FairJudgeWon","Value": "{{i18n:festival.raven.stardewValleyFair.judged.playerWon_{{Random:{{Range:1,3}}}}}}",},
{"Name": "FairJudged","Value": "{{i18n:festival.raven.stardewValleyFair.judged_{{Random:{{Range:1,3}}}}}}",},
```
</details>

Spirit's Eve

| Name | Value |
| --- | --- |
| --- | --- |

<details>
    <summary>Expand Code</summary>
     
```
{"Name": "spiritsEveYest","Value": "{{i18n:dialogue.raven.spiritsEve.dayBefore_{{Random:{{Range:1,3}}}}}}",},
{"Name": "spiritsEveToday","Value": "{{i18n:dialogue.raven.spiritsEve.dayOf_{{Random:{{Range:1,3}}}}}}",},
{"Name": "spiritsEveTomo","Value": "{{i18n:dialogue.raven.spiritsEve.dayAfter_{{Random:{{Range:1,3}}}}}}",},
```
</details>

Ice Festival

| Name | Value |
| --- | --- |
| --- | --- |

<details>
    <summary>Expand Code</summary>
     
```
{"Name": "iceFestYest","Value": "{{i18n:dialogue.raven.festivalOfIce.dayBefore_{{Random:{{Range:1,3}}}}}}",},
{"Name": "iceFestToday","Value": "{{i18n:dialogue.raven.festivalOfIce.dayOf_{{Random:{{Range:1,3}}}}}}",},
{"Name": "iceFestTomo","Value": "{{i18n:dialogue.raven.festivalOfIce.dayAfter_{{Random:{{Range:1,3}}}}}}",},
```
</details>

Feast of the Winter Star

| Name | Value |
| --- | --- |
| --- | --- |

<details>
    <summary>Expand Code</summary>
     
```
{"Name": "winterStarYest","Value": "{{i18n:dialogue.raven.feastOfTheWinterStar.dayBefore_{{Random:{{Range:1,3}}}}}}",},
{"Name": "winterStarToday","Value": "{{i18n:dialogue.raven.feastOfTheWinterStar.dayOf_{{Random:{{Range:1,3}}}}}}",},
{"Name": "winterStarTomo","Value": "{{i18n:dialogue.raven.feastOfTheWinterStar.dayAfter_{{Random:{{Range:1,3}}}}}}",},
{"Name": "winterStarGiftBefore","Value": "{{i18n:festival.raven.winterStar.GiveGift_Before_{{Random:{{Range:1,3}}}}}}",},
{"Name": "winterStarGiftBeforeSpouse","Value": "{{i18n:festival.raven.winterStar.GiveGift_Before_Spouse_{{Random:{{Range:1,3}}}}}}",},
{"Name": "winterStarGiftAfter","Value": "{{i18n:WinterStar_GiveGift_After_{{Random:{{Range:1,3}}}}}}",},
{"Name": "winterStarGiftAfterSpouse","Value": "{{i18n:WinterStar_GiveGift_After_Spouse_{{Random:{{Range:1,3}}}}}}",},
{"Name": "winterStarGiftReceive","Value": "{{i18n:WinterStar_ReceiveGift_{{Random:{{Range:1,3}}}}}}",},
```
</details>


#### Generic Dialogue

| Name | Value |
| --- | --- |
| --- | --- |

<details>
    <summary>Expand Code</summary>

```
//Generic
{"Name": "generic","Value": "{{i18n:dialogue.raven.generic_{{Random:{{Range:1,14}}}}}}",},

{"Name": "genericSpring","Value": "{{i18n:Raven_genericSpring_{{Random:{{Range:1,7}}}}}}",},
{"Name": "genericSummer","Value": "{{i18n:Raven_genericSummer_{{Random:{{Range:1,7}}}}}}",},
{"Name": "genericFall","Value": "{{i18n:Raven_genericFall_{{Random:{{Range:1,7}}}}}}",},
{"Name": "genericWinter","Value": "{{i18n:Raven_genericWinter_{{Random:{{Range:1,7}}}}}}",},

{"Name": "marriedGenSpring","Value": "{{i18n:Raven_married_genericSpring_{{Random:{{Range:1,3}}}}}}",},
{"Name": "marriedGenSummer","Value": "{{i18n:Raven_married_genericSummer_{{Random:{{Range:1,5}}}}}}",},
{"Name": "marriedGenFall","Value": "{{i18n:Raven_married_genericFall_{{Random:{{Range:1,3}}}}}}",},
{"Name": "marriedGenWinter","Value": "{{i18n:Raven_married_genericWinter_{{Random:{{Range:1,5}}}}}}",},
```
</details>


#### Weather

GreenRain

| Name | Value |
| --- | --- |
| --- | --- |

<details>
    <summary>Expand Code</summary>

```
{"Name": "gRain3","Value": "{{i18n:dialogue.raven.greenRain_3{{Random:{{Range:1,10}}}}}}",},
{"Name": "gRain3Fin","Value": "{{i18n:GreenRainFinished_3_{{Random:{{Range:1,10}}}}}}",},
```
</details>


Spring

| Name | Value |
| --- | --- |
| --- | --- |

<details>
    <summary>Expand Code</summary>

```
{"Name": "spRain","Value": "{{i18n:springRain_{{Random:{{Range:1,6}}}}}}",},
{"Name": "spStorm","Value": "{{i18n:springStorm_{{Random:{{Range:1,5}}}}}}",},
{"Name": "spWind","Value": "{{i18n:springWind_{{Random:{{Range:1,3}}}}}}",},
```
</details>

Summer

| Name | Value |
| --- | --- |
| --- | --- |

<details>
    <summary>Expand Code</summary>

```
{"Name": "suRain","Value": "{{i18n:summerRain_{{Random:{{Range:1,4}}}}}}",},
{"Name": "suStorm","Value": "{{i18n:summerStorm_{{Random:{{Range:1,3}}}}}}",},
```
</details>

Fall

| Name | Value |
| --- | --- |
| --- | --- |

<details>
    <summary>Expand Code</summary>

```
{"Name": "faRain","Value": "{{i18n:fallRain_{{Random:{{Range:1,5}}}}}}",},
{"Name": "faStorm","Value": "{{i18n:fallStorm_{{Random:{{Range:1,3}}}}}}",},
{"Name": "faWind","Value": "{{i18n:fallWind_{{Random:{{Range:1,3}}}}}}",},
```
</details>

Winter

| Name | Value |
| --- | --- |
| --- | --- |

<details>
    <summary>Expand Code</summary>

```
{"Name": "wiRain","Value": "{{i18n:winterRain_{{Random:{{Range:1,3}}}}}}",},
{"Name": "snowingD","Value": "{{i18n:Snowing_{{Random:{{Range:1,5}}}}}}",},
```
</details>

Heart Dialogue

| Name | Value |
| --- | --- |
| --- | --- |

<details>
    <summary>Expand Code</summary>

```
{"Name": "0hearts","Value": "{{i18n:dialogue.raven.0hearts_{{Random:{{Range:1,10}}}}}}",},
{"Name": "2hearts","Value": "{{i18n:dialogue.raven.2hearts_{{Random:{{Range:1,8}}}}}}",},
{"Name": "Raven_4hearts","Value": "{{i18n:dialogue.raven.4hearts_{{Random:{{Range:1,5}}}}}}",},
{"Name": "Raven_6hearts","Value": "{{i18n:dialogue.raven.6hearts_{{Random:{{Range:1,10}}}}}}",},
{"Name": "Raven_8hearts","Value": "{{i18n:dialogue.raven.8hearts_{{Random:{{Range:1,10}}}}}}",},
{"Name": "Raven_8heartsdating","Value": "{{i18n:Raven_8heartsdating_{{Random:{{Range:1,10}}}}}}",},
{"Name": "10hearts","Value": "{{i18n:dialogue.raven.8hearts_{{Random:{{Range:1,10}}}}}}",},
```
</dialogue>


Conversation Topics

| Name | Value |
| --- | --- |
| --- | --- |

<details>
    <summary>Expand Code</summary>

```
{"Name": "dumpsterDive","Value": "{{i18n:DumpsterDiveComment_{{Random:{{Range:1,10}}}}}}",},
{"Name": "hitSlingshot","Value": "{{i18n:HitBySlingshot_{{Random:{{Range:1,10}}}}}}",},
```
</details>

Married Dialogue

| Name | Value |
| --- | --- |
| --- | --- |

<details>
    <summary>Expand Code</summary>

```
{"Name": "inSpouseRoom","Value": "{{i18n:Raven_inSpouseRoom_{{Random:{{Range:1,3}}}}}}",},
{"Name": "onSpousePatio","Value": "{{i18n:Raven_spousePatio_{{Random:{{Range:1,4}}}}}}",},
{"Name": "marRainDay","Value": "{{i18n:Rainy_Day_{{Random:Raven,0,{{Range:1,5}}}}}}",},
{"Name": "marRainNight","Value": "{{i18n:Raven_rainyNight_{{Random:Raven,0,{{Range:1,5}}}}}}",},
{"Name": "marIndDay","Value": "{{i18n:Indoor_Day_{{Random:Raven,0,{{Range:1,5}}}}}}",},
{"Name": "marIndNight","Value": "{{i18n:Indoor_Night_{{Random:Raven,0,{{Range:1,5}}}}}}",},
{"Name": "marOutdoor","Value": "{{i18n:Outdoor_{{Random:Raven,0,{{Range:1,4}}}}}}",},
{"Name": "marGood","Value": "{{i18n:Good_{{Random:0,{{Range:1,9}}}}}}",},
{"Name": "marNeutral","Value": "{{i18n:Neutral_{{Random:0,{{Range:1,9}}}}}}",},
{"Name": "marBad","Value": "{{i18n:Bad_{{Random:0,{{Range:1,9}}}}}}",},
{"Name": "marOneKid","Value": "{{i18n:OneKid_{{Random:0,{{Range:1,4}}}}}}",},
{"Name": "marTwoKids","Value": "{{i18n:TwoKids_{{Random:0,{{Range:1,4}}}}}}",},
{"Name": "marNoBed","Value": "{{i18n:NoBed_{{Random:0,{{Range:1,4}}}}}}",},
```
</dialogue>

Divorce Dialogue

| Name | Value |
| --- | --- |
| --- | --- |

<details>
    <summary>Expand Code</summary>

```
{"Name": "divorcedDialogue","Value": "{{i18n:divorced_{{Random:{{Range:1,8}}}}}}",},
{"Name": "divorcedRejectGift","Value": "{{i18n:RejectGift_Divorced_{{Random:{{Range:1,3}}}}}}",},
{"Name": "divorcedRejectMPend","Value": "{{i18n:Raven_RejectMermaidPendant_Divorced{{Random:{{Range:1,3}}}}}}",},
```
</details>

Movie Invites

| Name | Value |
| --- | --- |
| --- | --- |

<details>
    <summary>Expand Code</summary>

```
{"Name": "movieInvite","Value": "{{i18n:MovieInvitation_{{Random:{{Range:1,5}}}}}}",},
{"Name": "movieInviteSpouse","Value": "{{i18n:MovieInvite_Spouse_{{Random:{{Range:1,5}}}}}}",},
{"Name": "movieInviteAlrInv","Value": "{{i18n:RejectMovieTicket_AlreadyInvitedBySomeoneElse_{{Random:{{Range:1,3}}}}}}",},
{"Name": "movieInviteAlrWat","Value": "{{i18n:RejectMovieTicket_AlreadyWatchedThisWeek_{{Random:{{Range:1,3}}}}}}",},
{"Name": "movieInviteDivorced","Value": "{{i18n:RejectMovieTicket_Divorced_{{Random:{{Range:1,5}}}}}}",},
{"Name": "movieInviteDislike","Value": "{{i18n:RejectMovieTicket_DontWantToSeeThatMovie_{{Random:{{Range:1,3}}}}}}",},
```

Island Dialogue

| Name | Value |
| --- | --- |
| --- | --- |

<details>
    <summary>Expand Code</summary>

```
{"Name": "resortD","Value": "{{i18n:Resort_{{Random:{{Range:1,3}}}}}}",},
{"Name": "resortBarD","Value": "{{i18n:Resort_Bar_{{Random:{{Range:1,3}}}}}}",},
{"Name": "resortChairD","Value": "{{i18n:Resort_Chair_{{Random:{{Range:1,3}}}}}}",},
{"Name": "resortDanceD","Value": "{{i18n:Resort_Dance_{{Random:{{Range:1,3}}}}}}",},
{"Name": "resortEnteringD","Value": "{{i18n:Resort_Entering_{{Random:{{Range:1,3}}}}}}",},
{"Name": "resortLeavingD","Value": "{{i18n:Resort_Leaving_{{Random:{{Range:1,3}}}}}}",},
{"Name": "resortShoreD","Value": "{{i18n:Resort_Shore_{{Random:{{Range:1,3}}}}}}",},
{"Name": "resortTowelD","Value": "{{i18n:Resort_Towel_{{Random:{{Range:1,3}}}}}}",},
{"Name": "resortUmbrellaD","Value": "{{i18n:Resort_Umbrella_{{Random:{{Range:1,3}}}}}}",},
{"Name": "resortWanderD","Value": "{{i18n:Resort_Wander_{{Random:{{Range:1,3}}}}}}",},
```
</dialogues>

Strings - Map Objects 

| Name | Value |
| --- | --- |
| --- | --- |

<details>
    <summary>Expand Code</summary>

```
{"Name": "ravenDesk","Value": "{{i18n:Desk_{{Random:{{Range:1,2}}}}}}",},
{"Name": "ravenGuitar","Value": "{{i18n:Guitar_{{Random:{{Range:1,4}}}}}}",},
{"Name": "ravenLoosePaper","Value": "{{i18n:LoosePaper_{{Random:{{Range:1,4}}}}}}",},
{"Name": "ravenPianoKey","Value": "{{i18n:PianoKey_{{Random:{{Range:1,2}}}}}}",},
{"Name": "ravenYobaShrine","Value": "{{i18n:YobaShrine_{{Random:{{Range:1,3}}}}}}",},
{"Name": "ravenCrystal","Value": "{{i18n:Crystal_{{Random:{{Range:1,4}}}}}}",},
{"Name": "ravenMailbox","Value": "{{i18n:Mailbox_{{Random:{{Range:1,3}}}}}}",},
{"Name": "ravenTrashBag","Value": "{{i18n:TrashBag_{{Random:{{Range:1,6}}}}}}",},
{"Name": "ravenJournal","Value": "{{i18n:Journal_{{Random:{{Range:1,4}}}}}}",},
{"Name": "ravenStove","Value": "{{i18n:Stove_{{Random:{{Range:1,3}}}}}}",},
{"Name": "ravenStove2","Value": "{{i18n:Stove2_{{Random:{{Range:1,2}}}}}}",},
{"Name": "ravenLogs","Value": "{{i18n:Logs_{{Random:{{Range:1,5}}}}}}",},
{"Name": "ravenFridge","Value": "{{i18n:Fridge_{{Random:{{Range:1,5}}}}}}",},
{"Name": "ravenComputer","Value": "{{i18n:Computer_{{Random:{{Range:1,3}}}}}}",},
{"Name": "ravenTrashBin","Value": "{{i18n:TrashBin_{{Random:{{Range:1,4}}}}}}",},
{"Name": "ravenCoatRack","Value": "{{i18n:Raven_CoatRack_{{Random:{{Range:1,7}}}}}}",},
```
</details>


### Mod Compat

| Name | Value |
| --- | --- |
| --- | --- |

<details>
    <summary>Expand Code</summary>

```
//Mod Compat
{"Name": "NBDialogue","Value": "{{i18n:dialogue.raven.NB.generic_{{Random:{{Range:1,22}}}}}}","When": {"HasMod |contains={{NB}}": "true",},},

```
</details>


### Animations

| Name | Value |
| --- | --- |
| `aniSweep` | `l0veraven_raven_sweep` |
| `aniRead` | `l0veraven_raven_read` |
| `aniStand` | `l0veraven_raven_stand` |
| `aniBlunt` | `l0veraven_raven_blunt` |
| `aniEdible` | `l0veraven_raven_edible` |

<details>
    <summary>Expand Code</summary>
    
```
{
    "Name": "aniSweep",
    "Value": "l0veraven_raven_sweep",
},
{
    "Name": "aniRead",
    "Value": "l0veraven_raven_read",
},
{
    "Name": "aniStand",
    "Value": "l0veraven_raven_stand",
},
{
    "Name": "aniBlunt",
    "Value": "l0veraven_raven_blunt",
},
{
    "Name": "aniEdible",
    "Value": "l0veraven_raven_edible",
},
```
</details>


### Schedule Dialogue

| Name | Value |
| --- | --- |
| `stoveSchD` | `{{i18n:Custom_L0veRaven_RavenTentInside_1_{{Random:{{Range:1,2}}}}}}` |
| `standSaloonSchD` | `{{i18n:Saloon_1_{{Random:{{Range:1,2}}}}}}` |
| `shoppingSSschD` | `{{i18n:shoppingSS_1_{{Random:{{Range:1,2}}}}}}` |
| `{{i18n:Forest_101_{{Random:{{Range:1,2}}}}}}` | `{{i18n:Forest_101_{{Random:{{Range:1,2}}}}}}"` |


<details>
    <summary>Expand Code</summary>
    
```
{
    "Name": "stoveSchD",
    "Value": "{{i18n:Custom_L0veRaven_RavenTentInside_1_{{Random:{{Range:1,2}}}}}}",
},
{
    "Name": "standSaloonSchD",
    "Value": "{{i18n:Saloon_1_{{Random:{{Range:1,2}}}}}}",
},
{
    "Name": "shoppingSSschD",
    "Value": "{{i18n:shoppingSS_1_{{Random:{{Range:1,2}}}}}}",
},
{
    "Name": "smokeBluntSchD",
    "Value": "{{i18n:Forest_101_{{Random:{{Range:1,2}}}}}}",
    "When": {
        "HasMod |contains={{NB}}": "true",
    },
},
```
</details>


### Locations
#### Bus Stop
| Name | Value | When | Map | Vanilla / SVE / Both |
| --- | --- | --- | --- | --- |
| `RavenStandBusStop` | `{{i18n:RavenStandBusStop}}` |  | Bus Stop | X |

<details>
    <summary>Expand Code</summary>
    
```
{
    "Name": "RavenStandBusStop",
    "Value": "{{i18n:RavenStandBusStop}}",
},
```
</details>

#### Forest
| Name | Value | When | Mods |
| --- | --- | --- | --- |
| `RavenRelaxForest` | `{{i18n:RavenRelaxForest}}` | `"HasMod |contains={{SVE}}": "false"`, `"HasMod |contains={{NB}}": "false"` |  |
| `RavenRelaxForest` | `{{i18n:RavenRelaxForestSVE}}` | `"HasMod |contains={{SVE}}": "true"`, `"HasMod |contains={{NB}}": "false"` | SVE |
| ``RavenRelaxForest | `{{Random:{{i18n:RavenRelaxForest}},{{i18n:RavenRelaxForest}} {{aniBlunt}},{{i18n:RavenRelaxForest}} {{aniEdible}}}}` | `HasMod |contains={{SVE}}": "false"`, `"HasMod |contains={{NB}}": "true",` |  |
| `` | `` | `` |  |
| `RavenStandRiverForest` | `{{i18n:RavenStandRiverForest}}` | `"HasMod |contains={{SVE}}": "false"`, `"HasMod |contains={{NB}}": "false"` |  |
| `RavenStandRiverForest` | `{{i18n:RavenStandRiverForestSVE}}` | `"HasMod |contains={{SVE}}": "true"`, `"HasMod |contains={{NB}}": "false"` | SVE |
| `` | `` | `` |  |
| `` | `` | `` |  |

<details>
    <summary>Expand Code</summary>
    
```
{
    "Name": "RavenRelaxForest",
    "Value": "{{i18n:RavenRelaxForest}}",
    "When": {
        "HasMod |contains={{SVE}}": "false",
        "HasMod |contains={{NB}}": "false",
    },
},
{
    "Name": "RavenRelaxForest",
    "Value": "{{i18n:RavenRelaxForestSVE}}",
    "When": {
        "HasMod |contains={{SVE}}": "true",
        "HasMod |contains={{NB}}": "false",
    },
},
{
    "Name": "RavenRelaxForest",
    "Value": "{{Random:{{i18n:RavenRelaxForest}},{{i18n:RavenRelaxForest}} {{aniBlunt}},{{i18n:RavenRelaxForest}} {{aniEdible}}}}",
    "When": {
        "HasMod |contains={{SVE}}": "false","HasMod |contains={{NB}}": "true",
    },
},
{
    "Name": "RavenRelaxForest",
    "Value": "{{Random:{{i18n:RavenRelaxForest}},{{i18n:RavenRelaxForest}} {{aniBlunt}},{{i18n:RavenRelaxForest}} {{aniEdible}}}}",
    "When": {
        "HasMod |contains={{SVE}}": "true","HasMod |contains={{NB}}": "true"
    ,}
,},

{
    "Name": "RavenStandRiverForest",
    "Value": "{{i18n:RavenStandRiverForest}}",
    "When": {
        "HasMod |contains={{SVE}}": "false",
        "HasMod |contains={{NB}}": "false",
    },
},
{
    "Name": "RavenStandRiverForest",
    "Value": "{{i18n:RavenStandRiverForestSVE}}",
    "When": {
        "HasMod |contains={{SVE}}": "true",
        "HasMod |contains={{NB}}": "false",
    },
},
{
    "Name": "RavenStandRiverForest",
    "Value": "{{Random:{{i18n:RavenStandRiverForest}},{{i18n:RavenStandRiverForest}} {{aniBlunt}},{{i18n:RavenStandRiverForest}} {{aniEdible}}}}",
    "When": {
        "HasMod |contains={{SVE}}": "false",
        "HasMod |contains={{NB}}": "true",
    },
},
{
    "Name": "RavenStandRiverForest",
    "Value": "{{Random:{{i18n:RavenStandRiverForest}},{{i18n:RavenStandRiverForest}} {{aniBlunt}},{{i18n:RavenStandRiverForest}} {{aniEdible}}}}",
    "When": {
        "HasMod |contains={{SVE}}": "true",
        "HasMod |contains={{NB}}": "true",
    },
},
```
</details>



#### Custom_L0veRaven_RavenTentInside(SVE)
| Name | Value | When | Vanilla / SVE / X |
| --- | --- | --- | --- |
| `tentInside` | `{{i18n:tentInside}}` | `"HasMod |contains={{SVE}}": "false"` | Vanilla |
| `tentInside` | `{{i18n:tentInsideSVE}}` | `"HasMod |contains={{SVE}}": "true"` | SVE |
| `tentInside` | `{{i18n:tentInside}}` | `"HasMod |contains={{SVE}}": "false"` | Vanilla |
| `tentInside` | `{{i18n:tentInsideSVE}}` | `"HasMod |contains={{SVE}}": "true"` | SVE |

<details>
    <summary>Expand Code</summary>
    
```
{
    "Name": "tentInside",
    "Value": "{{i18n:tentInside}}",
    "When": {
        "HasMod |contains={{SVE}}": "false",
    },
},
{
    "Name": "tentInside",
    "Value": "{{i18n:tentInsideSVE}}",
    "When": {
        "HasMod |contains={{SVE}}": "true",
    },
},

{
    "Name": "standStove",
    "Value": "{{RavenTentInside}} {{i18n:standStove}} \"Strings\\schedules\\{{Raven}}:Custom_L0veRaven_RavenTentInside.001\"",
    "When": {
        "HasMod |contains={{SVE}}": "false",
        "HasFlag: |contains={{Raven}}Apartment": false,
    },
},
{
    "Name": "standStove",
    "Value": "{{RavenTentInside}} {{i18n:standStoveSVE}} \"Strings\\schedules\\{{Raven}}:Custom_L0veRaven_RavenTentInside.001\"",
    "When": {
        "HasMod |contains={{SVE}}": "true",
        "HasFlag: |contains={{Raven}}Apartment": false,
    },
},

{
    "Name": "inBed",
    "Value": "{{RavenTentInside}} {{i18n:inBed}} l0veraven_raven_sleep",
},
```
</details>



#### FRL_NPCApt_Floor1
| Name | Value | When | Vanilla / SVE / X |
| --- | --- | --- | --- |
| `apartment` | `{{i18n:apartment}}` | X | Both |
| `standStove` | `{{RavenTentInside}} {{i18n:standStove}} \"Strings\\schedules\\{{Raven}}:Custom_L0veRaven_RavenTentInside.001\"` | `"HasMod |contains={{SVE}}": "false"`, `"HasFlag: |contains={{Raven}}Apartment": false,` | Vanilla |
| `standStove` | `{{RavenTentInside}} {{i18n:standStoveSVE}} \"Strings\\schedules\\{{Raven}}:Custom_L0veRaven_RavenTentInside.001\"` | `"HasMod |contains={{SVE}}": "true"`, `"HasFlag: |contains={{Raven}}Apartment": false,` | SVE |
| `inBed` | `{{RavenTentInside}} {{i18n:inBed}} l0veraven_raven_sleep"` |  | X |

<details>
    <summary>Expand Code</summary>
    
```
{
    "Name": "apartment",
    "Value": "{{i18n:apartment}}",
},

{
    "Name": "standStove",
    "Value": "{{i18n:standStoveApt}} \"Strings\\schedules\\L0veRaven_Raven:Custom_L0veRaven_RavenTentInside.001\"",
    "When": {
        "HasReadLetter": "{{Raven}}Apartment",
    },
},
    {
    "Name": "inBed",
    "Value": "{{i18n:inBedApt}} l0veraven_raven_sleep",
    "When": {
        "HasReadLetter": "{{Raven}}Apartment",
    },
}, 
```
</details>



#### Town
| Name | Value | When | V / S / X |
| --- | --- | --- | --- |
| `relaxBushTown` | `{{Random:{{i18n:relaxBushTown}},{{i18n:relaxBushTown}} {{aniBlunt}},{{i18n:relaxBushTown}} {{aniEdible}}}}` | `"HasMod |contains={{NB}}": "true"` |  |
| `relaxBushTown` | `{{Random:{{i18n:RavenRelaxForestSVE}},{{i18n:relaxBushTown}} {{aniBlunt}},{{i18n:relaxBushTown}} {{aniEdible}}}}` | `"HasMod |contains={{NB}}": "true"` |  |

<details>
    <summary>Expand Code</summary>
    
```
{
    "Name": "RavenStandCC",
    "Value": "{{i18n:standCC}}",},

{
    "Name": "RavenRelaxBushTown",
    "Value": "{{i18n:relaxBushTown}}",
    "When": {
        "HasMod |contains={{NB}}": "false",
    },
},
{
    "Name": "RavenRelaxBushTown",
    "Value": "{{Random:{{i18n:relaxBushTown}},{{i18n:relaxBushTown}} {{aniBlunt}},{{i18n:relaxBushTown}} {{aniEdible}}}}",
    "When": {
        "HasMod |contains={{SVE}}": "false","HasMod |contains={{NB}}": "true",
    },
},
{
    "Name": "RavenRelaxBushTown",
    "Value": "{{Random:{{i18n:relaxBushTown}},{{i18n:relaxBushTown}} {{aniBlunt}},{{i18n:relaxBushTown}} {{aniEdible}}}}",
    "When": {
        "HasMod |contains={{SVE}}": "true","HasMod |contains={{NB}}": "true",
    },
},
```
</details>



#### Hospital
| Name | Value | When | Vanilla / SVE / X |
| --- | --- | --- | --- |
| --- | --- | --- | --- | --- |

<details>
    <summary>Expand Code</summary>
    
```
{
    "Name": "standMeds",
    "Value": "{{i18n:standMeds}}",
},
```
</details>



#### Seed Shop
| Name | Value | When | Vanilla / SVE / X |
| --- | --- | --- | --- |
| --- | --- | --- | --- | --- |

<details>
    <summary>Expand Code</summary>
    
```
{
    "Name": "shoppingSS",
    "Value": "{{i18n:shoppingSS}} \"Strings\\schedules\\{{Raven}}:SeedShop.001\"",
},
```
</details>



#### Saloon
| Name | Value | When | Vanilla / SVE / X |
| --- | --- | --- | --- |
| --- | --- | --- | --- | --- |
| --- | --- | --- | --- | --- |
| --- | --- | --- | --- | --- |
| --- | --- | --- | --- | --- |

<details>
    <summary>Expand Code</summary>
    
```
{
    "Name": "standJobSaloon1",
    "Value": "{{i18n:standJobSaloon1}} {{aniSweep}}",
},
{
    "Name": "standJobSaloon2",
    "Value": "{{i18n:standJobSaloon2}} {{aniSweep}}",
},
{
    "Name": "standJobSaloon3",
    "Value": "{{i18n:standJobSaloon3}} {{aniSweep}}",
},

{
    "Name": "RavenStandTableSaloon",
    "Value": "{{i18n:standTableSaloon}}",
},
```
</details>



#### Archaeology House
| Name | Value | When | Vanilla / SVE / X |
| --- | --- | --- | --- |
| --- | --- | --- | --- | --- |
| --- | --- | --- | --- | --- |

<details>
    <summary>Expand Code</summary>
    
```
{
    "Name": "RavenStandBookcase",
    "Value": "{{i18n:standBookcase}}",
    "When": {
        "HasMod |contains={{SVE}}": "false",
    },
},
{
    "Name": "RavenStandBookcase",
    "Value": "{{i18n:standBookcaseSVE}}",
    "When": {
        "HasMod |contains={{SVE}}": "true",
    },
},
```
</details>



#### Beach
| Name | Value | When | Vanilla / SVE / X |
| --- | --- | --- | --- |
| --- | --- | --- | --- |

<details>
    <summary>Expand Code</summary>
    
```
{
    "Name": "relaxBeach",
    "Value": "{{i18n:relaxBeach}}",
},
```
</details>


#### Mountain
| Name | Value | When | Vanilla / SVE / X |
| --- | --- | --- | --- |
| --- | --- | --- | --- |

<details>
    <summary>Expand Code</summary>
    
```

```
</details>


### Randomizers
#### Clinic Day Randomizer
| Name | Value | When | Vanilla / SVE / X |
| --- | --- | --- | --- |
| --- | --- | --- | --- |
| --- | --- | --- | --- |

<details>
    <summary>Expand Code</summary>
    
```
{
    "Name": "goToClinic",
    "Value": "{{610am}} {{RavenStandMeds}}",
},
{
    "Name": "postClinic",
    "Value": "{{Random:{{RavenStandMountain}},{{RavenRelaxBeach}},{{RavenStandBookcase}},{{RavenStandCC}}}}",
},
```
</details>

#### Morning/Night
| Name | Value | When | Vanilla / SVE / X |
| --- | --- | --- | --- |
| --- | --- | --- | --- |
| --- | --- | --- | --- |
| --- | --- | --- | --- |

<details>
    <summary>Expand Code</summary>
    
```
{
    "Name": "RavenGoodMorning",
    "Value": "{{610am}} {{RavenStandStove}}",
},
{
    "Name": "RavenGoodMorningBus",
    "Value": "{{610am}} {{RavenStandBusStop}}",
},
{
    "Name": "RavenGoodNight",
    "Value": "{{10pm}} {{RavenStandStove}}/{{130am}} {{RavenInBed}}",
},
```
</details>

#### Job Schedules
| Name | Value | When | Vanilla / SVE / X |
| --- | --- | --- | --- |
| --- | --- | --- | --- |
| --- | --- | --- | --- |

<details>
    <summary>Expand Code</summary>
    
```
{
    "Name": "RavenPostJobSaloon1",
    "Value": "{{RavenStandMountain}}",
    "When": {
        "HasReadLetter": "{{Raven}}Apartment",
    },
},
{
    "Name": "RavenPostJobSaloon1",
    "Value": "{{Random:{{RavenRelaxForest}},{{RavenStandRiverForest}}}}",
    "When": {
        "HasFlag: |contains={{Raven}}Apartment": false,
    },
},
```
</details>

#### Free Days
| Name | Value | When | Vanilla / SVE / X |
| --- | --- | --- | --- |
| --- | --- | --- | --- |
| --- | --- | --- | --- |
| --- | --- | --- | --- |
| --- | --- | --- | --- |

<details>
    <summary>Expand Code</summary>
    
```
{
    "Name": "RavenFreeDay1",
    "Value": "{{RavenGoodMorning}}/{{7am}} {{RavenStandRiverForest}}/{{1130am}} {{RavenRelaxBeach}} {{aniRead}}/{{6pm}} {{RavenStandStove}}/{{10pm}} {{RavenInBed}}",
},
{
    "Name": "RavenFreeDay2",
    "Value": "{{RavenGoodMorning}}/{{7am}} {{RavenRelaxBushTown}}/{{1130am}} {{RavenStandTableSaloon}}/{{6pm}} {{RavenStandStove}}/{{10pm}} {{RavenInBed}}",
},
{
    "Name": "RavenFreeDay3",
    "Value": "{{2pm}} {{RavenStandStove}}/{{4pm}} {{RavenRelaxBushTown}}/{{8pm}} {{RavenRelaxBeach}}/{{10pm}} {{RavenInBed}}",
},
{
    "Name": "RavenFreeDay4",
    "Value": "{{4pm}} {{RavenStandTableSaloon}}/{{8pm}} {{RavenStandCC}}/{{10pm}} {{RavenInBed}}",
},
```
</details>

#### Free Day Shop
| Name | Value | When | Vanilla / SVE / X |
| --- | --- | --- | --- |
| --- | --- | --- | --- |
| --- | --- | --- | --- |

<details>
    <summary>Expand Code</summary>
    
```
{
    "Name": "RavenFreeDayShop1",
    "Value": "{{7am}} {{RavenStandRiverForest}}/{{11am}} {{RavenShoppingSS}}/{{1pm}} {{RavenStandMountain}}/{{5pm}} {{RavenRelaxForest}}/{{9pm}} {{RavenStandStove}}/{{12am}} {{RavenInBed}}",
},
{
    "Name": "RavenFreeDayShop2",
    "Value": "{{7am}} {{RavenStandCC}}/{{11am}} {{RavenShoppingSS}}/{{1pm}} {{RavenStandBusStop}}/{{5pm}} {{RavenRelaxBushTown}}/{{9pm}} {{RavenStandStove}}/{{12am}} {{RavenInBed}}",
},
```
</details>

#### Job Randomizers
| Name | Value | When | Vanilla / SVE / X |
| --- | --- | --- | --- |
| --- | --- | --- | --- |
| --- | --- | --- | --- |
| --- | --- | --- | --- |

<details>
    <summary>Expand Code</summary>
    
```
{
    "Name": "RavenJobTasksSaloon",
    "Value": "{{7am}} {{RavenSweepJobSaloon1}}/{{1250pm}} {{RavenSweepJobSaloon2}}/{{350pm}} {{RavenSweepJobSaloon3}}",
},
{
    "Name": "RavenJobTasksSaloon_married",
    "Value": "{{8am}} {{RavenSweepJobSaloon1}}/{{1250pm}} {{RavenSweepJobSaloon2}}/{{350pm}} {{RavenSweepJobSaloon3}}",
},
{
    "Name": "RavenPostJobSaloon",
    "Value": "{{6pm}} {{Random:{{RavenPostJobSaloon1}},{{RavenRelaxBeach}},{{RavenStandBusStop}},{{RavenStandCC}}}}",
},
```
</details>

#### Schedule Randomizers

| Name | Value | When | Vanilla / SVE / X |
| --- | --- | --- | --- |
| --- | --- | --- | --- |
| --- | --- | --- | --- |

<details>
    <summary>Expand Code</summary>
    
```

```
</details>

#### Random Tokens

Schedule Randomizers

| Name | Value |
| `freeDays` | `{{Random:{{RavenFreeDay1}},{{RavenFreeDay2}},{{RavenFreeDay3}},{{RavenFreeDay4}}}}` |
| `freeDaysRandom` | `{{RavenFreeDays}}` |
| `freeDayShopRandom` | `{{Random:{{RavenFreeDayShop1}},{{RavenFreeDayShop2}}}}` |
| `workDay` | `{{RavenGoodMorning}}/{{RavenJobTasksSaloon}}/{{RavenPostJobSaloon}}/{{RavenGoodNight}}` |
| `freeDay` | `{{RavenFreeDaysRandom}}` |
| `freeDayShop` | `{{RavenFreeDayShopRandom}}` |
| `medsDay` | `{{RavenGoToClinic}}/{{10am}} {{RavenPostClinic}}/{{RavenGoodNight}}` |

<details>
    <summary>Expand Code</summary>

```
{
    "Name": "RavenFreeDays",
    "Value": "{{Random:{{RavenFreeDay1}},{{RavenFreeDay2}},{{RavenFreeDay3}},{{RavenFreeDay4}}}}",
},
{
    "Name": "RavenFreeDaysRandom",
    "Value": "{{RavenFreeDays}}",
},
{
    "Name": "RavenFreeDayShopRandom",
    "Value": "{{Random:{{RavenFreeDayShop1}},{{RavenFreeDayShop2}}}}",
},
{
    "Name": "workDay",
    "Value": "{{RavenGoodMorning}}/{{RavenJobTasksSaloon}}/{{RavenPostJobSaloon}}/{{RavenGoodNight}}",
},
{
    "Name": "RavenFreeDay",
    "Value": "{{RavenFreeDaysRandom}}",
},
{
    "Name": "RavenFreeDayShop",
    "Value": "{{RavenFreeDayShopRandom}}",
},
{
    "Name": "medsDay",
    "Value": "{{RavenGoToClinic}}/{{10am}} {{RavenPostClinic}}/{{RavenGoodNight}}",
},
```
</dialogue>

### Event Commands: Complete

| Name | Value | When | Meaning |
| --- | --- | --- | --- | --- |
|`fadeout` |  `globalFade/viewport -1000 -1000` | - | VFX - Fade in |

<details>
    <summary>Expand Code</summary>
    
```
{
    "Name": "fadeout",
    "Value": "globalFade/viewport -1000 -1000",
},
```
</details>

## Custom Locations: Complete

```
"CustomLocations": [
    {
    
    }
]
```

The game loads the maps and associates them with the new locations.

| Name | FromMapFile |
| --- | --- |
| `Custom_L0veRaven_RavenTentInside` | `data/maps/L0veRaven_RavenTentInside.tmx` |
| `Custom_L0veRaven_RavenTentInsideSVE` | `data/maps/L0veRaven_RavenTentInsideSVE.tmx` |

<details>
    <summary>Expand Code</summary>
    
```
{
    "Name": "Custom_L0veRaven_RavenTentInside",
    "FromMapFile": "data/maps/L0veRaven_RavenTentInside.tmx",
},
{
    "Name": "Custom_L0veRaven_RavenTentInsideSVE",
    "FromMapFile": "data/maps/L0veRaven_RavenTentInsideSVE.tmx",
},
```
</details>

## Changes: Add

```
"Changes": [
    {
    
    }
]
```

There is where I put my `Load`s and `Include`s. The order they load in is very important.

| LogName | Action | Target | FromFile | Meanings |
| --- | --- | --- | --- | --- |
| `Blank Loads` | `Load` | `Characters/Dialogue/{{Raven}}`, `Characters/Dialogue/MarriageDialogue{{Raven}}`, `Characters/schedules/{{Raven}}`, `Strings/Schedules/{{Raven}}`, `Data/Events/Custom_L0veRaven_RavenTentInside` `Data/Events/Custom_L0veRaven_RavenTentInsideSVE` | `"data/blank.json` | Loads blank versions of files required for adding content relevant to this mod. |
| `Locations` | `Include` |  | `data/locations/WorldMap.json`, `data/locations/MapPatches.json`, `data/locations/warps.json`, `data/locations/LocationsData.json`, `data/locations/StringsFromMaps.json` | Includes files related to location patches |
| `Spouse Room` | `Load` | `Maps/{{Raven}}SpouseRoom` | `data/maps/{{Raven}}SpouseRoom.tmx` | Loads map |
| `Spouse Patio` | `Load` | `Maps/{{Raven}}SpousePatio` | `data/maps/{{Raven}}SpousePatio.tmx` | Loads map |
| `NPC Data` | `Include` |  | `data/animationFrames.json`, `data/concessionTastes.json`, `data/NPCGiftTastes.json`, `data/schedule.json`, `data/events.json`, `data/festivals.json`, `data/mail.json`, `data/character.json`, `data/outfits.json`, `data/home.json`, `data/winterStarGifts.json`, `data/triggerActions.json` | Includes files required for NPC Data. |
| `Dialogue` | `Include` |  | `data/dialogue/dialogue.json`, `data/dialogue/marriageDialogue.json`, `data/dialogue/giftResponses.json`, `data/dialogue/moviesReactions.json`, `data/StringsFromCSFiles.json`, `data/dialogue/scheduleDialogue.json` | Includes files required for dialogue. |
| `ModCompat` | `Include` |  | `data/modCompat/CJBWarps.json`, `data/modCompat/naturesBounty.json`, `data/modCompat/RavenEventExcludesDELETE.json`, `data/modCompat/downtownZuzu.json`, `data/modCompat/ridgesideVillage.json`, `data/modCompat/pelicanTownPotluck.json`, `data/modCompat/fireworksFestival.json`, `data/modCompat/solsticeWinterStar.json`, `data/modCompat/stardewValleyExpanded.json` | Includes files required for certain mod compatability. |
    
<details>
    <summary>Expand Code</summary>
    
```
{
    "LogName": "content.json: Blank Loads",
    "Action": "Load",
    "Target": "Characters/Dialogue/{{Raven}}, Characters/Dialogue/MarriageDialogue{{Raven}}, Characters/schedules/{{Raven}}, Strings/Schedules/{{Raven}}, Data/Events/Custom_L0veRaven_RavenTentInside, Data/Events/Custom_L0veRaven_RavenTentInsideSVE",
    "FromFile": "data/blank.json",
},
{
    "LogName": "content.json: Locations",
    "Action": "Include",
    "FromFile": "data/locations/WorldMap.json, data/locations/MapPatches.json, data/locations/warps.json, data/locations/LocationsData.json, data/locations/StringsFromMaps.json",
},
{
    "LogName": "content.json: Spouse Patio",
    "Action": "Load",
    "Target": "Maps/{{Raven}}SpousePatio",
    "FromFile": "data/maps/{{Raven}}SpousePatio.tmx",
},
{
    "LogName": "content.json: Spouse Room",
    "Action": "Load",
    "Target": "Maps/{{Raven}}SpouseRoom",
    "FromFile": "data/maps/{{Raven}}SpouseRoom.tmx",
},
{
    "LogName": "content.json: NPC Data",
    "Action": "Include",
    "FromFile": "data/animationFrames.json, data/concessionTastes.json, data/NPCGiftTastes.json, data/schedule.json, data/events.json, data/festivals.json, data/mail.json, data/character.json, data/outfits.json, data/home.json, data/winterStarGifts.json, data/triggerActions.json",
},
{
    "LogName": "content.json: Dialogue",
    "Action": "Include",
    "FromFile": "data/dialogue/dialogue.json, data/dialogue/marriageDialogue.json, data/dialogue/giftResponses.json, data/dialogue/moviesReactions.json, data/StringsFromCSFiles.json, data/dialogue/scheduleDialogue.json",
},
{
    "LogName": "content.json: ModCompat",
    "Action": "Include",
    "FromFile": "data/modCompat/CJBWarps.json, data/modCompat/naturesBounty.json, data/modCompat/RavenEventExcludesDELETE.json, data/modCompat/downtownZuzu.json, data/modCompat/ridgesideVillage.json, data/modCompat/pelicanTownPotluck.json, data/modCompat/fireworksFestival.json, data/modCompat/solsticeWinterStar.json, data/modCompat/stardewValleyExpanded.json",
},
```
</details>