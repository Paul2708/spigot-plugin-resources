# API Repository

There are a lot of tools, libraries and frameworks for Bukkit-based plugin development.
This file lists an unexhaustive selection.

## Contents
- [Frameworks](#Frameworks)
- [Utilities](#Utilities)
  - [Environment](#Environment)
  - [Version Independent Code](#Version-Independent-Code)
  - [Dependency Management](#Dependency-Management)
  - [Bridges](#Bridges)
  - [Packets](#Packets)
  - [CI/CD](#CICD)
- [Commands](#Commands)
- [Templates](#Templates)
- [Libraries](#Libraries)
  - [Chat](#Chat)
  - [Configuration](#Configuration)
  - [Events](#Events)
  - [GUIs](#GUIs)
  - [Holograms](#Holograms)
  - [Maps](#Maps)
  - [Mojang](#Mojang)
  - [NBT](#NBT)
  - [Noteblocks](#Noteblocks)
  - [NPCs](#NPCs)
  - [Particles](#Particles)
  - [Scheduling](#Scheduling)
  - [Scoreboards](#Scoreboards)
  - [Sockets](#Sockets)
  - [Testing](#Testing)
  - [Worlds](#Worlds)
- [Other Languages](#Other-Languages)

## Frameworks

Full-blown frameworks that operate on top of Bukkit and define how you write your plugins.

- [helper](https://github.com/lucko/helper) by [@lucko](https://github.com/lucko)

  > helper is another all-in-one framework that aims to reduce most boilerplate code in bukkit but also other stuff like lilypad, redis and database management.
  
  __Main features__:
  - Events
  - Scheduler
  - Promise
  - Metadata
  - Messenger
  - Commands
  - Scoreboard
  - GUI
  - Menu Scheming
  - Random
  - Bucket
  - Profiles
  - Plugin & Maven- Annotations
  - Terminables
  - Serialization
  - Bungee Messaging
  - JavaScript Plugins

- [kelp](https://github.com/PXAV/kelp) by [@PXAV](https://github.com/PXAV/)

  > kelp is an all-in-one framework that aims to avoid version-depended code.

  __Core features__:
  - Sidebar system
  - Inventory system
  - NPC system: 
  - Command system
  - Config system
  
- [SpigotLib](https://github.com/gyurix/SpigotLib) by [@gyurix](https://github.com/gyurix)

  > SpigotLib is a collection of several useful libraries and APIs for Spigot plugin development.
  
  __Features__:
  - Animations
  - BungeeCord Communication
  - Chat API
  - Command API
  - Config management
  - EconomyAPI
  - Gui API
  - Json API
  - Language management
  - Map API
  - Mojang API
  - MySQL API
  - NBT API
  - Packet API
  - PlayerFile
  - RomanNums API
  - Scoreboard API
  - Time API
  - Title API
  - TPS meter and crashreporter
  - Variable API

## Utilities

Tools that help you with compatibility, interopability, and workflow.

### Environment

- [docker-minecraft-server](https://github.com/itzg/docker-minecraft-server) by [@itzg](https://github.com/itzg)

  > Dockerize minecraft servers by providing customizable images.

- [MinecraftDev](https://github.com/minecraft-dev/MinecraftDev) by [@minecraft-dev](https://github.com/minecraft-dev)

  > An IntelliJ plugin that helps you with plugin projects, among others.

- [paperspigot-docker](https://github.com/FelixKlauke/paperspigot-docker) by [@FelixKlauke](https://github.com/FelixKlauke)

  > Easy to use and clean Docker image for running Paper Spigot servers in Docker containers using OpenJDK.


### Version Independent Code

- [compatre](https://github.com/johnnyjayjay/compatre) by [@JohnnyJayJay](https://github.com/johnnyjayjay)

  > compatre replaces version-specific nms and craftbukkit types at runtime using bytecode manipulation.

  __Main features:__
  - Version compatibility with only a single annotation
  - Java agent/Custom class loader

- [ProtocolSupport](https://github.com/ProtocolSupport/ProtocolSupport) by [@ProtocolSupport](https://github.com/ProtocolSupport)

  > ProtocolSupport exists to solve the age-old problem of "What do I do if my users refuse to update their client?" in the most effective way possible.

- [XSeries](https://github.com/CryptoMorin/XSeries) by [@CryptoMorin](https://github.com/CryptoMorin)

  > XSeries provides abstraction for several version-depended classes.

  __Main features__:
  - potions, materials, sounds, particles, ...
  - blocks, entities, bioms

### Dependency Management

- [libby](https://github.com/Byteflux/libby) by [@Byteflux](https://github.com/Byteflux)

  > libby lets you add your external dependencies to the classpath without shading.
  
  __Main features:__
  - Dependency relocation

- [pdm](https://github.com/knightzmc/pdm) by [@knightzmc](https://github.com/knightzmc)

  > pdm lets you add your external dependencies to the classpath without shading.
  
  __Main features:__
  - Declarative dependency notation
  - Reuse of shared dependencies (including transitive ones)
  - Plugin to integrate with Gradle
  
### Bridges

- [PlaceholderAPI](https://github.com/PlaceholderAPI/PlaceholderAPI) by [@extendedclip](https://github.com/extendedclip)

  > PlaceholderAPI provides a uniform way to share information with and use information from other plugins.
  
  __Main features:__
  - Developer API 
  - External expansions
  
- [Vault](https://github.com/milkbowl/Vault) by [@MilkBowl](https://github.com/milkbowl)

  > Vault provides bridge APIs for common plugin systems on Bukkit servers.
  
  __Main features:__
  - Economy API
  - Chat API
  - Permissions API
  
### Packets

- [ProtocolLib](https://github.com/dmulloy2/ProtocolLib) by [@aadnk](https://github.com/aadnk)/[@dmulloy2](https://github.com/dmulloy2)

  > ProtocolLib provides read and write access to the Minecraft server protocol in combination with Bukkit.
  
  __Main features:__
  - Packet interception
  - Obfuscation-free API

### CI/CD

- [Action-SpigotMC](https://github.com/SpraxDev/Action-SpigotMC) by [@SpraxDev](https://github.com/SpraxDev)

  > A GitHub action that allows you to easily compile Minecraft Spigot and install it in your runners local maven repository.

## Commands

High-level alternatives and extensions for Bukkit's rusty command system. 
They all aim to reduce the boilerplate involved in writing commands the traditional way.

- [Annotation Command Framework](https://github.com/aikar/commands) by [@aikar](https://github.com/aikar/)
- [Brigadier](https://github.com/Mojang/brigadier) by [@Mojang](https://github.com/Mojang)
- [cloud](https://github.com/Incendo/cloud) by [@Incendo](https://github.com/Incendo)
- [CommandAPI](https://github.com/JorelAli/CommandAPI) by [@JorelAli](https://github.com/JorelAli/)
- [CommandFlow](https://github.com/unnamed/CommandFlow) by [@unnamed](https://github.com/unnamed)
- [Commands-Plus](https://github.com/Paulanerus/Commands-Plus) by [@Paulanerus](https://github.com/Paulanerus)
- [Commodore](https://github.com/lucko/commodore) by [@lucko](https://github.com/lucko)
- [kaesk](https://github.com/DRSchlaubi/kaesk) by [@DRSchlaubi](https://github.com/DRSchlaubi)
- [Matt's framework](https://github.com/ipsk/MattFramework) by [@ipsk](https://github.com/ipsk)
- [pipe](https://github.com/Lukaesebrot/pipe) by [@Lukaesebrot](https://github.com/Lukaesebrot)
- [simple-commands](https://github.com/Paul2708/simple-commands) by [@Paul2708](https://github.com/Paul2708)

## Templates

Templates are repositories which you can use to reduce the work on creating a new project with all that boilerplate stuff.

- [spigot-gradle-java-template](https://github.com/NyCodeGHG/spigot-gradle-java-template) by [@NyCodeGHG](https://github.com/NyCodeGHG)

  > Template for creating a Spigot Plugin with Gradle.

- [spigot-gradle-kotlin-template](https://github.com/NyCodeGHG/spigot-gradle-kotlin-template) by [@NyCodeGHG](https://github.com/NyCodeGHG)

  > Template for creating a Spigot Plugin with Gradle and the Kotlin programming language.

## Libraries

Libraries are projects that focus on a specific aspect of plugins.

### Chat

- [adventure](https://github.com/KyoriPowered/adventure) by [@KyoriPowered](https://github.com/KyoriPowered)

  > Adventure is a library for server-controllable user interface elements in Minecraft: Java Edition.

- [better-components](https://github.com/RealCerus/better-components) by [@RealCerus](https://github.com/RealCerus/)

  > A very small Spigot library for text components.
  
- [book-api](https://github.com/upperlevel/book-api) by [@upperlevel](https://github.com/upperlevel)

  > This project contains more APIs that help the developer in using the books.

- [InteractiveChat](https://github.com/LOOHP/InteractiveChat) by [@LOOHP](https://github.com/LOOHP)

  > Add click and hover events to chat messages!

- [IridiumColorAPI](https://github.com/Iridium-Development/IridiumColorAPI) by [@Iridium-Development](https://github.com/Iridium-Development)

  > Add gradients and rainbow effects to your messages.

- [kampfire](https://github.com/NyCodeGHG/kampfire) by [@NyCodeGHG](https://github.com/NyCodeGHG)

  > A Java/Kotlin extension library for adventure providing translation functionality.

- [komponent](https://github.com/BomBardyGamer/komponent) by [@BomBardyGamer](https://github.com/BomBardyGamer)

  > An easy to use, fast and lightweight Minecraft chat component library, written in Kotlin.

- [MF-MSG](https://github.com/ipsk/MF-MSG) by [@ipsk](https://github.com/ipsk/)

  > A Discord like markdown implementation for Spigot supporting colors and gradients.
 
- [MineDown](https://github.com/Phoenix616/MineDown) by [@Phoenix616](https://github.com/Phoenix616/)

  > A library that adds the ability to use a MarkDown inspired markup to write Minecraft chat components!

### Configuration

- [simple-message-system](https://github.com/Amejonah1200/simple-message-system) by [@Amejonah1200](https://github.com/Amejonah1200)

  > A simple message system for Spigot.

- [SimplixStorage](https://github.com/Simplix-Softworks/SimplixStorage) by [@Simplix Softworks](https://github.com/Simplix-Softworks)

  > A library to store data in a better way independently from Bukkit or BungeeCord

### Events

- [EventAwaiter.java](https://gist.github.com/Paul2708/32d127c8d1d5c31f3a4751cedee3268e) by [@Paul2708](https://github.com/Paul2708)

  > A class that allows to wait (non-blocking) for an event.

### GUIs

- [AnvilGUI](https://github.com/WesJD/AnvilGUI) by [@WesJD](https://github.com/WesJD/)

  > AnvilGUI provides an API to open an anvil inventory that reacts on renaming.

  __Main features__:
  - support of nearly every version
  - easy-to-use builder
  - set title, items, closing listener and completion listener

- [IF](https://github.com/stefvanschie/IF) by [@stefvanschie](https://github.com/stefvanschie/)

  > An inventory framework for managing GUIs

- [pipe](https://github.com/Lukaesebrot/pipe) by [@Lukaesebrot](https://github.com/Lukaesebrot)

  > Pipe helps to create simple callback-based GUIs.

  __Main features__:
  - intuitive component API (makes additions easier)
  - not bloated
  - easy to use builder classes

- [SmartInvs](https://github.com/MinusKube/SmartInvs) by [@MinusKube](https://github.com/MinusKube/)

  > SmartInvs provides an interface for creating inventories by setting clickable items.

  __Main features__:
  - Iterator for inventory slots
  - Page system
  - Util methods to fill an inventory's row/column/borders/...
  - Actions when player clicks on an item

  More features and examples can be found [here](https://minuskube.gitbook.io/smartinvs/).

- [SpigotGUI](https://github.com/JanHolger/SpigotGUI) by [@JanHolger](https://github.com/JanHolger)

  > A simple to use graphical interface system for spigot.

### Holograms

- [HolographicDisplays](https://github.com/filoghost/HolographicDisplays) by [@filoghost](https://github.com/filoghost)

  > Plugin and API to create holograms.
  
### Maps

- [menu-framework](https://github.com/heroslender/menu-framework) by [@heroslender](https://github.com/heroslender)
  
  > Innovating the way you make menus in minecraft java edition by using maps to render a custom UI and allowing the player to interact with it.

- [MinecraftMediaLibrary](https://github.com/PulseBeat02/MinecraftMediaLibrary) by [@PulseBeat02](https://github.com/PulseBeat02)
  
  > A library built off the Spigot API to play media for users on a server.

- [packet-maps](https://github.com/cerus/packet-maps) by [@cerus](https://github.com/cerus)
  
  > Library for doing cool stuff (screenshots, videos, 3D rendering, gifs, ...) with Minecraft maps using packets

- [spigot-maps](https://github.com/johnnyjayjay/spigot-maps) by [@JohnnyJayJay](https://github.com/johnnyjayjay)
  
  > Library to render custom images, gifs and text on Minecraft map items
  
  __Main features:__
  - Lots of customisation (how often to render, to whom to render, ...)
  - Tools to resize/crop/divide images and gifs to better fit maps
  - Persistence API

### Mojang

- [MojangAPI](https://github.com/DRSchlaubi/mojang_api) by [@DRSchlaubi](https://github.com/DRSchlaubi)
  
  > Java API wrapper for the most commonly used parts of the Mojang API.

### NBT

- [Item-NBT-API](https://github.com/tr7zw/Item-NBT-API) by [@tr7zw](https://github.com/tr7zw)

  > NMS-free NBT api with yaml, json, SQL and Redis serialization.
  
- [KotlinNBT](https://github.com/DevSrSouza/KotlinNBT) by [@DevSrSouza](https://github.com/DevSrSouza)
  
  > Named Binary Tag (NBT) library for Kotlin Multiplatform
  
- [simple-nbt](https://github.com/cerus/simple-nbt) by [@cerus](https://github.com/cerus)

  > Very simple implementation of the NBT (Named Binary Tag) format, including reading and writing.

### Noteblocks

- [NoteBlockAPI](https://github.com/koca2000/NoteBlockAPI) by [@koca2000](https://github.com/koca2000/)

  > Play custom `.nbs` files ingame as noteblock sound.

### NPCs

- [CitizensAPI](https://github.com/CitizensDev/CitizensAPI) by [@fullwall](https://github.com/fullwall)

  > API to create and manage NPCs using the [Citizens](https://github.com/CitizensDev/Citizens2) plugin

- [entity-api](https://github.com/FllipEis/entity-api) by [@FllipEis](https://github.com/FllipEis)

  > Create fake players with additonal settings by using a clean interface.

- [NPC-Lib](https://github.com/juliarn/NPC-Lib) by [@juliarn](https://github.com/juliarn)

  > Asynchronous, high-performance Minecraft NPC library for 1.8-1.16 servers.

- [NPCLib](https://github.com/MinecraftLibraries/NPCLib) by [@JitseB](https://github.com/JitseB)

  > Library that allows developers to create NPCs with an easy-to-use API.

### Particles

- [ParticleLib](https://github.com/ByteZ1337/ParticleLib) by [@ByteZ1337](https://github.com/ByteZ1337)

  > A spigot library supporting all particles from 1.8 to 1.16.5.

### Scheduling

- [TaskChain](https://github.com/aikar/TaskChain) by [@aikar](https://github.com/aikar)

  > Library to help organize tasks.
  
- [Skedule](https://github.com/okkero/Skedule) by [@okkero](https://github.com/okkero/Skedule)
  
  > Library for easier usage of Bukkit Schedulers with the [Kotlin](https://kotlinlang.org programming language.

### Scoreboards

- [FastBoard](https://github.com/MrMicky-FR/FastBoard) by [@MrMicky-FR](https://github.com/MrMicky-FR)

  > A Scoreboard API for Bukkit with 1.7-1.16 support.

- [JScoreboards](https://github.com/JordanOsterberg/JScoreboards) by [@JordanOsterberg](https://github.com/JordanOsterberg)

  > An API with global and per-player scoreboard support.

- [MultiLineAPI](https://github.com/iso2013/MultiLineAPI) by [@iso2013](https://github.com/iso2013/)

  > This API adds custom lines of text below a players name.

- [Netherboard](https://github.com/MinusKube/Netherboard) by [@MinusKube](https://github.com/MinusKube/)

  > Netherboard provides a simple-to-use wrapper for scoreboards.

  __Main features__:
  - simple syntax for creation `BPlayerBoard board = Netherboard.instance().createBoard(player, scoreboard, "My Scoreboard");`
  - simple syntax for adding/removing scores: `board.set("Test Score", 5);`, `board.remove(5)`
 
 - [simple-scoreboard](https://github.com/einfachBlu/simple-scoreboard) by [@einfachBlu](https://github.com/einfachBlu)

   > This library was made to handle easier the scoreboard components, especially tablist and the sidebar.
 
### Sockets

- [Skungee](https://github.com/Skungee/Skungee/) by [@TheLimeGlass](https://github.com/TheLimeGlass)

  > Spigot Socket API and Bungeecord Skript Addon.
  
### Testing

- [MockBukkit](https://github.com/seeseemelk/MockBukkit) by [@seeseemelk](https://github.com/seeseemelk)

  > MockBukkit is a framework that makes the unit testing of Bukkit plugins a whole lot easier. It aims to be provide complete mock implementation of CraftBukkit that can be completely controlled from a unit test.

### Worlds

- [EntityCulling](https://github.com/tr7zw/EntityCulling) by [@tr7zw](https://github.com/tr7zw)

  > Hides entities and tiles(mainly chests) that players are not able to see due to blocks in the way(occlusion culling), and then blocks packets for these entities.

- [FastAsyncWorldEdit](https://github.com/IntellectualSites/FastAsyncWorldEdit) by [@boy0001](https://github.com/boy0001)

  > Fork of WorldEdit that operates asynchronously for higher performance.

- [Iris](https://github.com/VolmitSoftware/Iris) by [@VolmitSoftware](https://github.com/VolmitSoftware)

  > Iris is a full-featured terrain generator including multiple dimensions and configuration opportunities.

- [Slime-World-Manager](https://github.com/Grinderwolf/Slime-World-Manager) by [@Grinderwolf](https://github.com/Grinderwolf/)

  > Implementation of the Slime Region Format, developed by the Hypixel Dev Team.

- [WorldEdit](https://github.com/EngineHub/WorldEdit) by [@sk89q](https://github.com/sk89q)
  
  > Plugin and API to manipulate Minecraft worlds.

- [WorldGeneratorAPI](https://github.com/rutgerkok/WorldGeneratorApi) by [@rutgerkok](https://github.com/rutgerkok)

  > API to create custom world generators easily.
  
- [WorldGuard](https://github.com/EngineHub/WorldGuard) by [@sk89q](https://github.com/sk89q)

  > Plugin and API to manage and protect custom areas of Minecraft worlds.
  
## Other Languages

Who says that you can only use Java to write plugins?

- [VisualBukkit](https://github.com/OfficialDonut/VisualBukkit) by [@OfficialDonut](https://github.com/OfficialDonut)

  > VisualBukkit is a visual programming language for Bukkit plugins.
  
- [Skript](https://github.com/SkriptLang/Skript) by [@bensku](https://github.com/bensku)

  > Skript is a domain specific language for Bukkit with the aim to enable non-programmers to be able to write their own plugins.
  
- [Denizen](https://github.com/DenizenScript/Denizen) by [@mcmonkey4eva](https://github.com/mcmonkey4eva)

  > NPC and general Spigot scripting, using the Denizen Scripting Language.

- [spiglin](https://github.com/johnnyjayjay/spiglin) by [@JohnnyJayJay](https://github.com/johnnyjayjay)

  > spiglin is a collection of extensions and utilities for plugins written in the [Kotlin](https://kotlinlang.org) programming language.

- [KotlinBukkitAPI](https://github.com/DevSrSouza/KotlinBukkitAPI) by [@DevSrSouza](https://github.com/DevSrSouza/)

  > KotlinBukkitAPI is an API for Bukkit/SpigotAPI using the cool and nifty features Kotlin has to make your life more easier.

- [KSpigot](https://github.com/bluefireoly/KSpigot) by [@bluefireoly](https://github.com/bluefireoly)

  > KSpigot adds functionality missing in spigot and makes it possible to do things the kotlin way.

- [spigot-clj-template](https://github.com/johnnyjayjay/spigot-clj-template) by [@JohnnyJayJay](https://github.com/JohnnyJayJay)

  > spigot-clj-template is a [Leiningen](https://leiningen.org) template to write plugins using the [Clojure](https://clojure.org) programming language.

- [spigot-gradle-kotlin-template](https://github.com/NyCodeGHG/spigot-gradle-kotlin-template) by [@NyCodeGHG](https://github.com/NyCodeGHG)

  > Template for creating a Spigot Plugin with Gradle and the Kotlin programming language.

- [minecraft-python](https://github.com/Macuyiko/minecraft-python) by [@Macuyiko](https://github.com/Macuyiko)

  > minecraft-python is an interpreter system leveraging [Jython](https://www.jython.org/) to write Spigot plugins in Python.
  
- [Lukkit](https://github.com/lukkit/Lukkit) by [@lukkit](https://github.com/lukkit)

  > Lukkit allows you to write Spigot plugins in LUA.
