---
parent: Harmony 3 driver and system service application examples for PIC32CZ-CA80 family
title: FAT filesystem using SST26 Media 
has_children: false
has_toc: false
---

[![MCHP](https://www.microchip.com/ResourcePackages/Microchip/assets/dist/images/logo.png)](https://www.microchip.com)

# FAT filesystem using SST26 Media

This application shows an example of using the FAT File System to access SQI based SST26 flash media

## Description

### File System Operations on the On-Board SST26 Flash Memory:

- Performs a SYS_FS_FormatDisk
- Opens a **newfile.txt** on the SST26 flash
- Write and reads back 4KB of data on **newfile.txt**
- Verifies the Data Read back

### File system layer uses:

- One instance of the Memory driver is used to communicate with the On-Board SQI Flash memory

## Downloading and building the application

To clone or download this application from Github, go to the [main page of this repository](https://github.com/Microchip-MPLAB-Harmony/csp_apps_pic32cz_ca) and then click **Clone** button to clone this repository or download as zip file.
This content can also be downloaded using content manager by following these [instructions](https://github.com/Microchip-MPLAB-Harmony/contentmanager/wiki).

Path of the application within the repository is **apps/fs/sqi_flash_fat/firmware**

To build the application, refer to the following table and open the project using its IDE.

| Project Name      | Description                                    |
| ----------------- | ---------------------------------------------- |
| pic32cz_ca80_curiosity_ultra.X    | MPLABX Project for [PIC32CZ-CA80 Curiosity Ultra board](https://www.microchip.com/developmenttools/ProductDetails/)|
|||

## Setting up the hardware

The following table shows the target hardware for the application projects.

| Project Name| Board|
|:---------|:---------:|
| pic32cz_ca80_curiosity_ultra.X    | [PIC32CZ-CA80 Curiosity Ultra board](https://www.microchip.com/developmenttools/ProductDetails/)|
|||

### Setting up [PIC32CZ-CA80 Curiosity Ultra board](https://www.microchip.com/developmenttools/ProductDetails/)

- Connect the Debug USB port on the board to the computer using a micro USB cable

## Running the Application

1. Build and program the application using its IDE
2. The LED is turned ON if data has successfully been written and read back from file "newfile.txt"

Refer to the following table for LED name:

| Board | LED Name |
| ----- | -------- |
|  [PIC32CZ-CA80 Curiosity Ultra board](https://www.microchip.com/developmenttools/ProductDetails/) | LED1 |
|||