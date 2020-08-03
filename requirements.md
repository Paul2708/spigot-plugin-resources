# Spigot Plugin Development - Requirements

To develop a plugin as defined by the client, it is important to know _everything_ about the plugin.
This file lists information and questions that have to be specified and answered.

## Server software
> The server software is "the jar you run to start the server".

- Are you using Spigot, Paper or something else?
- (Are you using BungeeCord?)
- On which version runs the server?
  - Should the plugin support a range of versions, e.g. 1.8 to 1.14.4?

## Configuration
> Most times, a custom plugin provides a lot of possible configurations.

- Should the plugin provide a configuration?
- What do you want to configure?
  - Give a detailed description about the configuration fields including type (int, message, ...) and impact.
- If you edit the configuration, when should the changes be active?
  - after a plugin restart/reload?
  - instant?
  - after executing a command like `/config reload`?

## Messages
> Messages include player messages, inventory names, sidebar scores, tab list messages and item names.

- Should it be possible to edit messages?
- Could the messages contain any placeholder?
- Should the plugin support multiple languages (per player)?

## Inventories
Please provide screenshots and detailed descriptions for every inventory.
You can create an inventory by filling a chest in creative.

## Commands
> Commands are very common. So it's just more important to fully specify the commands.

- What commands do you want?

The following information should be given for _every_ command.
- Give a detailed description about the command and what it should do if executed.
- Who is allowed to execute it?
  - players with a special permission?
  - OP players?
  - only console?
  - ...
- Describe every parameter of the command.
  - optional or not?
  - What does the parameter mean and what is the impact of it?
  - What values are valid for the parameter? (e.g. only positive numbers, single word without spaces, ...)


## Data management
> Often, a plugin manages data like warp points, coins, etc.
The data has to be stored somewhere.

- Where should the data be stored?
  - SQL database (MySQL, sqlLite, Postgres, ...)
  - non-SQL database (MongoDB, ...)
  - plain text file (`.json` file in `plugins/`, ...)
  - in-memory (the data is only available if the server is running and no data is saved after restarting the server)
- What kind of data should be stored? 
  

## Others
- Should the plugin be "reload-save"? Meaning reloading the server should not break the plugin.
- Should the plugin provide an API that can be accessed by other plugins?
  - And if so, please specify the interface.
  - Should the plugin call own events?
- Should external APIs be used in the plugin? (e.g. Vault)
- Are there plugins/APIs, you _don't_ want to have on the server to run the developed plugin?
