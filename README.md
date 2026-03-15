# Laser CNC  


Using klipper, SV06, and RPI Pico.
(Pico for PWM control, with mosfet for logic level at 5V)

Tested with Arduino Mega.  
Max micro steps was 3.  
Was crashing if the microsteps on the 2y motors were set higher than 3.  

Swapped to testing on a SVO6 printer. Working well.

Laser cable was most likely incorrect. Tested before using.
Tested driver seems the labels on the module are correct. 

Does not logically match the cable.
The cable has two PWM wires 1 black 1 yellow which are tied in the 3 pin laser input. 
Black(PWM) and red(+) are both connected to a JST style connector.
White(-) and yellow(PWM) are broken off.


TODO:
- [ ] Add a distance sensor the the pico that will trigger a endstop.
