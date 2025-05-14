# SBC_GPIO_Hat

GPIO PCB Hat design to be used on slim form factor SBC such as Pi Zero family. 
The architecture is: 
VIDEO Signal: [Analog cam]->[AV2USB converter]->[SBC processing]->[HDMI2AV converter]->[FC Video-in] 
UART: [SBC GPIO UART GND/Rx/Tx]->[FC UART GND/Tx/Rx] 
The Hat makes possible to add functionality to Betaflight/iNav based FC such as: autopilot/visual AI etc, based on the software you deploy on SBC.
<img width="1430" alt="Git-1" src="https://github.com/user-attachments/assets/6be5660e-a38b-4bfa-9094-bb598695eb53" />
<img width="1346" alt="Git-2" src="https://github.com/user-attachments/assets/e13ba533-d870-47a3-937d-d5ce8fe62537" />

