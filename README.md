# Avante53
Open-source 53 keys alice-style ortho keyboard. Features hotswap switches, a rotary encoder, and OLED screen.

## Bill of materials
- 53 Hotswap sockets
  - https://www.aliexpress.com/item/4001051840976.html
- 54 SMD 1N4148 diodes
  - https://www.aliexpress.com/item/32849879904.html
- Teensy 2.0 microcontroller
  - https://www.aliexpress.com/item/4000829915634.html
- a rotary encoder
  - https://www.aliexpress.com/item/10000056483250.html (the 15mm half handle)
- 11x 5mm m2 standoffs
  - https://www.aliexpress.com/item/1005004564012666.html
- 11x m2 nuts
- 11x short m2 screws (8-10mm)
- 53 switches of your choice
- any set of preonic/ortho keycaps
  - I used https://www.aliexpress.com/item/1005003294964787.html
- recommended: a 3d printer for the case and plate
- optional: 128x32 OLED screen breakout board
  - https://www.aliexpress.com/item/32850288143.html
- optional: a very short ws2812b led strip (like 5 leds)
  - https://www.aliexpress.com/item/2036819167.html

## Building
It's pretty straightforward.
- get the PCB printed at JLCPCB or your supplier of choice.
- solder the teensy on the underside with its header pins.
- solder the diodes and hotswap sockets.
- solder the encoder and oled screen on the top side of the board.
- print the case, and punch open the screw holes. If you printed the 2 separate pieces, put them on a flat surface like glass, and glue them together with super glue.
- push the nuts in the holes from the bottom, and screw in the standoffs.
- put the PCB in the case and screw it in.
- print the plate and install it along with the switches.
- done!

## Flashing
You can clone my fork of vial (https://github.com/Pimentoso/vial-qmk) and compile the keymap for this keyboard with `make pimentoso/avante53:vial`
Or you can just flash the compiled binary you can find in the `firmware` folder, using QMK toolbox or a tool of your choice.
Then you can use vial to edit the keymap.
