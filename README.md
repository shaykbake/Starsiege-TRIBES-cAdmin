# Starsiege: TRIBES cAdmin
cAdmin Modification for Starsiege: TRIBES

## What is cAdmin?

This Tribes server-side modification was thought up when I decided that I want a quick and easy in-game way to change mods on a server without having to physically be at the server or even remoted into it to manually launch the server with a new mod.

Instead, cAdmin allows for configuring server mods to run with their own specific Target Line replacements, and it is all possible due to the way Tribes' console.cs file works when a server is initialized.

In order to work, a client has to have a client-side script that sends and receives messages to and from the server, and so there are only a few core files and file changes for the modification to work:
1. cAdmin.s.cs
2. cAdmin.c.cs
3. console.cs

### cAdmin.s.cs
This file contains the core functions for cAdmin, and it is also where you would configure server target lines that get passed for whatever mod is selected.

### cAdmin.c.cs
This file simply contains a few small functions that allow the client to perform functions through the cAdmin modification with the `cAdmin()` command and any arguments that get passed through it.

### console.cs
The `console.cs` in Tribes has to be updated to work with cAdmin. The changes needed do not make it so that the `console.cs` file cannot work as traditionally, launching a server instance with a specified target line the default way. In fact, running a server like so is completely unaffected by cAdmin.

## Help/Community
In addition to the Issues and Discussion tabs within the Github projects page here, you can also reach out to me regarding this project via the {LS} Long Shots team resources - notably our [forums](https://longshots.mk0.pw/forums/) and [Discord](https://longshots.mk0.pw/discord/).
