# Pokemon auto-script hex files

## Introduction

These are generated hex files for the pokemon auto script I have been developing, which an be found [here](https://github.com/ironandstee1/pkmn-auto-hatcher).

This repository is meant for users to be able to download and flash their boards with the software without having to go through the trouble of installing a bunch of programs and building the code. 

## Requirements

* [Teensy++ 2.0](https://www.pjrc.com/store/teensypp.html)
  * If these boards are out, reach out to the developer or check on alternate websites
  * The code is only currently available for this board
* [Teensy Loader](https://www.pjrc.com/teensy/loader.html)
  * This is available on Windows, Linux, and OSX
  * The install is painless. Just follow his instructions
  
## How to use the software

Note: When I say egg steps I am referring to base egg steps. So 2560 for Morpeko, 5120 for Scorbunny, etc

1. Download and run the Teensy Loader program
1. Download your chosen hex file
  * [Single hatch for 2560 base egg steps](http://google.com) - find out your pokemon's egg steps [here](https://bulbapedia.bulbagarden.net/wiki/Egg_cycle)
  * [Single hatch for 3840 base egg steps](http://google.com) - find out your pokemon's egg steps [here](https://bulbapedia.bulbagarden.net/wiki/Egg_cycle)
  * [Single hatch for 5120 base egg steps](http://google.com) - find out your pokemon's egg steps [here](https://bulbapedia.bulbagarden.net/wiki/Egg_cycle)
  * [5 box release](http://google.com)
  * [Surprise Trade](http://google.com) (in development)
  * [Link trade](http://google.com) (in development)
  
1. Plug your Teensy into your computer
1. Press the white button on the Teensy. It should now load in the Teensy Loader program
1. Press the black list button and navigate to the hex file 
1. Select the hex file and click program (green arrow going into hole)
1. Wait for programming to complete
1. Unplug this from the computer
1. Disconnect all your switch controllers
1. Stick your teensy into one of the USB ports on the switch dock

## In game requirements
1. [Pokemon with flame body](https://www.serebii.net/abilitydex/flamebody.shtml) - This is required for all hatching scripts. I use a Carkoal that I caught on the mine tracks. 
1. [Oval charm](https://bulbapedia.bulbagarden.net/wiki/Oval_Charm) - This is required for all the hatching scripts. If you don't have this item you may not get the eggs fast enough. I believe it requires completing the game, visiting Circhester, and defeating Morimoto in a hotel.
1. [Masuda Method](https://bulbapedia.bulbagarden.net/wiki/Masuda_method) - This is pretty necessary for all hatching scripts. Foreign ditto/foreign breeding partner. A ditto is best because it can be used for any pokemon, but in a pinch, use any foreign pokemon with a normal ditto. If you don't have a foreign pokemon, surprise trade until you get one. Using hatch scripts without Masuda method is a huge waste of time. 
1. Box space - Make sure you have quite a few free boxes. You can get ~30 pokemon per hour with some of these scripts. 

## In-game script instructions

### Single hatch scripts ([2560](http://google.com), [3840](http://google.com), [5120](http://google.com))

1. Place your ditto and breeding partner in the Route 5 nursery
1. Make sure you have 6 pokemon in your party and no eggs when starting this script
1. Bike around until the nursery person has an egg ready (arms crossed)
1. Open up the town map and warp to Route 5
1. Get off your bike and disconnect all controllers
1. Plug in your programmed teensy (see "How to use software")

The scripts should take anywhere from 2-5 minutes to complete. All of these scripts have been tested to run indefinitely as long as you have box room.

### 5 Box release script

1. Set up all the pokemon you want to release in 5 consecutive boxes. If you have less, leave the box after empty
1. Go to the box before the first box and make sure there is a pokemon in spot 1 column 1 (this pokemon will not be released)
1. Place your selector on the first pokemon in the first box you want to release
1. Ensure you're on single select (red option)
1. Disconnect all controllers
1. Connect your teensy

When the script is finished it will pause indefinitely. Just disconnect your Teensy. If you have < 5  and followed my instrutions, it'll end up in the mark selection section, so there's not really risk here. 
