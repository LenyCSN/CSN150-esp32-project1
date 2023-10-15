# CSN150 Lab: ESP32-NAT_Router_LC
## Objective: Create an ESP32 Router using our inexpensive ESP32CAM.
### Equipment:
1. [ESP32CAM Amazon link](https://www.google.com](https://www.amazon.com/Aideepen-ESP32-CAM-Bluetooth-ESP32-CAM-MB-Arduino/dp/B08P2578LV/ref=sr_1_3?crid=4FY0ECFW0ZX7&keywords=ESP32+Cam&qid=1678902050&sprefix=esp32+cam%2Caps%2C240&sr=8-3)https://www.amazon.com/Aideepen-ESP32-CAM-Bluetooth-ESP32-CAM-MB-Arduino/dp/B08P2578LV/ref=sr_1_3?crid=4FY0ECFW0ZX7&keywords=ESP32+Cam&qid=1678902050&sprefix=esp32+cam%2Caps%2C240&sr=8-3)
2. [USB Micro Data Cable Amazon link](https://www.amazon.com/AmazonBasics-Male-Micro-Cable-Black/dp/B0711PVX6Z/ref=sr_1_1_sspa?keywords=micro%2Busb%2Bdata%2Bcable&qid=1678902214&sprefix=Micro%2BUSB%2Bdata%2B%2Caps%2C89&sr=8-1-spons&spLa=ZW5jcnlwdGVkUXVhbGlmaWVyPUFaU0NaUVZHU1RFUlAmZW5jcnlwdGVkSWQ9QTA3NTA4MDVFVERCS01HVlgxM1YmZW5jcnlwdGVkQWRJZD1BMDE4NTE1NTIwWUdONkdWSzU1M1Amd2lkZ2V0TmFtZT1zcF9hdGYmYWN0aW9uPWNsaWNrUmVkaXJlY3QmZG9Ob3RMb2dDbGljaz10cnVl&th=1)

---

### Documentation Links (operating on a Windows 11 machine):
1. https://github.com/martin-ger/esp32_nat_router

2. [Expressif ESP32 flashing tool link](https://www.espressif.com/en/support/download/other-tools)

3. "How to Make a WiFi Repeater using ESP32 NodeMCU | WiFi Router Range Extender esp32 esp8266 | 2022"

Youtube Video: https://www.youtube.com/watch?v=BP1Dz66faf4

4. "ESP32 as a Wifi Range Extender" (similar to the video above but uses the updated expressive flash tool)

Youtube Video: https://www.youtube.com/watch?v=LvhhCDjHnGk&t

---

### Steps Followed:
1. I downloaded the zip file from documentation 1 and unzipped the file.
2. I downloaded the zip file from documentation 2 under "Flash Download Tools" (Windows PC V3.9.5 for my machine) and unzipped the file.
3. Run the Flash Download Tool from step 2 that's inside the folder.
4. Following Documentation 3 and 4 (similar information), select ChipType "ESP32" and WorkMode as "Develop".
5. Load the bootloader from documentation 1 folder under "esp32_nat_router-master" and under "build" > "esp32" > you see 3 .bin files; "bootloader.bin", "firmware.bin", "partitions.bin".
6.  Load the "firmware.bin".
7.  Load the "partitions.bin".
8.  Type the correct hex location numbers; "bootloader.bin" = 0x1000, "firmware.bin" = 0x10000, "partitions.bin" = 0x8000.
9.  Plug in the ESP32 (ensure your drivers are correct if this is your first time using esp32) and identify which port your esp32 is plugged into. Select the port on the bottom right and set BAUD rate to 115200.
10.  Start the flash tool (you may need to put esp32 in flashing mode, refer to documentation 3-4).
11.  Now unplug and plug in your esp32 to reset.
12.  On your PC's internet settings, you should see the esp32 appear shortly (disconnect from any ethernet connections at this time). Connect to the esp32.
13.  Connect into the esp32 by opening your browser and typing "192.168.4.1"
14.  Configure your esp32 router accordingly based on your prefrences as described by documentation 3-4.

---

### Problems Encoutered:
1. 

