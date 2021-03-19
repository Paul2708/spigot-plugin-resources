# External Applications
This chapter introduces external applications that may be independent of Spigot itself.

## Contents
- [Authentication](#Authentication)
- [Orchestration](#Orchestration)

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