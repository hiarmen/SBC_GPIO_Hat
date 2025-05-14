# SBC_hat
SBC Flight Companion PCB Hat
GPIO PCB Hat design to be used on slim form factor SBC such as Pi Zero family. 
The architecture is: 
VIDEO Signal: [Analog cam]->[AV2USB converter]->[SBC processing]->[HDMI2AV converter]->[FC Video-in] 
UART: [SBC GPIO UART GND/Rx/Tx]->[FC UART GND/Tx/Rx] 
The Hat makes possible to add functionality to Betaflight/iNav based FC such as: autopilot/visual AI etc, based on the software you deploy on SBC.
