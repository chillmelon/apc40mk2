# apc40mk2

CDJ-style looping control mapping for the APC40MKII ableton midi controller

## prerequisites

* ableton live 11 (only works with 11~)
* an APC40MKII controller

## installing

1. download apc40mk2_chillmelon.zip from https://github.com/chillmelon/apc40mk2/releases/latest
2. unzip it
3. copy the unzipped `apc40mkii_chillmelon` folder to your Ableton MIDI remote
   scripts directory using the instructions at
   https://help.ableton.com/hc/en-us/articles/209072009-Installing-Third-Party-Control-Surfaces.
   for instance on Mac with Ableton 11, this would be `/Applications/Ableton
   Live 11 Suite.app/Contents/App-Resources/MIDI Remote Scripts`.
4. open Ableton Preferences with your apc40mk2 plugged in and select `apc40mkii
   chillmelon` as the control surface.

## usage

the custom mappings are as follows. note that all clips must be warped for this
to work.

* `METRONOME` - sets the loop start point to the nearest bar of the current playing position. if already looping, this turns off looping.
* `TAP TEMPO` - sets loop end point to the nearest bar of the current playing position and engages looping.
* `NUDGE-` - moves entire loop left by a bar
* `NUDGE+` - moves entire loop right by a bar
* `SHIFT NUDGE-` - halves the loop length
* `SHIFT NUDGE+` - doubles the loop length. note: this will cause the play position to jump unnecessarily sometimes (i think this is an ableton bug)

## demo/tutorial made by Azuki

https://www.youtube.com/watch?v=YILKOWhN2ag

## credits

I just converted diracdeltas' code to work with Python 3 so it can work with Ableton Live 11. The python2 version that works with older Ableton Live can at https://github.com/diracdeltas/apc40mk2.
Thanks to will marshall for doing most of the work for LooperComponent in https://github.com/willrjmarshall/AbletonDJTemplateUnsupported.

## license

http://www.wtfpl.net/
