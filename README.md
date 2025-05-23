# SBC_GPIO_Hat

1. GPIO PCB Hat design to be used on slim form factor SBC such as Pi Zero family.<br> 
The HDMI architecture:<br> 
- VIDEO Signal: [Analog cam]->[AV2USB converter]->[SBC processing]->[HDMI2AV converter]->[FC Video-in] <br>
- UART: [SBC GPIO UART GND/Rx/Tx]->[FC UART GND/Tx/Rx] <br>
The Hat makes possible to add functionality to Betaflight/iNav based FC such as: autopilot/MCP override/visual AI etc [based on the software you deploy on SBC].
<img width="1426" alt="Git-1" src="https://github.com/user-attachments/assets/9323dd50-2cdb-41dd-a0d4-35c062cf9761" />
<img width="1346" alt="Git-2" src="https://github.com/user-attachments/assets/e13ba533-d870-47a3-937d-d5ce8fe62537" /><br>

2. GPIO PCB Hat design to be used on slim form factor SBC such as Pi Zero family.<br> 
The PARALLEL architecture:<br> 
- VIDEO Signal: [Analog cam]->[AV2USB converter]->[SBC processing]->[HDMI2AV converter]->[FC Video-in] <br>
- UART: [SBC GPIO UART GND/Rx/Tx]->[FC UART GND/Tx/Rx] <br>
 +-------------------+
           |   Ratel Pro Cam   |
           +-------------------+
              |    |    |
              |    |    +----▶ GND ───▶ FC GND + USB Grabber GND
              |    +---------▶ 5V ───▶ FC CAM VCC
              |
              └────▶ VIDEO OUT (YELLOW)
                       |
                       +----▶ FC CAM IN
                       |
                       +----▶ USB Grabber RCA (Video In)
![image](https://github.com/user-attachments/assets/0d01c2ca-f49f-4da0-b7fa-344a3c75c09d)
