# Minecraft Servers

## Java Edition

The Minecraft Java Edition client knows how to communicate with any TCP server that follows the [Minecraft server protocol](https://wiki.vg/Protocol). Servers that conform to this are called "Notchian" servers. While there is an [official implementation](https://www.minecraft.net/en-us/download/server) of this server provided by Mojang, there are re-implementations and modifications of it.

### Modifications

Below you can see a hierarchy of the most popular server software based on the official server. 

- [Vanilla Server](https://www.minecraft.net/en-us/download/server)
  - [CraftBukkit](https://bukkit.org)
    - [Spigot](https://spigotmc.org)
      - [TacoSpigot](https://tacospigot.github.io)
      - [PaperMC](https://papermc.io)
  - [Sponge](https://spongepowered.org)

#### CraftBukkit

[CraftBukkit](https://bukkit.org/) is the most commonly known modification of the vanilla server. It doesn't change or modify the protocol, but it provides an API (Bukkit) for server-side modifications called plugins. CraftBukkit and Bukkit themselves have in turn be forked and modified multiple times. The most popular CraftBukkit fork nowadays is Spigot, which also has several popular forks. 

CraftBukkit and most of its descendants are compatible with each other for the most part, meaning that you can often write a plugin for one of them and it will work on all of them.

See [the API repository](./api-repository.md) for a list of tools for Bukkit-based plugin development.

#### Sponge

[Sponge](https://spongepowered.org) is another modified vanilla server independent from CraftBukkit. It also has a plugin system with an API to create server-side mods, but additionally, it's commonly used as a server for the [Forge](http://files.minecraftforge.net) modding platform.

### Re-Implementations

There is a number of reasons why it may be beneficial to use a server that does not depend on the official vanilla server at all. First of all, it prevents the [licensing issues that occur when redistributing proprietary code](https://blog.jwf.io/2020/04/open-source-minecraft-bukkit-gpl/). Second of all, it gives you a lot more freedom in how to structure the server, which systems to use etc.

There are many independent Notchian server implementations and you can find [unofficial lists](https://wiki.vg/Server_List) on the internet. Below, we list a couple of Java-based servers that we find interesting.

- [Cleanstone](https://github.com/CleanstoneMC/Cleanstone) by [@Fionera](https://github.com/Fionera) and [@MyzelYam](https://github.com/MyzelYam)

  > Cleanstone is an alternative server software that is based on Spring and Multi-Threading.
- [Minestom](https://github.com/Minestom/Minestom) by [@Minestom](https://github.com/Minestom/)

  > Minestom is an alternative server software that aims to improve the performance.

   __Main features__:
  - Remove the overhead of vanilla features
  - Multi-threaded (Chunks & Entities)
  - Instance system which is much more scalable than worlds
  - Modern API

I case you want to play around with the protocol in Java yourself, this may be of use:

- [MCProtocolLib](https://github.com/Steveice10/MCProtocolLib) by [@Steveice10](https://github.com/Steveice10/MCProtocolLib)

  > MCProtocolLib provides a protocol library to send and receive packets without using Spigot as dependency.

### Proxies

*Information about BungeeCord and its descendants TBA...*

## Bedrock Edition

...

## Bridges

There are attempts to construct bridges between the Bedrock and the Java edition protocols, so that players from both editions can play together. Note that none is fully production ready or 100% functional yet.

- [Geyser](https://github.com/GeyserMC/Geyser/) by [@GeyserMC](https://github.com/GeyserMC/), a proxy allowing Bedrock players to join Java servers

- [Waterdog](https://github.com/yesdog/Waterdog) by [@yesdog](https://github.com/yesdog), a fork of Waterfall/BungeeCord adding Bedrock protocol support
