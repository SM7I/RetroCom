# RetroCom for ZXpand+ Super Serial card

ZX81 computers can also utilize the wonders of Internet if equipped with ZXpand+ interface by Charlie Robson (sirmorris).
By connecting the Super Serial card, which can be purchased by me, Internet is in reach. Simply connect the Super Serial card to your ZXpand+ using a 10 pin IDC cable. Default RS232 speed of ESP-01 is 1200 baud.

For the wifi to work you´ll have to update the firmware of your ZXpand+. Latest firmware can be found here: https://github.com/charlierobson/ZXpand-Vitamins#zxpand-vitamins 

The Super Serial card has the following features:
* ESP-01 industrial wifi module
* 5 pin DIN MIDI connector
* Joystick port

RetroCom client software is being developed as of now, but a terminal software is finished and can be downloaded. The ESP-01 module firmware is a fork of Zimodem CoCo version into which I have implemented some features of my own, AT+PING for example. Standard AT commands are obeyed by the module, but unfortunately the ZX81 does not have the ampersand (&) character so certain AT commands will not be possible to enter.

**Please note**: SSIDs are CaSe-sensitive. You can toggle CAPS mode on ZX81 by pressing GRAPHICS and then 9.

The other file in the repo, player2.p, is a MIDI file player which works very fine with the MIDI jack on the Super Serial Card connected to f.ex. Roland SC-55 which is a Sound Canvas MIDI sound module.
Syntax: RUN <<midifile>>   ***Don´t type in the .ZXM extension. Player will do this itself***
