# Frogmonster Randomizer Setup Guide

This guide presumes you've never used Archipelago before. If you know the basics, skip to [Client Setup](#Client Setup) for the new stuff.

# Choose your Settings
Download `Frogmonster.yaml` from this repository and name it something unique. Open it up in a text editor of your choice. Give yourself a player name, and choose options according to your liking. (Settings which give you multiple options are written as weighted choices (50 or 0) by default. Writing them out unweighted like `game_difficulty: normal` is perfectly OK too.) Consider running your YAML through a YAML linter to make sure that you didn't break YAML formatting accidentally.

# Generating a Game

## I'm playing alone, or I'm hosting the room:
Download the following:
1. `frogmonster.apworld` (found here)
2. [Archipelago.](https://github.com/ArchipelagoMW/Archipelago/releases/latest).

Open the folder where Archipelago was installed. Place `frogmonster.apworld` in the folder `\custom_worlds`, and place your YAML file in `\Players`. If there are other players in your multiworld, they will sent you their YAMLs as well, which you will also place in `\Players`. 

Optionally, you can open the `host.yaml` file and adjust some generation settings if you'd like. The defaults are fine if you're new to Archipelago, though.

Once you've got all the player YAMLs, open Archipelago, and click "Generate". If everything works correctly, a zip folder will appear in your `\outputs` folder. Go to [archipelago.gg](https://archipelago.gg) and click "Host Game". Upload that .zip file to create a room. Share this room link with any other players.

If you're having issues with the generation process, ask around. Consider providing the generation logs from your most recent attempts (found in `\logs`) as well as the YAML files used in generation.

## I'm not hosting the room:
Send your completed settings YAML to the room host. Make sure they also have a copy of the `frogmonster.apworld` file (they can download it here, or you can send it to them). Eventually, the host will send you a room link.

# Client Setup
Remind me to write this later once we get this figured out on our end. Oops!

# Cool Things to know about Archipelago
Remind me to do this too.