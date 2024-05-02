Example Brief:
===================
This example demonstrates combining ISSDK and FreeMASTER to create FXLS89xxxF 3-axis accelerometer evaluation GUI
for our customer to evaluate this sensor using sensor development tools with sensors expansion boards.

Hardware requirements
=====================
- Mini/micro C USB cable
- FRDM-MCXN947 board
- FRDM-STBI-A8974 board (https://mcuxpresso.nxp.com/eb-hub/product/frdm-stbi-a8974)
- FreeMASTER 3.2.2 or newer

Board settings
============
Since the examples use I2C, Pins 2-3 of SW2 on FRDM-STBI-A8974 should be connected.
Connect pins 1-2 on jumpers J7 and J8 to select I2C0 on FRDM-STBI-A8974 shield board.
SW1 Pins 2-3 should be connected to select default operating mode i.e. "ACCEL NORMAL" mode..

Prepare the demo
===============
1.  Connect a USB cable between the host PC and the Debug USB port on the target board.
2.  Compile and download the program to the target microcontroller.
3.  Run and resume application execution when debugger stops in the main() function.

Connect with FreeMASTER
=======================
4.  Launch FreeMASTER application installed on your Windows PC.
5.  Click on "Connection Wizard" and select Next>.
6.  Select “Use direct connection to on board USB port” and click Next>.
7.  The FreeMASTER tool detects the COM port (Select the identified COM port on next screen) with the configured baud-rate automatically. Confirm the COM port and baud-rate, click “Next>”.
8.  FreeMASTER detects the board connection and will ask to confirm the detected settings. Confirm by selecting “Yes” and click “Finish”.
9.  FreeMASTER opens an option to “Open an Existing Project”. Select the option.
10. Browse to “<dm-freemaster-fxls89xxxf-evaluation-gui-firmware/fxls89xxxf_evaluation_gui/frdmmcxn947/freemaster_gui/sensors/fxls8974cf” folder.
11. Select “FXLS897xCF_Evaluation_Demo.pmpx” sensor demo project. Click “Open”.
12. FreeMASTER launches the FXLS8974CF sensor demo and opens the control page where user can see sensor power control selections, FS/ODR selections, Offset/Noise measurement selection, along with time-series charts for accelerometer samples.
13. Click “FXLS8974CF Register Page” tab to access the FXLS8974CF register set. Click “Read All” to view instantaneous values of the FXLS8974CF sensor registers in real time.
14. Users can select specific registers and perform single register read or write actions in real time. For a chosen sensor register with read/write access, users can toggle bitfields to change the register value and click “Write” to perform register write operation and/or perform register read by clicking “Read”.


More information
================
Read more information about FreeMASTER Sensor tool at:
https://www.nxp.com/design/design-center/software/sensor-toolbox/freemaster-sensor-tool-for-iot-industrial-medical-sensors:FREEMASTER-SENSOR-TOOL
Feel free to ask questions and report issues at FreeMASTER's 
community page at https://community.nxp.com/community/freemaster
