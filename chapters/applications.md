# External Applications
This chapter introduces external applications that may be independent of Spigot itself.

## Contents
- [Authentication](#Authentication)
- [Orchestration](#Orchestration)
- [Performance](#Performance)
- [Template](#Template)

## Authentication
### Mc-Auth
[Mc-Auth](https://github.com/Mc-Auth-com/Mc-Auth/) by [@SpraxDev](https://github.com/SpraxDev) is an [oAuth2](https://tools.ietf.org/html/rfc6749) implementation for Minecraft.
This allows developers to add an additional login option (next to Login via Google or GitHub): Login via Minecraft.

#### How does it work?
The user who wants to log in through Minecraft clicks on a button on your web page that redirects to [https://mc-auth.com](https://mc-auth.com).
Now, the user has to connect to the Minecraft server `mc-auth.com`.
After joining, they will be kicked immediately with a 6-digit code as a reason.
The user has to fill in the form on [https://mc-auth.com](https://mc-auth.com) by adding their Minecraft ingame name and the code they got.
If the provided data is correct, the user will be redirected to the original web page again and is now logged in.

## Orchestration
### CloudNet
*tbd*

### See Also
- [SubServers2](https://github.com/ME1312/SubServers-2) by [@ME1312](https://github.com/ME1312)
  
  > SubServers 2 is a rewrite of SubServers, the Server Management Platform.

## Performance
### See Also
- [KibblePatcher](https://github.com/KibbleLands/KibblePatcher) by [@KibbleLands](https://github.com/KibbleLands)
  
  > KibbleLands Spigot patcher for better server performances and bytecode optimization.

## Template
### Plugin-Starter
[Plugin-Starter](https://github.com/Tammo0987/Plugin-Starter) by [@Tammo0987](https://github.com/Tammo0987) is a project that creates Minecraft plugin boilerplate code via CLI or from a web interface.
It is inspired by [Spring Initializr](https://start.spring.io).
It allows developers to select the programming language, server software, Minecraft version, and dependencies.
The result is a generated zip file that can be extracted to start working with it.
