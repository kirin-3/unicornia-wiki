---
template: overrides/main.html
title: How to Claim Land
---

## Why should you claim your land?

In our server griefing is against the rules and if someone griefs your base it will be rolled back and fixed but there are bad apples always and stolen items can be hard to recover so claiming your land is highly encouraged.

## Getting Started

Grief Prevention is quite straightforward, there are only a few items you need to get started.

==A Golden Shovel.== This will allow you to create and resize your claims.

==A Stick.== This will allow you to check if a block is claimed as well as check the borders of claims. The outlines will be shown by Gold Block as markers with Glowstone at the corners.

Using the golden shovel – The controls for the golden shovel are as follows:

* Creating a new claim – Right clicking at two points to mark two opposing corners will create a claim.
* Resizing a claim – Right click once using a stick to view an existing claim and its respective markers. Right click on a corner block with the golden shovel and then again on a different position further in or further out to move that corner.
* Cancelling operations – Putting away a golden shovel without completing an operation cancels all actions


Using the stick – The controls for the stick are as follows:

* Right clicking shows existing claim locations
* Shift right clicking searches for all claims in a 100 block radius and shows their location
* Left clicking hides the markers

After you have created your claim there are a few extra commands and tips you can use.

To set a claim spawn use – `/claimsetspawn`

To teleport to your claim after setting claim spawn use – `/claimspawn`

If you wish to trust a friend to allow them to build use – `/trust <playername>`

To view information about your claim ( while standing inside the claim ) use – `/claiminfo`

To delete your claim ( while standing inside ) use – `/abandonclaim`

To gain more claim blocks you can buy them via – `/buyclaimblocks <number of blocks>`

## Simple Video Guide

<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/33uKeMNQSls" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## Trust System

There are four different types of trust: Accessors, Builders, Containers, and Managers. Each of them has a different tier of abilities and things they can access to. Give other people these permissions **wisely** in order to avoid potential grief in your claimed land. 

**Accessors**
Command: `/accesstrust <player>`
Commandalias: `at`
Grants a player entry to your claim(s) and use of your bed
 

**Containers**
Command: `/containertrust <player>`
Commandalias: `ct`
Grants a player access to your claim’s containers, crops, animals, bed, buttons, and levers


**Builders**
Command: `/trust <player>`
Commandalias: `t`
Grants a player edit access to your claim(s)


**Managers**
Command: `/permissiontrust <player>`
Commandalias: `pt`
Grants a player permission to grant their level of permission to others

**Other commands**
`/trustall <player>` – Allows a player to access ALL of your claims
`/untrust <player>` – Untrusts a player from the current claim you’re standing on
`/untrustall <player>` – Untrusts a player from ALL of your claims
`/trustlist` – Shows a list of people who are trusted on the claim you’re standing on

## Subdividing Claims

Subdividing claims allows you to give players access to specific parts of your claim. This is the best way to manage a town or shop!

The idea behind subdivisions is easy. You are creating mini-claims within your main claim so that you can trust people to certain areas, but not the entire claim. You are still in control of the border of these mini-claims (size and location). Once a subdivision is created you can trust people the same way as before. Just stand in the mini-claim and use the trust commands. It will only trust them to the mini-claim. (To trust someone to your main claim you will need to stand outside of any mini-claims you’ve created.)

​​To create a subdivision you need to go into “subdivision mode”. You can access this mode with `/subdivideclaims`. Once you are in this mode you can create the subdivisions the same way you would make a regular claim, just right click two corners. Subdivisions will be outlined with a white dotted line. To leave subdivision mode use `/basicclaims`.

When you execute the command `/abandonclaim` while standing inside a sub-division, it will **only** remove the sub-division you’re standing on, not the whole main claim.

Other commands like `/containertrust <player>` and `/accesstrust <player>` will also only lock on to a particular sub-division given that you’re standing on that same sub-division claim.

## Commands

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

