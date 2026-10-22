# starbie
a fun  little pet !

starbie isa cute fun little  interactive digital pet
this project includes a custom digital pet - which i named LEgoat

starbie uses parts such as esp32-c3 , switches , resistor , MPU6050 module ,an oled screen and a DHT11 sensor.

# What does starbie do:
Starbie is a cute interactive desk pet that reacts to you and your surroundings.
it is a small digital pet (LEgoat) that has 2 buttons and mpu6050 module , the mpu6050 module helps it make reactive to tilting and shaking .


![image alt]( https://github.com/AlteranteTony/starbie/blob/2ed99856e868ce408fd0646d3987f0d527796926/sch1.png)

what is in the repo
- starbie.ino this includes the code
-BOM.md it contins bill of materials
-journal.md contains journal that i wrote while working on starbie
-project file - pcb layout , circuit design
-production 1 contains files for fabrication of pcb


## Tech stack
- kicad
- c++
- arduino ide

how to set up firmware ( use arduino ide)
-open the firmware folder. install listed libraries now select xiao esp32 c3 board and the correct port and upload the code. after that you are basically good to go.

## How to Use starbie

### Controls

- Button 1 =it  Opens the action menu and confirms a selected action.
- Button 2 = Toggles the stats screen.
- Shake = Give LEgoat a small joy boost.

### Actions
the stabie has actions like nap , play , feed ,pet . pet action makes LEgoat jump and show hearts. when you use Feed it gains fullness . when using play runs around the screen and gains joy . Nap it goes to sleep.

Stats range from 0 to 100 

### Sensors use in project

The MPU6050 detects movement and controls the action menu. The DHT11 measures temperature and humidity, which are displayed on the stats screen.


YOU CAN CUSTOMIZE THE PET IF YOU WANT !!

PCB WAS CHECKED FOR ERRORS USING KI CAD'S DRC. CHECK PCB FOR ERROR BEFORE MANUFACTURING THE PCB 


FINAL LOOK FOR PCB

![image alt](https://github.com/AlteranteTony/starbie/blob/653a51dd401e3277d5c9f7e93e20e1d4f9f48382/pcb1.png)


3D render of PCB
![image alt](https://github.com/AlteranteTony/starbie/blob/40dc25fa13a34689987a8b8a6f80386a0d33baa0/3d%20render1.png)

## Bill of Materials (BOM)

The following components are used to build Starbie.

| Designator | Footprint | Quantity | Value | vendor name | Unit Price ($) | Line Total ($) | Link |
|---|---|---:|---|---|---:|---:|---|
| J1 | Display_128x64_096_I2C | 1 | Conn_01x04_Pin | Sharvi electronics | 2.17 | 2.17 | https://sharvielectronics.com/product/0-96-inch-i2c-4pin-oled-display-module-white/ |
| J2 | MPU6050_Module | 1 | Conn_01x08_Pin | Sharvi electronics | 1.95 | 1.95 | https://sharvielectronics.com/product/mpu-6050-3-axis-accelerometer-and-gyro-sensor/ |
| R1 | R_Axial_DIN0207_L6.3mm_D2.5mm_P7.62mm_Horizontal | 1 | 10K | Sharvi electronics | 0.26 | 0.26 | https://sharvielectronics.com/product/10k-ohm-1-2-watt-resistor-1-tolerance/ |
| SW1, SW2 | SW_Cherry_MX_1.00u_PCB | 2 | SW_Push | Sunrom electronics | 1.2 | 2.40 | https://www.sunrom.com/m/6479 |
| U1 | XIAO-ESP32-C6-DIP | 1 | XIAO-ESP32-C3-SMD | Sharvi electronics | 6.56 | 6.56 | https://sharvielectronics.com/product/seeed-studio-xiao-esp32c3-tiny-mcu-board-with-wifi-and-ble-battery-charge-supported-module/ |
| U2 | Aosong_DHT11_5.5x12.0_P2.54mm | 1 | DHT11 | Sharvi electronics | 0.71 | 0.71 | https://sharvielectronics.com/product/dht11-temperature-and-humidity-sensor-module/ |
| N/A | PCB | 1 | - | JLCPCB | 10 | 10 | https://jlcpcb.com/ |
| | | | | TOTAL= | $24.5 | | |

*Prices are estimates and may change. Shipping, taxes, and other charges may not be included.*

