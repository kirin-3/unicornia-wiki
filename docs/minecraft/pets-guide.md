---
template: overrides/main.html
title: myPet Guide
---

## Getting a Pet

There are two ways of obtaining pets on the server. You either need to buy them or tame them. To buy one type `/petshop` and this will open the pet shop in which you can buy almost every pet for pretty cheap.

To tame a mob and make it a pet you will need to beat it with **lead in your hand**. Once they reach low enough HP they will become your pet. Be aware some mobs such as horses and donkeys require you to tame them with vanilla mechanics first.

Players can have up to 3 pets in storage and 1 active pet at a time. To claim an additional pet you must first store your current pet with `/petswitch store`. You will not be able to call it or interact with your other pets while they are in storage. To interact with your MyPet you will need to make it your active MyPet by doing `/petswitch` and selecting the one you want to use.

## Pet GUI

You can access a MyPet GUI with `/pet` command or by clicking on MyPet from the F menu. This GUI allows you to do almost everything without memorizing any commands!

## Skilltrees and Levels

Pets can be assigned to a skill tree with `/pcst`, which allows them to level up and unlock new skills. There are 4 skill trees to choose from; Combat, Utility and Ride. Pets earn XP when they kill mobs, and also earn a small amount of XP any time you kill a mob.

You can see individual skill trees [here](/minecraft/pet-skill-trees).

* **Combat**<br />
Specializes in doing damage and staying alive. It has HP regen and most damage out of all the skill trees. You also get a small inventory space and control skill.
* **Ride**<br />
A rideable pet that specializes in speed and jump height. Also able to fly depending on the mob type. Has decent inventory and pickup range as well. Ranged attacks.
* **Utility**<br />
Massive inventory, pickup range is pretty good, and can pick up XP after level 15. Speed beacon at level 25 +1 at level 50 and night vision.

## Equip Your Pet

Some pets can hold items in their hands or wear armor. To equip a pet with something to hold or wear, simply right-click on your pet while shifting with the item in your hand. To remove the equipment right-click on your MyPet while shifting with shears in your hand.

## Naming Your Pet

You can name your pet with `/petname <name>`. Please note that inappropriate names (anything that wouldn’t be allowed to be said in chat) are not allowed.

You can also use color codes in your pet names. Type `/colors` and `/colorpicker` in the server.

## Feed Your Pet

You must feed your pet to keep its health up or it will die from hunger! If your pet is hungry it will also be weaker and will deal less damage when attacking.

Each pet has a special food that it must be fed. You can see which food is right for your pet by doing `/petinfo`.

## How to Hide/Disable a MyPet

There are two ways to disable a pet, and they work very differently. The first, `/petsendaway`, will hide your active MyPet until you un-hide it with `/petcall`. A pet that has been hidden is still considered your “active MyPet”, it just isn’t visible right now. It also only hides your pet during your current session, so your pet will reappear if you disconnect and reconnect to the server.

The second way to disable a pet is to put it into storage with `/petstore`. Pets that are in storage are completely deactivated until you use `/petswitch` to choose the one you want to use. If all of your pets are in storage, the server will tell you that you do not have a MyPet. This is also how you can claim additional MyPets – by completely deactivating your current one first.

## Pet Behaviors

You can change the way your pet attacks by changing its behavior. Different behaviors are unlocked as your pet levels up. The available behaviors are listed below.

* **Friendly:** Won’t fight, even if it’s attacked by anything​
* **Normal:** Acts like a normal wolf
* **Aggressive:** Attacks everything within 15 blocks of the owner​
* **Farm:** Attacks every hostile mob within 15 blocks of the owner
* **Raid:** Like normal, but the MyPet won’t attack players and their pets
* **Duel:** Attacks other pets with active duel behavior within a 5 block radius​

## Useful Commands

| Command     | Description                          |
| :---------- | :----------------------------------- |
| `/petcall` | Make your pet come to you if it was vanished​. |
| `/pet` | Opens the MyPet GUI interface. |
| `/petsendaway` | Make your pet vanish temporarily. |
| `/petrelease` | Release your pet forever. |
| `/petinfo` | Check your pet’s health and food as well as other stats. |
| `/pcst` | Choose a skilltree for your pet. |
| `/petskill` | Check your pet’s skills and strengths​. |
| `/petname` | Change the name of your pet (see Naming Your Pet above). |
| `/petinventory` | Open your pet’s inventory to see what it has picked up. |
| `/petpickup` | Toggle whether your pet will pick up items or not. |
| `/petbehavior` | Change the behavior class of your pet (see Pet Behavior above). |
| `/petbeacon` | Turn your pet into a walking beacon to give you strength, speed, and other power-ups. |
| `/petswitch` | This allows you to switch between your MyPets. |
| `/petstore` | Store your current pet to claim another. |


## Wiki and More Information

If you wish to learn more about the skills and systems that are included in this plugin, feel free to check the [plugin’s own wiki](https://wiki.mypet-plugin.de/).