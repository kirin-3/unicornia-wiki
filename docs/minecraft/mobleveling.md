---
template: overrides/main.html
title: Mob Leveling
---

## What is Mob Leveling?

Mob leveling is a system in the server that makes the mobs harder as you get more gear and stuff and play more. 

Not all mobs are leveled, spawner mobs will not be leveled unless you have a special spawner that says otherwise.
Also, there are some mobs that will never get leveled, which are:

* All Passive Mobs, including villagers
* Vex
* Baby mobs
* Ender Dragon
* Wither
* Phantom
* Bat

## How are the Levels calculated?

Firstly, the levels are in a range you will not see only one specific level of mobs even if your mob scaling value is not changed. For the system to level mobs it first gets a number from your stats, you can see this value on your scoreboard(does not show on spawn world), if you do not have the scoreboard open you can do so with `/tab scoreboard toggle` command. The number next to the "Mob Scaling:" is the value the system uses to level mobs for you.

### What does the number mean though?

As said previously there is a range of levels the mobs can spawn with based on your Mob Scaling value.
The number on the left represents the "Mob Scaling" value range and the number on the right represents the value of levels that mobs can spawn with, if your Mob Scaling is in that range.

| Mob Scaling Range     | Mob Level Range                        | 
| :----------: | :-----------------------------------: | 
| 1-100 | 1-3 | 
| 101-160 | 4-5 | 
| 161-400 | 6-10 | 
| 401-600 | 11-15 | 
| 601-800 | 16-25 | 
| 801-1000 | 26-34 | 
| 1001-1300 | 35-45 | 
| 1301-1500 | 46-54 | 
| 1501-1800 | 55-60 | 
| 1801-2100 | 61-66 | 
| 2101-2400 | 67-70 | 
| 2401-3000 | 70-76 | 
| 3001-9999999 | 77-80 | 


Example: If your "Mob Scaling" value is "150" the mobs around you will be level 4 or 5.
If your "Mob Scaling" value is "450" the mobs around you will be between level 11 and 15.
It is possible very rarely the mobs can spawn +/-2 levels of what they are supposed to, so it is possible to spawn a mob slightly higher or lower than what the numbers above show.

The level cap is 80.

### How is the Mob Scaling number calculated?

The Mob Scaling number is: (`Your Total Wealth` X 0.01) + ( `Your play time in hours` X 0.001) + (`Your balance/money` X 0.0001).
To explain further, the money part is simple it's just how much money you have times 0.0001, the playtime you are able to see in the stats page of the main menu.

The wealth number comes from another plugin that calculates your value, it takes into account what you have in your claim area, in chests, containers, and what you have in your inventory. However, it does not calculate all the items. It calculates ores, valuable blocks, gear, and some custom items. To see a breakdown of your wealth and to see the number itself use the `/st stats` command.

## What is affected by the Levels?

Now the actual nerdy part, firstly let me get the simple ones out of the way, the more levels the mob has it drops more money, more vanilla items, vanilla XP, and also custom drops(keys, XP bottles,mcmmo tokens).

The levels also affect the base stats of the mobs. Every mob in the game has different stats firstly there are multipliers the system applies:

* Max health: 1.5
* Movement speed: 0.3
* Attack damage: 1.4
* Ranged attack damage: 1.1
* Creeper blast damage: 1.5
* Follow range: 0.1

There is also attributes it applies to mobs, which normally doesn't happen in vanilla these are:

* Armor bonus: 0.2
* Armor toughness: 0.04
* Attack knockback: 0.2
* Knockback resistance: 0.2
* Zombie spawn reinforcements: 0.1

These are pretty straightforward in terms of what they do, the follow range is just detection/aggro range. Cool now we have some values but what do they mean really?

???- tip "Regarding Wardens"

    Wardens are unique, they are leveled however the system doesn't change any base stats other than XP and item drop values, the higher level more drops but not harder wardens. Also, warden leveling is capped at 50 instead of 80.

There is a very cool tool, plugin devs made for seeing what these numbers actually do. [The Tool](http://pbmc.hopto.org/lm/index.php)

If you put the numbers given above into the respective boxes, you can select and mob you want and see how stats are changed based on levels. Under "Multiplier Processing" select "Default" and click on "Display Multipliers".

Just in case the tool goes down or if you don't wanna bother with it here is the table showing what happens to Zombies at every level on our server:


| CurrentLevel | MaxHealth         | AttackDamage    | MovementSpeed | FollowRange   | Armor       | ArmorToughness | AttackKnockback | KnockbackResistance |
|--------------|-------------------|-----------------|---------------|---------------|-------------|----------------|-----------------|---------------------|
| Not-Levelled | 20 hp[10♥]        | 3 dmg[1.5♥]     | 0.23          | 35 blocks     | 2 / 30.00   | 0 / 20.00      | 0 / 5.00        | 0 / 1.00            |
| Level 1      | 20.375 hp[10.19♥] | 3.05 dmg[1.53♥] | 0.231         | 35.044 blocks | 0.1 / 30.00 | 0.025 / 20.00  | 0.013 / 5.00    | 0.003 / 1.00        |
| Level 2      | 20.75 hp[10.38♥]  | 3.11 dmg[1.55♥] | 0.232         | 35.088 blocks | 0.2 / 30.00 | 0.05 / 20.00   | 0.025 / 5.00    | 0.005 / 1.00        |
| Level 3      | 21.125 hp[10.56♥] | 3.16 dmg[1.58♥] | 0.233         | 35.131 blocks | 0.3 / 30.00 | 0.075 / 20.00  | 0.038 / 5.00    | 0.008 / 1.00        |
| Level 4      | 21.5 hp[10.75♥]   | 3.21 dmg[1.61♥] | 0.233         | 35.175 blocks | 0.4 / 30.00 | 0.1 / 20.00    | 0.05 / 5.00     | 0.01 / 1.00         |
| Level 5      | 21.875 hp[10.94♥] | 3.26 dmg[1.63♥] | 0.234         | 35.219 blocks | 0.5 / 30.00 | 0.125 / 20.00  | 0.063 / 5.00    | 0.013 / 1.00        |
| Level 6      | 22.25 hp[11.13♥]  | 3.32 dmg[1.66♥] | 0.235         | 35.263 blocks | 0.6 / 30.00 | 0.15 / 20.00   | 0.075 / 5.00    | 0.015 / 1.00        |
| Level 7      | 22.625 hp[11.31♥] | 3.37 dmg[1.68♥] | 0.236         | 35.306 blocks | 0.7 / 30.00 | 0.175 / 20.00  | 0.088 / 5.00    | 0.018 / 1.00        |
| Level 8      | 23 hp[11.5♥]      | 3.42 dmg[1.71♥] | 0.237         | 35.35 blocks  | 0.8 / 30.00 | 0.2 / 20.00    | 0.1 / 5.00      | 0.02 / 1.00         |
| Level 9      | 23.375 hp[11.69♥] | 3.47 dmg[1.74♥] | 0.238         | 35.394 blocks | 0.9 / 30.00 | 0.225 / 20.00  | 0.113 / 5.00    | 0.023 / 1.00        |
| Level 10     | 23.75 hp[11.88♥]  | 3.53 dmg[1.76♥] | 0.239         | 35.438 blocks | 1 / 30.00   | 0.25 / 20.00   | 0.125 / 5.00    | 0.025 / 1.00        |
| Level 11     | 24.125 hp[12.06♥] | 3.58 dmg[1.79♥] | 0.239         | 35.481 blocks | 1.1 / 30.00 | 0.275 / 20.00  | 0.138 / 5.00    | 0.028 / 1.00        |
| Level 12     | 24.5 hp[12.25♥]   | 3.63 dmg[1.82♥] | 0.24          | 35.525 blocks | 1.2 / 30.00 | 0.3 / 20.00    | 0.15 / 5.00     | 0.03 / 1.00         |
| Level 13     | 24.875 hp[12.44♥] | 3.68 dmg[1.84♥] | 0.241         | 35.569 blocks | 1.3 / 30.00 | 0.325 / 20.00  | 0.163 / 5.00    | 0.033 / 1.00        |
| Level 14     | 25.25 hp[12.63♥]  | 3.74 dmg[1.87♥] | 0.242         | 35.613 blocks | 1.4 / 30.00 | 0.35 / 20.00   | 0.175 / 5.00    | 0.035 / 1.00        |
| Level 15     | 25.625 hp[12.81♥] | 3.79 dmg[1.89♥] | 0.243         | 35.656 blocks | 1.5 / 30.00 | 0.375 / 20.00  | 0.188 / 5.00    | 0.038 / 1.00        |
| Level 16     | 26 hp[13♥]        | 3.84 dmg[1.92♥] | 0.244         | 35.7 blocks   | 1.6 / 30.00 | 0.4 / 20.00    | 0.2 / 5.00      | 0.04 / 1.00         |
| Level 17     | 26.375 hp[13.19♥] | 3.89 dmg[1.95♥] | 0.245         | 35.744 blocks | 1.7 / 30.00 | 0.425 / 20.00  | 0.213 / 5.00    | 0.043 / 1.00        |
| Level 18     | 26.75 hp[13.38♥]  | 3.95 dmg[1.97♥] | 0.246         | 35.788 blocks | 1.8 / 30.00 | 0.45 / 20.00   | 0.225 / 5.00    | 0.045 / 1.00        |
| Level 19     | 27.125 hp[13.56♥] | 4 dmg[2♥]       | 0.246         | 35.831 blocks | 1.9 / 30.00 | 0.475 / 20.00  | 0.238 / 5.00    | 0.048 / 1.00        |
| Level 20     | 27.5 hp[13.75♥]   | 4.05 dmg[2.03♥] | 0.247         | 35.875 blocks | 2 / 30.00   | 0.5 / 20.00    | 0.25 / 5.00     | 0.05 / 1.00         |
| Level 21     | 27.875 hp[13.94♥] | 4.1 dmg[2.05♥]  | 0.248         | 35.919 blocks | 2.1 / 30.00 | 0.525 / 20.00  | 0.263 / 5.00    | 0.053 / 1.00        |
| Level 22     | 28.25 hp[14.13♥]  | 4.16 dmg[2.08♥] | 0.249         | 35.963 blocks | 2.2 / 30.00 | 0.55 / 20.00   | 0.275 / 5.00    | 0.055 / 1.00        |
| Level 23     | 28.625 hp[14.31♥] | 4.21 dmg[2.1♥]  | 0.25          | 36.006 blocks | 2.3 / 30.00 | 0.575 / 20.00  | 0.288 / 5.00    | 0.058 / 1.00        |
| Level 24     | 29 hp[14.5♥]      | 4.26 dmg[2.13♥] | 0.251         | 36.05 blocks  | 2.4 / 30.00 | 0.6 / 20.00    | 0.3 / 5.00      | 0.06 / 1.00         |
| Level 25     | 29.375 hp[14.69♥] | 4.31 dmg[2.16♥] | 0.252         | 36.094 blocks | 2.5 / 30.00 | 0.625 / 20.00  | 0.313 / 5.00    | 0.063 / 1.00        |
| Level 26     | 29.75 hp[14.88♥]  | 4.37 dmg[2.18♥] | 0.252         | 36.138 blocks | 2.6 / 30.00 | 0.65 / 20.00   | 0.325 / 5.00    | 0.065 / 1.00        |
| Level 27     | 30.125 hp[15.06♥] | 4.42 dmg[2.21♥] | 0.253         | 36.181 blocks | 2.7 / 30.00 | 0.675 / 20.00  | 0.338 / 5.00    | 0.068 / 1.00        |
| Level 28     | 30.5 hp[15.25♥]   | 4.47 dmg[2.24♥] | 0.254         | 36.225 blocks | 2.8 / 30.00 | 0.7 / 20.00    | 0.35 / 5.00     | 0.07 / 1.00         |
| Level 29     | 30.875 hp[15.44♥] | 4.52 dmg[2.26♥] | 0.255         | 36.269 blocks | 2.9 / 30.00 | 0.725 / 20.00  | 0.363 / 5.00    | 0.073 / 1.00        |
| Level 30     | 31.25 hp[15.63♥]  | 4.58 dmg[2.29♥] | 0.256         | 36.313 blocks | 3 / 30.00   | 0.75 / 20.00   | 0.375 / 5.00    | 0.075 / 1.00        |
| Level 31     | 31.625 hp[15.81♥] | 4.63 dmg[2.31♥] | 0.257         | 36.356 blocks | 3.1 / 30.00 | 0.775 / 20.00  | 0.388 / 5.00    | 0.078 / 1.00        |
| Level 32     | 32 hp[16♥]        | 4.68 dmg[2.34♥] | 0.258         | 36.4 blocks   | 3.2 / 30.00 | 0.8 / 20.00    | 0.4 / 5.00      | 0.08 / 1.00         |
| Level 33     | 32.375 hp[16.19♥] | 4.73 dmg[2.37♥] | 0.258         | 36.444 blocks | 3.3 / 30.00 | 0.825 / 20.00  | 0.413 / 5.00    | 0.083 / 1.00        |
| Level 34     | 32.75 hp[16.38♥]  | 4.79 dmg[2.39♥] | 0.259         | 36.488 blocks | 3.4 / 30.00 | 0.85 / 20.00   | 0.425 / 5.00    | 0.085 / 1.00        |
| Level 35     | 33.125 hp[16.56♥] | 4.84 dmg[2.42♥] | 0.26          | 36.531 blocks | 3.5 / 30.00 | 0.875 / 20.00  | 0.438 / 5.00    | 0.088 / 1.00        |
| Level 36     | 33.5 hp[16.75♥]   | 4.89 dmg[2.45♥] | 0.261         | 36.575 blocks | 3.6 / 30.00 | 0.9 / 20.00    | 0.45 / 5.00     | 0.09 / 1.00         |
| Level 37     | 33.875 hp[16.94♥] | 4.94 dmg[2.47♥] | 0.262         | 36.619 blocks | 3.7 / 30.00 | 0.925 / 20.00  | 0.463 / 5.00    | 0.093 / 1.00        |
| Level 38     | 34.25 hp[17.13♥]  | 5 dmg[2.5♥]     | 0.263         | 36.663 blocks | 3.8 / 30.00 | 0.95 / 20.00   | 0.475 / 5.00    | 0.095 / 1.00        |
| Level 39     | 34.625 hp[17.31♥] | 5.05 dmg[2.52♥] | 0.264         | 36.706 blocks | 3.9 / 30.00 | 0.975 / 20.00  | 0.488 / 5.00    | 0.098 / 1.00        |
| Level 40     | 35 hp[17.5♥]      | 5.1 dmg[2.55♥]  | 0.265         | 36.75 blocks  | 4 / 30.00   | 1 / 20.00      | 0.5 / 5.00      | 0.1 / 1.00          |
| Level 41     | 35.375 hp[17.69♥] | 5.15 dmg[2.58♥] | 0.265         | 36.794 blocks | 4.1 / 30.00 | 1.025 / 20.00  | 0.513 / 5.00    | 0.103 / 1.00        |
| Level 42     | 35.75 hp[17.88♥]  | 5.21 dmg[2.6♥]  | 0.266         | 36.838 blocks | 4.2 / 30.00 | 1.05 / 20.00   | 0.525 / 5.00    | 0.105 / 1.00        |
| Level 43     | 36.125 hp[18.06♥] | 5.26 dmg[2.63♥] | 0.267         | 36.881 blocks | 4.3 / 30.00 | 1.075 / 20.00  | 0.538 / 5.00    | 0.108 / 1.00        |
| Level 44     | 36.5 hp[18.25♥]   | 5.31 dmg[2.66♥] | 0.268         | 36.925 blocks | 4.4 / 30.00 | 1.1 / 20.00    | 0.55 / 5.00     | 0.11 / 1.00         |
| Level 45     | 36.875 hp[18.44♥] | 5.36 dmg[2.68♥] | 0.269         | 36.969 blocks | 4.5 / 30.00 | 1.125 / 20.00  | 0.563 / 5.00    | 0.113 / 1.00        |
| Level 46     | 37.25 hp[18.63♥]  | 5.42 dmg[2.71♥] | 0.27          | 37.013 blocks | 4.6 / 30.00 | 1.15 / 20.00   | 0.575 / 5.00    | 0.115 / 1.00        |
| Level 47     | 37.625 hp[18.81♥] | 5.47 dmg[2.73♥] | 0.271         | 37.056 blocks | 4.7 / 30.00 | 1.175 / 20.00  | 0.588 / 5.00    | 0.118 / 1.00        |
| Level 48     | 38 hp[19♥]        | 5.52 dmg[2.76♥] | 0.271         | 37.1 blocks   | 4.8 / 30.00 | 1.2 / 20.00    | 0.6 / 5.00      | 0.12 / 1.00         |
| Level 49     | 38.375 hp[19.19♥] | 5.57 dmg[2.79♥] | 0.272         | 37.144 blocks | 4.9 / 30.00 | 1.225 / 20.00  | 0.613 / 5.00    | 0.123 / 1.00        |
| Level 50     | 38.75 hp[19.38♥]  | 5.63 dmg[2.81♥] | 0.273         | 37.188 blocks | 5 / 30.00   | 1.25 / 20.00   | 0.625 / 5.00    | 0.125 / 1.00        |
| Level 51     | 39.125 hp[19.56♥] | 5.68 dmg[2.84♥] | 0.274         | 37.231 blocks | 5.1 / 30.00 | 1.275 / 20.00  | 0.638 / 5.00    | 0.128 / 1.00        |
| Level 52     | 39.5 hp[19.75♥]   | 5.73 dmg[2.87♥] | 0.275         | 37.275 blocks | 5.2 / 30.00 | 1.3 / 20.00    | 0.65 / 5.00     | 0.13 / 1.00         |
| Level 53     | 39.875 hp[19.94♥] | 5.78 dmg[2.89♥] | 0.276         | 37.319 blocks | 5.3 / 30.00 | 1.325 / 20.00  | 0.663 / 5.00    | 0.133 / 1.00        |
| Level 54     | 40.25 hp[20.13♥]  | 5.84 dmg[2.92♥] | 0.277         | 37.363 blocks | 5.4 / 30.00 | 1.35 / 20.00   | 0.675 / 5.00    | 0.135 / 1.00        |
| Level 55     | 40.625 hp[20.31♥] | 5.89 dmg[2.94♥] | 0.277         | 37.406 blocks | 5.5 / 30.00 | 1.375 / 20.00  | 0.688 / 5.00    | 0.138 / 1.00        |
| Level 56     | 41 hp[20.5♥]      | 5.94 dmg[2.97♥] | 0.278         | 37.45 blocks  | 5.6 / 30.00 | 1.4 / 20.00    | 0.7 / 5.00      | 0.14 / 1.00         |
| Level 57     | 41.375 hp[20.69♥] | 5.99 dmg[3♥]    | 0.279         | 37.494 blocks | 5.7 / 30.00 | 1.425 / 20.00  | 0.713 / 5.00    | 0.143 / 1.00        |
| Level 58     | 41.75 hp[20.88♥]  | 6.05 dmg[3.02♥] | 0.28          | 37.538 blocks | 5.8 / 30.00 | 1.45 / 20.00   | 0.725 / 5.00    | 0.145 / 1.00        |
| Level 59     | 42.125 hp[21.06♥] | 6.1 dmg[3.05♥]  | 0.281         | 37.581 blocks | 5.9 / 30.00 | 1.475 / 20.00  | 0.738 / 5.00    | 0.148 / 1.00        |
| Level 60     | 42.5 hp[21.25♥]   | 6.15 dmg[3.08♥] | 0.282         | 37.625 blocks | 6 / 30.00   | 1.5 / 20.00    | 0.75 / 5.00     | 0.15 / 1.00         |
| Level 61     | 42.875 hp[21.44♥] | 6.2 dmg[3.1♥]   | 0.283         | 37.669 blocks | 6.1 / 30.00 | 1.525 / 20.00  | 0.763 / 5.00    | 0.153 / 1.00        |
| Level 62     | 43.25 hp[21.63♥]  | 6.26 dmg[3.13♥] | 0.283         | 37.713 blocks | 6.2 / 30.00 | 1.55 / 20.00   | 0.775 / 5.00    | 0.155 / 1.00        |
| Level 63     | 43.625 hp[21.81♥] | 6.31 dmg[3.15♥] | 0.284         | 37.756 blocks | 6.3 / 30.00 | 1.575 / 20.00  | 0.788 / 5.00    | 0.158 / 1.00        |
| Level 64     | 44 hp[22♥]        | 6.36 dmg[3.18♥] | 0.285         | 37.8 blocks   | 6.4 / 30.00 | 1.6 / 20.00    | 0.8 / 5.00      | 0.16 / 1.00         |
| Level 65     | 44.375 hp[22.19♥] | 6.41 dmg[3.21♥] | 0.286         | 37.844 blocks | 6.5 / 30.00 | 1.625 / 20.00  | 0.813 / 5.00    | 0.163 / 1.00        |
| Level 66     | 44.75 hp[22.38♥]  | 6.47 dmg[3.23♥] | 0.287         | 37.888 blocks | 6.6 / 30.00 | 1.65 / 20.00   | 0.825 / 5.00    | 0.165 / 1.00        |
| Level 67     | 45.125 hp[22.56♥] | 6.52 dmg[3.26♥] | 0.288         | 37.931 blocks | 6.7 / 30.00 | 1.675 / 20.00  | 0.838 / 5.00    | 0.168 / 1.00        |
| Level 68     | 45.5 hp[22.75♥]   | 6.57 dmg[3.29♥] | 0.289         | 37.975 blocks | 6.8 / 30.00 | 1.7 / 20.00    | 0.85 / 5.00     | 0.17 / 1.00         |
| Level 69     | 45.875 hp[22.94♥] | 6.62 dmg[3.31♥] | 0.29          | 38.019 blocks | 6.9 / 30.00 | 1.725 / 20.00  | 0.863 / 5.00    | 0.173 / 1.00        |
| Level 70     | 46.25 hp[23.13♥]  | 6.68 dmg[3.34♥] | 0.29          | 38.063 blocks | 7 / 30.00   | 1.75 / 20.00   | 0.875 / 5.00    | 0.175 / 1.00        |
| Level 71     | 46.625 hp[23.31♥] | 6.73 dmg[3.36♥] | 0.291         | 38.106 blocks | 7.1 / 30.00 | 1.775 / 20.00  | 0.888 / 5.00    | 0.178 / 1.00        |
| Level 72     | 47 hp[23.5♥]      | 6.78 dmg[3.39♥] | 0.292         | 38.15 blocks  | 7.2 / 30.00 | 1.8 / 20.00    | 0.9 / 5.00      | 0.18 / 1.00         |
| Level 73     | 47.375 hp[23.69♥] | 6.83 dmg[3.42♥] | 0.293         | 38.194 blocks | 7.3 / 30.00 | 1.825 / 20.00  | 0.913 / 5.00    | 0.183 / 1.00        |
| Level 74     | 47.75 hp[23.88♥]  | 6.89 dmg[3.44♥] | 0.294         | 38.238 blocks | 7.4 / 30.00 | 1.85 / 20.00   | 0.925 / 5.00    | 0.185 / 1.00        |
| Level 75     | 48.125 hp[24.06♥] | 6.94 dmg[3.47♥] | 0.295         | 38.281 blocks | 7.5 / 30.00 | 1.875 / 20.00  | 0.938 / 5.00    | 0.188 / 1.00        |
| Level 76     | 48.5 hp[24.25♥]   | 6.99 dmg[3.5♥]  | 0.296         | 38.325 blocks | 7.6 / 30.00 | 1.9 / 20.00    | 0.95 / 5.00     | 0.19 / 1.00         |
| Level 77     | 48.875 hp[24.44♥] | 7.04 dmg[3.52♥] | 0.296         | 38.369 blocks | 7.7 / 30.00 | 1.925 / 20.00  | 0.963 / 5.00    | 0.193 / 1.00        |
| Level 78     | 49.25 hp[24.63♥]  | 7.1 dmg[3.55♥]  | 0.297         | 38.413 blocks | 7.8 / 30.00 | 1.95 / 20.00   | 0.975 / 5.00    | 0.195 / 1.00        |
| Level 79     | 49.625 hp[24.81♥] | 7.15 dmg[3.57♥] | 0.298         | 38.456 blocks | 7.9 / 30.00 | 1.975 / 20.00  | 0.988 / 5.00    | 0.198 / 1.00        |
| Level 80     | 50 hp[25♥]        | 7.2 dmg[3.6♥]   | 0.299         | 38.5 blocks   | 8 / 30.00   | 2 / 20.00      | 1 / 5.00        | 0.2 / 1.00          |
