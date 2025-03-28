# Frogmonster Randomizer Setup Guide

This guide presumes you've never used Archipelago before. If you know the basics, skip to [Client Setup](https://github.com/Rooby-Roo/FrogmonsterAPWorld?tab=readme-ov-file#client-setup) for stuff specific to this game, and grab the files from the [Releases page](https://github.com/Rooby-Roo/FrogmonsterAPWorld/releases/latest).

# Choose your Settings
Download `Frogmonster.yaml` from this repository and name it something unique. Open it up in a text editor of your choice. Give yourself a player name, and choose options according to your liking. (Settings which give you multiple options are written as weighted choices (50 or 0) by default. Writing them out unweighted like `game_difficulty: normal` is perfectly OK too.) Consider running your YAML through a YAML linter to make sure that you didn't break YAML formatting accidentally.

# Generating a Game

Choose one of the below options:

### I'm playing alone, or I'm hosting the room:
Download the following:
1. `frogmonster.apworld` (found [on the Releases page](https://github.com/Rooby-Roo/FrogmonsterAPWorld/releases/latest))
2. [Archipelago](https://github.com/ArchipelagoMW/Archipelago/releases/latest).

Open the folder where Archipelago was installed. Place `frogmonster.apworld` in the folder `\custom_worlds`, and place your YAML file in `\Players`. If there are other players in your multiworld, they will sent you their YAMLs as well, which you will also place in `\Players`. 

Optionally, you can open the `host.yaml` file and adjust some generation settings if you'd like. The defaults are fine if you're new to Archipelago, though.

Once you've got all the player YAMLs, open Archipelago, and click "Generate". If everything works correctly, a zip folder will appear in your `\outputs` folder. Go to [archipelago.gg](https://archipelago.gg) and click "Host Game". Upload that .zip file and create a room. Share this room link with any other players.

If you're having issues with the generation process, ask around. Consider providing the generation logs from your most recent attempts (found in `\logs`) as well as the YAML files used in generation.

### I'm not hosting the room:
Send your completed settings YAML to the room host. Make sure they also have a copy of the `frogmonster.apworld` file (they can download it here, or you can send it to them). Eventually, the host will send you a room link.

# Client Setup
The Frogmonster AP Client is currently developed by the main developer of Frogmonster, and is distributed as a Steam beta of the game. To access Frogmonster game betas, open your Steam library, right click on Frogmonster, click "Properties", and then click "Betas". You can select the randomizer client from the dropdown menu on this page. Once you've selected a beta, launch Frogmonster.

In order to connect to your randomized game, start a new save file (or open a save file previously used during this run of the randomizer). Once you've opened a world, you will be presented with a dark screen as the game waits for you to connect to the world. Once you get to this screen, go the console window (that opened with Frogmonster) and run the /connect command as prompted. You will need the server name (most likely archipelago.gg), your port number (5 digits, which you can get from the room link), and your slot name (which is the name you put in your YAML settings. You can also pull this from the room page if you need to). If your server has a password set, you will need this as well.

A completed /connect command will look something like this: `/connect archipelago.gg:38281 FrogGamer`. Once you've entered that correctly, your game will start, and you can begin playing!

# Frogmonster client FAQ:

### What's randomized?
By default, every single chest in the game, as well as every item given to you by NPCs (except for Orchus Key and Workshop Key), and every boss reward is randomized. Additionally, each bug when eaten for the first time will give you a randomized item, and the ability to equip each bug is shuffled among these locations. Optionally, you can also include the assorted sliding tile puzzles, so their coin rewards are shuffled, and completing them gives an item.

### So, how do you win, exactly?
The goal is set in your settings. By default, you win the game by going to Myzand's Forest and defeating Myzand. Alternatively, with your settings, you can set it up so that the goal condition is instead to collect the Eye Fragment, which is just behind the 6-Eye Door.

### I've beaten 6 Ridge bosses, but the 6-Eye Door in Ridge isn't opening.
The door being opened is tied to how many Myzand Gun Upgrades you have in your inventory, not how many bosses have actually been defeated. This was done to prevent a situation where you're forced into an unnecessarily long post-game. That might be weird to hear if you're not used to the logistics of multiworld randomizers, but trust me on this one, it prevents a lot of headache.

### I got softlocked in Outskirts/Hedgeward Arena/Rootden/some weird geometry.
There's a button added for the randomizer that automatically resets your save position to Lost Swamp. It's in your pause menu, at the top of the screen. Use this any time you get stuck somewhere (or you just really wanna fast travel back to the beginning of the game).

### Where did my old saves go?!
The Frogmonster client pulls from a different bank of save files than the base game does. This prevents accidental overwriting of data and the corruption of your base game saves. If you would like to play the base game again, go back to the Steam betas and re-select the main branch, and they'll come back.

# Important things to know about Archipelago
- In case it isn't clear by this point, Archipelago supports randomization of a LOT of different game titles, and organically allows you to randomize your items between different games. The main Archipelago repository supports somewhere in the ballpark of 70 unique titles, and there's dozens more in various beta stages of development (like this one!). You can find these beta games in the future-game-design forum on the official Archipelago Discord server (link available on their website).

- If you'd like to be able to see items sent between other players in your game, use Archipelago's built-in hinting system, change your slot name, or do a handful of other cool Archipelago functions that the Frogmonster client does not currently support, you can also connect to your slot with the Archipelago Text Client (included in the Archipelago installation, link above).

- Archipelago game rooms hosted on archipelago.gg automatically go to sleep after about 2 hours of inactivity. If you suddenly cannot connect, this is probably why. To wake the room up, simply click on the room link and wait about 30 seconds for the room to spin back up. The port number may change during this process, so double check it if you are having issues connecting. Don't worry, your progress is saved!

- If for some reason you lose your room link, you can find it on archipelago.gg under the header "User Content". This data is tied to your browser cookies, so if you switch devices or clear your cookies, you may permanently lose the room. 

- For solo or LAN Archipelago play, you can also localhost your room server instead of uploading to archipelago.gg. Use the Host button in the Archipelago Launcher for this.
