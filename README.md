# SailingComputer
This is the Taylor Sailing Sailing Computer repository.
This project, which may span several years, is to explore some possiblities for making sailing racing computer sytsems more accessible, easier to mount, and compatibile with existing marine electronics and marine web/cloud services.
The sequence is as follows:
1: setup the STMCubeIDE and STMCubeMX integrated development environment.
2: outline the high level requirements.
3: setup the Nucleo-F303RE or -F401RE (the hardware system is not too important - these are the dev kits I have available).
4: develop the code for an LCD display - I am using a 1602 LCD (16 characters x 2 lines) and interfacing with I2C (the LCD I have came with a serial to parallel PCB8574 IC that communicates with the STM32F303 via I2C). This method allows for me to use various LCDs with different row/column configurations but stay with a simple I2C interface and reduce GPIO requirements on the microcontroller.
4a: create a simple UI/UX on the display so that I know if the GPS and system are working - the display is not going to be visible during operation.
5: develop the code to interface with an RTK GPS module (with compass?).
6: develop the code to store the GPS and compass data on a microSD card.
7: put everything in a waterproof box, with a rechargable battery, and test on the water while sailing.
8: if successful, develop the code to add Bluetooth connectivity from the system to an iOS app.
9: develop a simple iOS app to show the GPS data while sailing.
10: add to the UI/UX the ability to show heading and speed while sailing.
