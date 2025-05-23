# SBC_GPIO_Hat

1. GPIO PCB Hat design to be used on slim form factor SBC such as Pi Zero family.<br> 
<u>The <b>HDMI</b> architecture:</u><br> 
- VIDEO Signal: [Analog cam]->[AV2USB converter]->[SBC processing]->[HDMI2AV converter]->[FC Video-in] <br>
- UART: [SBC GPIO UART GND/Rx/Tx]->[FC UART GND/Tx/Rx] <br>
The Hat makes possible to add functionality to Betaflight/iNav based FC such as: autopilot/MCP override/visual AI etc [based on the software you deploy on SBC].
<img width="1426" alt="Git-1" src="https://github.com/user-attachments/assets/9323dd50-2cdb-41dd-a0d4-35c062cf9761" />
<img width="1346" alt="Git-2" src="https://github.com/user-attachments/assets/e13ba533-d870-47a3-937d-d5ce8fe62537" /><br>

2. GPIO PCB Hat design to be used on slim form factor SBC such as Pi Zero family.<br> 
The <b>PARALLEL<b> architecture:<br> 
- VIDEO Signal: [Analog cam]->[AV2USB converter]->[SBC processing]->[HDMI2AV converter]->[FC Video-in] <br>
- UART: [SBC GPIO UART GND/Rx/Tx]->[FC UART GND/Tx/Rx] <br>
           +-------------------+
           |    Analog Camera  |
           +-------------------+
              |    |    |
              |    |    +----▶ GND ───▶ FC GND + USB Grabber GND
              |    +<--------- 5V  <─── FC CAM VCC [or SBC VCC]
              |
              └────▶ VIDEO OUT (YELLOW)
                       |
                       +----▶ FC CAM IN
                       |
                       +----▶ USB Grabber RCA (Video In) ---> SBC USB IN
  
<img width="520" alt="image" src="https://github.com/user-attachments/assets/ba134549-7210-4e47-971a-9a1daab1ecb4" />
