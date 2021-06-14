# Window-discriminator

# The window discriminator is only a voltage comparator with not only one voltage level, but two voltage levels. If you for example chose 0.7V and 3.3V levels, if you will be in between this range of voltages you can do something, if not do something else.

# I created this as if i´m in the range it goes to the OR gate (7432) and INV (7404 - the output of the OPAmp is low in between) and it lights one LED - and so on for other three voltage windows. If all four windows are activated (leds are glowing), i added 4NAND (7420) and INV to count all the on outputs and multiply them together = if all of them are on, the output will be on too, so the fifth LED is glowing too - it signals that all windows are acitve.

# If i´m not in the range the the LEDs are not glowing.

# My motivation for doing this relatively "complicated" circuit was the fact that i saw the TCA965B chip (originaly designed to be a window comparator), but its not available for me, so i said to my self, hey let´s create something at least something similar to it.

# It has some mistake, as the biggest one (not destructing but on the top of what the ICs can hold) i see that id didnt gave any 5.1V zener diodes after the outputs of the LM324, second is due to big supp voltage (20V) the LM324 is geting hot (again, not destructive, but to the limits)

# The schematic is available to all of you (as well as the rest of the zip file), but you can create your own and better schematic/PCB.

# Thank you.
