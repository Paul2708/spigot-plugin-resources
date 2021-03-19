# Minecraft Servers

## Java Edition

The Minecraft Java Edition client knows how to communicate with any TCP server that follows the [Minecraft server protocol](https://wiki.vg/Protocol). Servers that conform to this are called "Notchian" servers. While there is an [official implementation](https://www.minecraft.net/en-us/download/server) of this server provided by Mojang, there are re-implementations and modifications of it.

### Modifications

Below you can see a hierarchy of the most popular server software based on the official server. 

- [Vanilla Server](https://www.minecraft.net/en-us/download/server)
  - [CraftBukkit](https://bukkit.org)
    - [Spigot](https://spigotmc.org)
      - [PaperMC](https://papermc.io)
        - [Tuinity](https://github.com/Spottedleaf/Tuinity)
        - [TacoSpigot](https://tacospigot.github.io)
  - [Sponge](https://spongepowered.org)
  - [Forge](https://minecraftforge.net)
  - [Fabric](https://fabricmc.net)
    - [Woven](https://www.wovenmc.net/)

#### CraftBukkit

[CraftBukkit](https://bukkit.org/) is the most commonly known modification of the vanilla server. It doesn't change or modify the protocol, but it provides an API (Bukkit) for server-side modifications called plugins. CraftBukkit and Bukkit themselves have in turn be forked and modified multiple times. The most popular CraftBukkit fork nowadays is Spigot, which also has several popular forks. 

CraftBukkit and most of its descendants are compatible with each other for the most part, meaning that you can often write a plugin for one of them and it will work on all of them.

See [the API repository](./api-repository.md) for a list of tools for Bukkit-based plugin development.

#### Sponge

[Sponge](https://spongepowered.org) is another modified vanilla server independent of CraftBukkit. It also has a plugin system with an API to create server-side mods, but additionally, it's commonly used as a server for the [Forge](http://files.minecraftforge.net) modding platform.

#### TacoSpigot
[TacoSpigot](https://tacospigot.github.io) is a even higher performance fork of [Paper](https://papermc.io)Spigot.

#### Tuinity
[Tuinity](https://github.com/Spottedleaf/Tuinity) is a Fork of Paper aimed to improve performance at high playercounts.

#### Forge

[Forge](https://minecraftforge.net) is a modified version of the vanilla server (& client) just like CraftBukkit, but it's not only for server side modding, it also has a client version that must be installed to work.

#### Fabric

[Fabric](https://fabricmc.net) is an alternative to Forge which aims to be more modular and with a more modern api than forge. It also has native support for [Kotlin](https://kotlinlang.org), [Scala](https://www.scala-lang.org/) and [Groovy](https://groovy-lang.org/).

### Re-Implementations

There is a number of reasons why it may be beneficial to use a server that does not depend on the official vanilla server at all. First, it prevents the [licensing issues that occur when redistributing proprietary code](https://blog.jwf.io/2020/04/open-source-minecraft-bukkit-gpl/). Second of all, it gives you a lot more freedom in how to structure the server, which systems to use etc.

There are many independent Notchian server implementations and you can find [unofficial lists](https://wiki.vg/Server_List) on the internet. Below, we list a couple of Java-based servers that we find interesting.

- [Akarin](https://github.com/Akarin-project/Akarin) by [@akarin-project](https://github.com/Akarin-project/)

  > Akarin is a powerful Minecraft Server Software based on Tuinity.

- [Cleanstone](https://github.com/CleanstoneMC/Cleanstone) by [@Fionera](https://github.com/Fionera) and [@MyzelYam](https://github.com/MyzelYam)

  > Cleanstone is an alternative server software that is based on Spring and Multi-Threading.
 
- [MCHPRS](https://github.com/MCHPR/MCHPRS) by [@MCHPR](https://github.com/MCHPR) 
  
  > A Minecraft creative server built for redstone. Each 256x256 plot runs on a separate thread, allowing for less lag, more concurrency, and many awesome extra features.

- [Minestom](https://github.com/Minestom/Minestom) by [@Minestom](https://github.com/Minestom/)

  > Minestom is an alternative server software that aims to improve the performance.

   __Main features__:
  - Remove the overhead of vanilla features
  - Multi-threaded (Chunks & Entities)
  - Instance system which is much more scalable than worlds
  - Modern API

- [Yatopia](https://github.com/YatopiaMC/Yatopia) by [@YatopiaMC](https://github.com/YatopiaMC)

  > Yatopia combines the code from many Paper forks and optimization mods, as well as many unique optimizations.

In case you want to play around with the protocol in Java yourself, this may be of use:

- [MCProtocolLib](https://github.com/Steveice10/MCProtocolLib) by [@Steveice10](https://github.com/Steveice10/MCProtocolLib)

  > MCProtocolLib provides a protocol library to send and receive packets without using Spigot as dependency.

- [minecraft-server](https://github.com/NyCodeGHG/minecraft-server) by [@NyCodeGHG](https://github.com/NyCodeGHG)

  > This is a small project by me experimenting with the minecraft protocol.
  
### Proxies

Reverse proxies can be used to coordinate connections between different servers.

- [BungeeCord](https://github.com/SpigotMC/BungeeCord)
  - [Waterfall](https://github.com/PaperMC/Waterfall)
    - [Travertine](https://github.com/PaperMC/Travertine)
- [Velocity](https://velocitypowered.com)

#### BungeeCord

BungeeCord is the de-facto standard for Minecraft Networks. You can link multiple servers together and dynamically switch between them. Most Networks use [Waterfall](https://github.com/PaperMC/Waterfall) by the PaperMC team. It's like Paper for spigot, but for bungeecord.

#### Velocity

Velocity is a modern alternative to BungeeCord which is faster and more secure than BungeeCord. It also has a nice [Plugin API](https://docs.velocitypowered.com/en/latest/developers/creating-your-first-plugin.html). Also it provides some compatibility stuff, so it can handle the BungeeCord Plugin Messaging Channel.

#### 

## Bedrock Edition

- [Cloudburst](https://github.com/CloudburstMC/Server) by [@CloudburstMC](https://github.com/CloudburstMC)
  
  > Cloudburst is a server software for Minecraft: Bedrock Edition. It has a few key advantages: written in Java and friendly structure.

## Bridges

There are attempts to construct bridges between the Bedrock and the Java edition protocols, so that players from both editions can play together. Note that none is fully production ready or 100% functional yet.

- [Geyser](https://github.com/GeyserMC/Geyser/) by [@GeyserMC](https://github.com/GeyserMC/), a proxy allowing Bedrock players to join Java servers

- [Waterdog](https://github.com/yesdog/Waterdog) by [@yesdog](https://github.com/yesdog), a fork of Waterfall/BungeeCord adding Bedrock protocol support
