# Catalysm-CSGO-config

# DPI: 800
# In-game mouse sens: 1.5

Autoexec for Counter Strike Global Offensive (CSGO) including scripts and binds.

**This includes my personal controls! Make sure to delete these lines or change them to yours because you will lose your current settings.**

The best thing to do is look at everything in this repo and copy what you want to your own autoexec.

## What is an autoexec?

An autoexec (automatic execute) is a config file which will run every time you start CSGO. This has multiple benefits

- More possibilities than the ingame settings menu because you are not limited to what Valve provides ingame.
- A backup of your configuration for when you get a new PC or you have to play on a different machine.

An autoexec can have as many (or as little) settings as you want. In this project I have split it up into different files for improved readability and to make it easier to find the settings you want.

## Features

* Assorted scripts bound to function keys
* Buy binds on numpad and arrow keys. (run `exec autoexec` ingame and it will echo the settings to your console)
* Sensible defaults for network, video and viewmodel.
* Displays damage done when you die. Will display at top left of your screen.
* Radar zoom in and out buttons
* Volume up/down buttons. To control ingame volume without changing your Windows volume.
* Show netgraph when holding TAB
* Friends can join your community server without an invite
* Disable automatic weapon switch on pickup
* Mute all music except the 10 second bomb timer
* Customized radio menu

## Installation

  Copy the csgo folder of this repo to the one in your csgo installation. When asked to overwrite, answer yes.
  
  `C:\Program Files (x86)\Steam\steamapps\common\Counter-Strike Global Offensive\csgo\cfg`
  
  It will automatically execute all commands when you start your game. 
  If you're having trouble you can reload the script by writing `exec autoexec` to console.

## For Teleports to work, run this as Admin
`mklink "C:\Program Files (x86)\Steam\steamapps\common\Counter-Strike Global Offensive\csgo\cfg\position.cfg" "C:\Program Files (x86)\Steam\steamapps\common\Counter-Strike Global Offensive\csgo\position.log"`

## Scripts

* **F1 - buy drop script**
  
Buys an AK/M4 and drops it.

* **F2 - find the bomb script**

Enables the noob-tips. This will show a tooltip above the bomb, useful for finding it inside a smoke.

* **F3 - Crosshair changing script**

Cycles through crosshairs. See the misc file to configure your own crosshair(s).

* **F4 - Toggles voice chat on/off.**

Very useful to mute cyka blyat teammates during clutches.

* **F5 - Rapid fire**

Toggles rapid fire mode. This will rebind your mousewheel to shooting. Combine this with dualies/tec-9 for maximum power.

* **F6 - sm_admin**

Opens the SourceMod admin menu.

* **F7 - Pro mode**

Inspect your weapon everytime you shoot. Because lol.

* **F8 - /**

* **F9 - noclip**

Toggle noclip

* **F10 - /**

* **F11 - disconnect**

Instantly disconnects you from current server

* **F12 - Quit prompt**

Shows the quit prompt. 

## Aliases

* Play aim_botz or recoil training while waiting for MM queue
* Nade training mode

## Radio menu commands

The radio menus have been customized with commands and scripts. The 10 man commands are from [Splewis Pug Setup](https://github.com/splewis/csgo-pug-setup)

![Radio client](img/radio_client.png)
![Radio bot](img/radio_bot.png)
![Radio 10man](img/radio_10man.png)
![Radio training](img/radio_training.png)


## Other controls

These are located in cata-controls.cfg. Change to your desired keys

* v - Clear all blood and bullet holes from the map for better visibility
* f - Toggles weapon between left and right hand, I use this to hold certain angles better where your gun could block vision
* o - Tell a bot to hold his position
* Page up/down - ingame volume buttons
* End/home - Zoom radar in or out
* Space - jump throw
* left alt - crouch + jump at the same time, this is just about the highest you can jump.
* delete/insert - +right and +left

### Text binds

Located in cata-text.cfg

* L - trashtalker. Will display a new message every time you press L
* k -  ¯\\_(ツ)_/¯
* m - xD
* p - What do you mean
* I - Navy seal copypasta

## Support

[Make an issue on Github](https://github.com/niekcandaele/Catalysm-CSGO-config/issues/new).

### What if the autoexec is not running on startup?

This can have multiple causes and luckily there's a couple of fixes!

- Manually execute the config from inside the game
  
  To do this, you open up your console and execute this command `exec autoexec`. If you are using the config files in this repo, you will see info about loaded scripts, buy binds and other controls.

  If you do this you please make sure you run the command again every time you make changes to your autoexec.

- Add the command `exec autoexec` to you config.cfg

  config.cfg is always executed on start, by adding this command to it you can make sure the autoexec is executed straight after

- Add `+exec autoexec` to the launch options of CSGO

# Credits

I took a lot of info from other configs. Check those out aswell!

- [/u/birkir](https://www.reddit.com/r/GlobalOffensive/comments/8ax858/updated_csgo_tips_configs_and_more/)
- [rwwrou](https://github.com/rwwrou/yuki.cfg)
- [KYSO](https://www.youtube.com/watch?v=l7gE8RjuJB8)

# Disclaimer

Please don't blindly copy and paste, it WILL override your settings (controls, binds, crosshair, viewmodel). Delete what you don't want or change to your own values! Be careful when using the jump throw script! It is banned on ESEA (and possibly other services aswell). Do your own research to make sure!
