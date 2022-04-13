---
template: overrides/main.html
title: All Commands
---

**Alias means command does the same thing just have a different name.**

**Options wrapped in <> means required. If they wrapped in (), they are optional.**

## Server Commands

| Command     | Alias(es)                   | Description | 
| :--------- | :-------------------------- | :--------- | 
| `/menu` | `/mainmenu` | Opens the main menu GUI. | 
| `/spawn` | `/hub` | Teleport to the Spawn world. | 
| `/survival` |  | Teleport to the Survival-1 world(OldGen)'s spawn. | 
| `/survival2` |  | Teleport to the Survival-2 world(1.18Gen)'s spawn. | 
| `/nether` | `/netherold` | Teleport to the pre 1.16 Nether that is connected to the survival 1 world. | 
| `/nether2` | `/nethernew` | Teleport to the new generation Nether that is connected to the survival 2 world. | 
| `/end` | `/theend` | Teleport to the The End world's spawn. | 
| `/crates` |  | Teleport to Crates at spawn world. | 
| `/vipclaim` |  | One time reward command for VIP members. | 
| `/vipdaily` |  | Daily reward command for VIP members. | 
| `/vipweekly` |  | Weekly reward command for VIP members. | 
| `/jobs` | `/job`,`jobs menu` | Opens Jobs GUI. | 
| `/jobs help` | `jobs commands` | Opens Jobs Help GUI. | 
| `/jobs top` | `jobs gtop` | Opens Jobs Top stats GUI. | 
| `/jobs stats` | `job stats` | Opens Jobs Stats GUI. | 
| `/jobs info` | `job info` | Statistics for each Job GUI. | 
| `/jobs browse` | `jobs list` | Jobs Browsing GUI. | 
| `/rules` |  | Show rules. | 
| `/statsgui` |  | Show many various stats about you GUI. | 
| `/usersettings` | `/settings` | Change per user settings for various things GUI. | 
| `/vaults` |  | Vaults GUI. | 
| `/vip` |  | VIP Section GUI. | 
| `/warps` |  | Server Warps GUI. | 
| `/mcmmo` | `/skills`,`mcmmogui` | mcMMO GUI. | 

## Advanced Achievements

| Command     | Alias(es)                   | Description | Usage  |
| :--------- | :-------------------------- | :--------- | -----:  |
| `/aach` | `/aach help` | Displays Advanced Achievements's help.<br />You can hover or click on the commands. | |
| `/aach book` |  | Creates a book listing the achievements of the player. | |
| `/aach stats` |  | Displays the number of achievements the player has received and the total amount available. | |
| `/aach list` |  | Displays a GUI containing all the achievements and the current progress for each one. | |
| `/aach top` |  | Displays global rankings. |`/aach top (pageNumber)` |
| `/aach week` |  | Displays weekly rankings.. |`/aach week (pageNumber)` |
| `/aach month` |  | Displays monthly rankings. |`/aach month (pageNumber)` |
| `/aach toggle` |  | Toggle achievement notifications in chat. |`/aach toggle (achievementType)` |

## Advanced Enchantments

Custom Enchantments.

| Command     | Alias(es)                   | Description | Usage  |
| :--------- | :-------------------------- | :--------- | -----:  |
| `/alchemist` |  | Open alchemist GUI. | |
| `/enchanter` |  | Open Enchanter GUI. | |
| `/tinkerer` |  | Open Tinkerer GUI. | |
| `/ae info` |  | Information about custom a enchantment. | `/ae info <enchantment>` |
| `/ae list` |  | List all custom enchantments. | |
| `/ae view` |  | Opens a menu containing info about the enchant. | `/ae view <enchantment>` |

## Angel Chest

Death chest plugin.

| Command     | Alias(es)                   | Description | Usage  |
| :--------- | :-------------------------- | :--------- | -----:  |
| `/acgui` |  | Shows the AngelChest GUI containing a list of all your AngelChests and allows you to do everything that's possible with the other commands. | |
| `/acinfo` |  | Lists all your AngelChests and allows you to unlock them, teleport yourself to them or teleport them to yourself. | |
| `/acunlock` |  | Unlock your existing AngelChests for all other players. | `/acunlock [chestID]` |
| `/actp` |  | Allows you to teleport yourself to your AngelChests. | `/actp [chestID]` |
| `/acfetch` |  | Allows you to teleport your AngelChests to yourself. | `/acfetch [chestID]` |
| `/aclist` |  | Shows a list of your AngelChests, including links for teleporting to, fetching and unlocking each chest. This is basically the "chat-only" version of `/acgui`. | |

## Beast Withdraw

| Command     | Alias(es)                   | Description | 
| :--------- | :-------------------------- | :--------- | 
| `/XpBottle <xp>/all` |  |  Transfer Xp to Bottle. | 

## BetterRTP

Random teleport.

| Command     | Alias(es)                   | Description |
| :--------- | :-------------------------- | :--------- | 
| `/rtp` |  | Randomly teleport in your current world. | 
| `/rtp world <world>` |  | Randomly teleport in another world. | 

## CMI

Core plugin. *[] is required*

| Command      | Description | Usage  |
| :--------- | :--------- | -----:  |
| `/afk` | Toggle afk mode. Reason could be provided. | `/afk (-p:playerName) (reason) (-s)` |
| `/autorecharge` | Toggle auto flight recharge. | `/autorecharge (playerName) [exp/money/off] (-s)` |
| `/back` | Teleports back to last saved location. Costs money. | |
| `/balance` | Check money balance. | `/balance (playerName)` |
| `/baltop` | Check top money list. | |
| `/colorlimits` | Shows all posible colors. | |
| `/colorpicker` | Pick hex color. | `/colorpicker (hex/colorname)` |
| `/donate` | Donate item you are holding. | `/donate [playerName] (amount)` |
| `/hat` | Place item like hat. | |
| `/home`   | Teleport to home location. | `/home (homeName)` |
| `/homes`  | A list of homes that you can click to teleport to. | |
| `/ignore`  | Ignores player. | `/ignore (playerName/all)` |
| `/kit`  | Gives predefined kit. Costs money.<br />-preview will open UI where player can check what kit gives but cant actually pick anything from it. This can be achieved by using `/kitpreview` command.<br />-open will open UI with items included in kit where player can choose what he wants to pick from it. Keep in mind that closing UI will delete items in top inventory permanently. This can be achieved by using `/kitopen` command | `/kit [kitName] (-preview) (-open)` |
| `/list`  | Shows online player list. |  |
| `/mail` | Send and receive mail. | `/mail [send/clear/read] [playerName] (message)` |
| `/msg` | Sends message to player. | `/msg [playerName] [message]` |
| `/nick` | Changes player name. | `/nick [newNickName/off]` |
| `/pay` | Perform money transaction. | `/pay [playerName] [amount]` |
| `/playtime`  | Shows player total play time. |  |
| `/playtimetop`  | Shows top list of player total play time. |  |
| `/prewards` | Check playtime rewards. |  |
| `/removehome`  | Removes home. | `/removehome (homeName)` |
| `/reply` | Replay to last message sender. | `/reply [message]` |
| `/sethome`  | Sets home location. | `/sethome (homeName) (block/Material) (slotNumber)` |
| `/shakeitoff` | Dismount any entity riding you. |  |
| `/sit` | Sit in your position. |  |
| `/stats` | Check players stats. |  |
| `/suicide` | Kill your self. |  |
| `/tpa`  | Ask the player if you can teleport to them. | `/tpa [playerName]` |
| `/tpaccept`  | Accept teleport request. | `/tpaccept (playerName)` |
| `/tpahere` | Asks player to accept teleportation to your location. | `/tpahere [playerName]` |
| `/tpdeny` | Deny teleport request. | `/tpdeny [playerName]` |


## Chest Sort

| Command     | Alias(es)                   | Description | 
| :--------- | :-------------------------- | :--------- | 
| `/sort` | `/chestsort` | Toggle your sorting settings using a GUI. | 
| `/sort on|off|toggle` | `/chestsort on|off|toggle` | Enable/disable automatic chest sorting. | 
| `/sort hotkeys` | `/chestsort hotkeys` | Open the hotkeys GUI to enable/disable hotkeys per player. |
| `/sort help` | `/chestsort help` | Display help about the /sort command | 
| `/invsort` | `/isort` | Sort the player's inventory. |
| `/invsort hotbar` | `/isort hotbar` | Sort the player's hotbar. |
| `/invsort all` | `/isort all` | Sort the player's inventory and hotbar. |
| `/invsort toggle` | `/isort toggle` | Toggle automatic inventory sorting. |
| `/invsort on|off` | `/isort on|off` | Enable/disable automatic inventory sorting. |
| `/invsort help` | `/isort help` | Display help about the /invsort command. |

## Daily Shop

| Command     | Description | 
| :--------- |  :--------- | 
| `/ds open [shop]` | Opens the given shop for yourself. | 
| `/ds sell [hand/all/gui]` | Sell player items with different methods. |

## DiscordSRV

| Command     | Description | 
| :--------- |  :--------- | 
| `/discord linked` | Shows if your Minecraft account is linked with a discord account. | 
| `/discord link` | Sends you instructions to link your Minecraft account with your Discord account. | 
| `/discord unlink` | Unlink your Discord account from your Minecraft account. | 

## Dynmap

Online map.

| Command     | Description | 
| :--------- |  :--------- | 
| `/dynmap hide` | Hides the player from the map. | 
| `/dynmap show` | Shows the player on the map again. | 

## GriefPrevention

Claims plugin.

| Command     | Description                          |
| :---------- | :----------------------------------- |
| `/AbandonClaim` | Deletes the claim you’re standing in.  |
| `/ClaimExplosions`       | Toggles if explosions are allowed in the claim. |
| `/Trust` | Gives another player permission to edit in your claim. |
| `/UnTrust` | Revokes any permissions granted to a player in your claim. |
| `/AccessTrust` | Gives a player permission to use your buttons, levers, and beds. |
| `/ContainerTrust` | Gives a player permission to use your buttons, levers, beds, crafting gear, containers, and animals. |
| `/TrustList` | Lists the permissions for the claim you’re standing in. |
| `/PermissionTrust` | Grants a player permission to share his permission level with others. |
| `/UnTrust All` | Removes all permissions for all players in your claim. |
| `/SubdivideClaims` | Switches your shovel to subdivision mode, so you can subdivide your claims. |
| `/RestrictSubclaim` | Restricts a subclaim, so that it inherits no permissions from the parent claim. |
| `/BasicClaims` | Puts your shovel back in basic claims mode. |
| `/AbandonAllClaims` | Deletes all of your claims. |
| `/BuyClaimBlocks` | Converts server money to claim blocks. |
| `/SellClaimBlocks` | 	Converts claim blocks to server money. |
| `/GivePet` | 		Gives away a tamed animal. |
| `/ClaimsList` | 	Lists a player’s claims and claim block details. |
| `/IgnorePlayer` | 		Ignores a target player’s chat messages. |
| `/UnIgnorePlayer` | 	Un-ignores a target player’s chat messages. |
| `/IgnoredPlayerList` | 	Lists all players currently ignored. |
| `/Trapped` | 	Gets a player out of a land claim they are trapped inside. |

## GuiRedeemMCMMO

mcMMO Credits plugin.

| Command     | Description | 
| :--------- |  :--------- | 
| `/credits` | Shows your credits amount. | 
| `/redeem` | Opens redeeming GUI. | 
| `/redeem <skill> <amount>` | Redeem credits via command. | 
| `/credits pay <player> <amount>` | Give credits to another player. | 
| `/credits withdraw <amount>` | Get credits as an item. | 

## HeadDatabase

Player heads as decoration.

| Command     | Alias(es)                   | Description | Usage  |
| :--------- | :-------------------------- | :--------- | -----:  |
| `/headdb` | `/hdb`,`/heads` | Opens the user interface. | |
| `/hdb search` | `/hdb s` | Search for heads in the database. | `/hdb search | s [input]` |

## ItemsAdder

Custom items.

| Command     | Description | 
| :--------- |  :--------- | 
| `/ia` | Opens items info GUI. | 
| `/iablock` | Show info about block you're looking at. | 
| `/ialiquid` | Show info about liquid you're looking at. | 
| `/iarecipe [item]` | Show item recipe GUI. | 
| `/emoji` | Shows you usable emojis in chat. | 

## Jobs

| Command     | Description | Usage  |
| :--------- |  :--------- | -----:  |
| `/jobs gtop/top` | Displays the global toplist in scoreboard or in chat. | `/jobs gtop/top (pageNumber)` |
| `/jobs info jobName` | Displays informations about the given job. | |
| `/jobs join jobName` | Joins to the given job. | |
| `/jobs quests` | Displays the available quests for the player.. | |
| `/jobs quests next` | Resets and gets a new quest lists. Costs money. | |

## PlayerVaults

| Command     | Description | 
| :--------- |  :--------- | 
| `/pv (number)` | Opens the specified vault. | 
| `/pvdel (number)` | Delete your vault. | 

## SFCalc

A calculator for the plugin Slimefun. 

| Command     | Description | 
| :--------- |  :--------- | 
| `/sfcalc calc [required: item] [optional: amount]` | Calculate how much basic slimefun resources you need to make the specified item. | 
| `/sfcalc needed` | Show the items needed for the calculated item. | 

## Selection Visualizer

Shows boundries of regions/claims with particles.

| Command     | Description | 
| :--------- |  :--------- | 
| `/svis gui (type)` | Open gui for setting your personal visualiser settings. | 
| `/svis toggle` | Toggles visualizer for player. | 

## ShopGUI Plus

Server Shop.

| Command     | Description | 
| :--------- |  :--------- | 
| `/shop` | Open the main shop menu. | 
| `/shop [shopName]` | Directly open the specified shop. | 
| `/sell hand [quantity]` | Sell the item held in your hand. | 
| `/sell handall` | Sells all items inventory which are the same as the one being held in your hand . | 
| `/sell all` | Sells all items from your inventory. | 
| `/shop [shopName]` | Directly open the specified shop. | 

## SlimeFun

| Command     | Description | 
| :--------- |  :--------- | 
| `/sf guide` | Get SlimeFun guide book. | 
| `/sf open_guide` | Directly open the guide book. | 
| `/sf search <searchTerm>` | Search for an item. | 
| `/sf stats` | Show player stats. | 

## VeinMiner

| Command     | Description | 
| :--------- |  :--------- | 
| `/vm toggle (category)` | Toggle vein miner on or off for all (or specific) categories. | 
| `/vm mode` | Set the mode that VeinMiner should use to activate for you (the player). Can be either "sneak", "stand" or "always". | 

## VotingPlugin

| Command     | Alias(es)                   | Description | Usage  |
| :--------- | :-------------------------- | :--------- | -----:  |
| `/vote Help/?` | | View help page. | `/vote Help/? (number)` |
| `/vote ToggleReminders` | Enable/disable vote reminders. | |
| `/vote Shop` | Open VoteShop GUI. | |
| `/vote URL` | Open VoteURL GUI. | `/vote URL (SiteName)` |
| `/vote Last` | See your last votes. | |
| `/vote ToggleBroadcast` | oggle whether or not you will recieve vote broadcasts. | |
| `/vote Points` | View your points. | |
| `/vote GUI` | Open VoteGUI. | |
| `/vote Top (Monthly|Weekly|All|Daily)` | Open list of Top Voters. | |
| `/vote Today` | View who list of who voted today. | |
| `/vote Total` | View your total votes. | |
| `/vote Best` | View your best voting. | |
| `/vote Streak` | View your voting streak. | |