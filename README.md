# Pokemon auto-script hex files

## Introduction

These are generated hex files for the pokemon auto script I have been developing, which can be found [here](https://github.com/ironandstee1/pkmn-auto-hatcher).

This repository is meant for users to be able to download and flash their boards with the software without having to go through the trouble of installing a bunch of programs and building the code. 

## Requirements

Either

* [Teensy++ 2.0](https://www.pjrc.com/store/teensypp.html)
  * Available on amazon
* [Teensy Loader](https://www.pjrc.com/teensy/loader.html)
  * This is available on Windows, Linux, and OSX
  * The install is painless. Just follow his instructions
  
or 

* [Pro micro/leonardo](https://www.amazon.com/KeeYees-ATmega32U4-Development-Microcontroller-Bootloader/dp/B07FXCTVQP/ref=sr_1_3?keywords=pro+micro&qid=1580795971&sr=8-3)
 * Code is still being optimized - only watt farm, box release, and 2560 multi hatch are currently supported
 * Support will be added for the rest of the scripts over the next two weeks
 * Arduino Uno (Atmega16U2) can also be used but has limited compatibility

  
## How to flash the software 

Note: Find out the appropriate egg steps for your pokemon [here](https://bulbapedia.bulbagarden.net/wiki/Egg_cycle) and download the appropriate hex. My script uses base egg steps, but the script depends on having a pokemon with flame body in your party. Not all the scripts are hatch scripts. 

1. Download and run the Teensy Loader program or download and run the [QMK Toolbox](https://github.com/qmk/qmk_toolbox/releases/download/0.0.16/qmk_toolbox.exe). For QMK (recommended for Leonardos) you may also need to download avr dude or some other software. If it gives you errors, google them and it will tell you what you are missing. 
1. Download [this repo](https://github.com/ironandstee1/pkmn-hexes) by clicking "Clone or Download" and selecting Download as Zip
1. Unzip the files using winrar or another similar program
1. Determine which hex file you want from the list above
1. Teensy
 * Plug your teensy into your computer
 * Press the white button on the Teensy. It should now load in the Teensy Loader program
 * Press the black list button and navigate to the hex file 
 * Select the hex file and click program (green arrow going into hole)
 * Wait for programming to complete
 * Unplug teensy from the computer
1. Pro micro/leonardo 
 * Start the program
 * Click the open button and select your hex file
 * Plug your board in and connect the RST to GND twice quickly 
 * Click the flash button 
1. Disconnect all your switch controllers
1. Plug your board into one of the USB ports on the switch dock

## In game requirements
1. [Pokemon with flame body](https://www.serebii.net/abilitydex/flamebody.shtml) - This is required for all hatching scripts. I use a Carkoal that I caught on the mine tracks. 
1. [Oval charm](https://bulbapedia.bulbagarden.net/wiki/Oval_Charm) - This is required for all the hatching scripts. If you don't have this item you may not get the eggs fast enough. I believe it requires completing the game, visiting Circhester, and defeating Morimoto in a hotel.
1. [Masuda Method](https://bulbapedia.bulbagarden.net/wiki/Masuda_method) - This is pretty necessary for all hatching scripts. Foreign ditto/foreign breeding partner. A ditto is best because it can be used for any pokemon, but in a pinch, use any foreign pokemon with a normal ditto. If you don't have a foreign pokemon, surprise trade until you get one. Using hatch scripts without Masuda method is a huge waste of time. 
1. Box space - Make sure you have quite a few free boxes. You can get >30 pokemon per hour with one of these scripts. 
1. If you are performing the watt farm, you need to perform [this exploit](https://www.youtube.com/watch?v=CUTpProiDwU) first. 

## In-game script instructions

### Automatic hatch scripts

* 10240: 10 minute runtime/up to 5 eggs
* 7640: 8 minute runtime/up to 4 eggs

1. Place your ditto and breeding partner in the Route 5 nursery
1. Make sure you have 6 pokemon in your party and no eggs when starting this script
1. Bike around until the nursery person has an egg ready (arms crossed)
1. Open up the town map and warp to Route 5
1. Get off your bike and disconnect all controllers
1. Plug in your board

### Single hatch scripts

1. Place your ditto and breeding partner in the Route 5 nursery
1. Make sure you have 6 pokemon in your party and no eggs when starting this script
1. Bike around until the nursery person has an egg ready (arms crossed)
1. Open up the town map and warp to Route 5
1. Get off your bike and disconnect all controllers
1. Plug in your programmed teensy (see "How to use the software")

The scripts should take anywhere from 2-5 minutes to complete. All of these scripts have been tested to run indefinitely as long as you have box room.

### 5 Box release script

1. Set up all the pokemon you want to release in 5 consecutive boxes. If you have less, leave the box after empty
1. Go to the box before the first box and make sure there is a pokemon in spot 1 column 1 (this pokemon will not be released)
1. Place your selector on the first pokemon in the first box you want to release
1. Ensure you're on single select (red option)
1. Disconnect all controllers
1. Plug in your board

When the script is finished it will just repeatedly press b. Just disconnect your board.

### Watt farm script

1. Set your date to 1/1/2000

1. Perform the exploit linked above

1. Set your date to 1/1/2001

1. Make sure you are standing in front of the den while it has the beam but grey (no watts)

1. Unplug your controller

1. Plug in your board



## Thanks

Thanks to Shiny Quagsire for his [Splatoon post printer](https://github.com/shinyquagsire23/Switch-Fightstick) and progmem for his [original discovery](https://github.com/progmem/Switch-Fightstick).

Thanks to [bertrandom](https://github.com/bertrandom/snowball-thrower/) the foundation of this script/method.

Thanks as well to all other contributors to previous projects.
