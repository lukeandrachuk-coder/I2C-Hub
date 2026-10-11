The purpose of this project is to make a board that expands the number of I2C connective devices that you can connect to a microcontroller. The board was designed in KiCAD a free PCB design software. How it works is you connect the VCC, GND, SCL, and SDA from your microcontroller to the same ports in the I2C_In pins on the I2C hub board. You can then connect one or more of the eight out pins to your I2C devices.
<img width="602" height="418" alt="image" src="https://github.com/user-attachments/assets/3e37bec6-6fe9-4e05-bba2-6283e08d913f" />
**Assembly instructions: **
  First the TCA9546APWR chip needs to be soldered to the board. I recommend using solder paste for this as it is a surface-mount device. 

  Next solder the corresponding resistors in their places as well as the ceramic capacitor and LED. Lastly, solder the male pin headers into their spots. You should have nine 4-pin headers, and three 3-pin headers. 
  
  The 3-pin headers allow you to change the I2C address of the board based on which endpin you connect to the centre. One will pull it low (0), and the other will pull it high (1), letting you very the I2C address so it does not get confused with other I2C boards in code.
