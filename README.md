# Ricoh-Toner-Chip-Reset
A program for an Arduino Nano to recognise Ricoh Toner Chips and reset the page count when refilling.
I am using an Arduino Nano, with a NANO3 Expansion PCB:- https://www.aliexpress.com/item/1005005764189363.html
and a 6 way PCB Edge Connector, with connector 1 and 6 removed. 
![image](https://github.com/user-attachments/assets/0aeef62e-ab1b-42d4-b549-38ffdb52ecce)

The PCB edgeconnector is ok for inserting the Ricoh Toner Chips and allows connection of :
left most pad = 1.
rightmost pad = 4.

1 = SCL = A5

2 = SDA = A4

3 = 5v  = VCC

4 = GND = GND

Place the toner chip in the edge connector. Connect the Nano to your Computer. Use any serial terminal app
connected to the USB port @ 115200 baud. The progrtam will test the I2C bus to see if there is a Toner chip
connected. If not it willtell you on the terminal. If it finds a valid I2C device at one of the four possible
addresses it will load the appropriate reset data into the chip and tell you it has done so.

![IMG20250104151519](https://github.com/user-attachments/assets/b78da8a4-ad39-4448-9b42-b4ca0cab23c5)
![IMG20250104151534](https://github.com/user-attachments/assets/defc87a6-9b91-4825-a5a4-cc07ed3d2777)


