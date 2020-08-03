API repository
---
Nowadays, there exists a lot of useful Spigot APIs that reduce boilerplate.
This file lists some of them.

## Commands
- [commands](https://github.com/aikar/commands) by [@aikar](https://github.com/aikar/)

  > commands is a command dispatcher framework that reduces boilerplate by annotations.

- [kaesk](https://github.com/DRSchlaubi/kaesk) by [@DRSchlaubi](https://github.com/DRSchlaubi)

  > kaesk is an annotation-based command framework that reduces duplicated code and boilerplate.
  
  __Main features__:
  - annotation-based command handling
  - every command is a dedicated method
  - custom error and argument handler
  - simple and easy-to-use

## NPCs
- [NPCLib](https://github.com/MinecraftLibraries/NPCLib) by [@JitseB](https://github.com/JitseB)
  
  > Library that allows developers to create NPCs with an easy-to-use API.

## Inventories
- [AnvilGUI](https://github.com/WesJD/AnvilGUI) by [@WesJD](https://github.com/WesJD/)

  > AnvilGUI provides an API to open an anvil inventory that reacts on renaming.
  
    __Main features__:
    - support of nearly every version
    - easy-to-use builder
    - set title, items, closing listener and completion listener

- [SmartInvs](https://github.com/MinusKube/SmartInvs) by [@MinusKube](https://github.com/MinusKube/)
  
  > SmartInvs provides an interface for creating inventories by setting clickable items.
  
  __Main features__:
  - Iterator for inventory slots
  - Page system
  - Util methods to fill an inventory's row/column/borders/...
  - Actions when player clicks on an item
    
  More features and examples can be found [here](https://minuskube.gitbook.io/smartinvs/).
  
## Scoreboards
- [Netherboard](https://github.com/MinusKube/Netherboard) by [@MinusKube](https://github.com/MinusKube/)

  > Netherboard provides a simple-to-use wrapper for scoreboards.
  
  __Main features__:
  - simple syntax for creation `BPlayerBoard board = Netherboard.instance().createBoard(player, scoreboard, "My Scoreboard");`
  - simple syntax for adding/removing scores: `board.set("Test Score", 5);`, `board.remove(5)`
  
- [MultiLineAPI](https://github.com/iso2013/MultiLineAPI) by [@iso2013](https://github.com/iso2013/)

  > This API adds custom lines of text below a players name.

## Create version-independent plugins
- [kelp](https://github.com/PXAV/kelp) by [@PXAV](https://github.com/PXAV/)

  > kelp is an all-in-one framework that aims to avoid version-depended code.
  
  __Main features__:
  - Sidebar system
  - Inventory system
  - NPC system: 
  - Command system
  - Config system

- [XSeries](https://github.com/CryptoMorin/XSeries) by [@CryptoMorin](https://github.com/CryptoMorin)

  > XSeries provides abstraction for several version-depended classes.
  
  __Main features__:
  - potions, materials, sounds, particles, ...
  - blocks, entities, bioms

## Other resources
- [docker-minecraft-server](https://github.com/itzg/docker-minecraft-server) by [@itzg](https://github.com/itzg)

  > Dockerize minecraft servers by providing customizable images.
  
- [WLOSP](https://github.com/WeLoveOpenSourcePlugins/contribute) (organization)

  > An organization that clones premium plugins (plugins you have to pay for) and publishes them on GitHub - free-to-use and open-source.
  
- [Cleanstone](https://github.com/CleanstoneMC/Cleanstone) by [@Fionera](https://github.com/Fionera) and [@MyzelYam](https://github.com/MyzelYam)

  > Cleanstone is an alternative server software that is based on Spring and Multi-Threading.
  
- [Geyser](https://github.com/GeyserMC/Geyser) by [@GeyserMC](https://github.com/GeyserMC/)

  > Geyser is a proxy that allows "Bedrock players" to join "Java servers". Note that the project is not production-ready.
  
- [Minestom](https://github.com/Minestom/Minestom) by [@Minestom](https://github.com/Minestom/)

  > Minestom is an alternative server software that aims to improve the performance.
  
   __Main features__:
   - Remove the overhead of vanilla features
   - Multi-threaded (Chunks & Entities)
   - Instance system which is much more scalable than worlds
   - Modern API
   
- [PaperMC](https://github.com/PaperMC/Paper)

  > The known PaperMC server software.
  
- [MinecraftDev](https://github.com/minecraft-dev/MinecraftDev) by [@minecraft-dev](https://github.com/minecraft-dev)

  > An IntelliJ plugin that setups minecraft plugin projects.
  
- [Slime-World-Manager](https://github.com/Grinderwolf/Slime-World-Manager) by [@Grinderwolf](https://github.com/Grinderwolf/)

  > Implementation of the Slime Region Format, developed by the Hypixel Dev Team.
  
- [MCProtocolLib](https://github.com/Steveice10/MCProtocolLib) by [@Steveice10](https://github.com/Steveice10/MCProtocolLib)

  > MCProtocolLib provides a protocol library to send and receive packets without using Spigot as dependency.
