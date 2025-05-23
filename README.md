# SBC_GPIO_Hat

1. GPIO PCB Hat design to be used on slim form factor SBC such as Pi Zero family.<br> 
<u>The <b>HDMI</b> architecture:</u><br> 
- VIDEO Signal: [Analog cam]->[AV2USB converter]->[SBC processing]->[HDMI2AV converter]->[FC Video-in] <br>
- UART: [SBC GPIO UART GND/Rx/Tx]->[FC UART GND/Tx/Rx] <br>
The Hat makes possible to add functionality to Betaflight/iNav based FC such as: autopilot/MCP override/visual AI etc [based on the software you deploy on SBC].
<img width="1426" alt="Git-1" src="https://github.com/user-attachments/assets/9323dd50-2cdb-41dd-a0d4-35c062cf9761" />
<img width="1346" alt="Git-2" src="https://github.com/user-attachments/assets/e13ba533-d870-47a3-937d-d5ce8fe62537" /><br><br>

2. GPIO PCB Hat design to be used on slim form factor SBC such as Pi Zero family.<br> 
The <b>PARALLEL<b> architecture:<br> 
- VIDEO Signal: [Analog cam]->[FC Video-in]->[AV2USB converter]->[SBC processing]-> <br>
- UART: [SBC GPIO UART GND/Rx/Tx]->[FC UART GND/Tx/Rx] <br>

  
<img width="520" alt="image" src="https://github.com/user-attachments/assets/ba134549-7210-4e47-971a-9a1daab1ecb4" /><br><br>
The key difference between these two methods:<br>
1. HDMI version: worked with HDMI display, but did not work well with FC OSD. Probably FC not compatible HDMI module. Got flickering video feed on goggles.<br>
2. PARALLEL version: direct video feed from camera, yet allows SBC to implement functions over MSP. More reliable, however functions are not reflected on OSD.
