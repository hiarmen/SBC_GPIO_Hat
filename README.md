# SBC_GPIO_Hat

GPIO PCB Hat design to be used on slim form factor SBC such as Pi Zero family.<br> 
The architecture is:<br> 
- VIDEO Signal: [Analog cam]->[AV2USB converter]->[SBC processing]->[HDMI2AV converter]->[FC Video-in] <br>
- UART: [SBC GPIO UART GND/Rx/Tx]->[FC UART GND/Tx/Rx] <br>
The Hat makes possible to add functionality to Betaflight/iNav based FC such as: autopilot/MCP override/visual AI etc [based on the software you deploy on SBC].
![Git-1](https://github.com/user-attachments/assets/7255e00d-8126-4dff-8ffd-972b04431ecc)
<img width="1346" alt="Git-2" src="https://github.com/user-attachments/assets/e13ba533-d870-47a3-937d-d5ce8fe62537" />

