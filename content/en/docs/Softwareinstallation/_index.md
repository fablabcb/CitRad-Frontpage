---
title: Software installation
description: Need some more brains? The last step before setting up on the road is to install the software on the Teensy
categories: []
tags: []
weight: 3
---

## What you need

<div class="row">
    <div class="col-md-6">

### Tool
- Laptop/PC with Linux or Windows
- Data cable (Micro-USB)
- Latest version of the [.hex file](https://github.com/fablabcb/CitRad-SensorUnit/releases) (sensor.ino.hex)
- Teensy-Loader](https://www.pjrc.com/teensy/loader.html) for your operating system.

</div>
    <div class="col-md-6">

### Parts
- finished sensor
       </div>
</div>

## How it works

The manufacturer of the Teensy provides the software (Teensy loader) for flashing for Linux, Windows and Mac on its website (see above). You can get the necessary .hex file from our repository (also linked above). Now you can connect the sensor to your PC/laptop via micro USB cable, start the Teensy loader and flash the .hex file. Simply follow the instructions on the manufacturer's website.

When flashing, the current time is also transmitted to the Teensy. This is important so that we can later assign the data to the date and time of day. If the power supply via the button cell is interrupted at any time (defect or replacement of the battery), simply reflash the .hex file before the next measurement.

{{% alert color="primary" %}}
The Teensy starts working immediately after installing the software. This means that there may already be .csv and .bin files on the memory card. It is best to disconnect the sensor unit from the battery pack now and delete these files from the SD card. You should <strong>not</strong> accidentally load this data into the portal later.
{{% /alert %}}

### Flashing with Arduino IDE

If you are familiar with the Arduino IDE, you are of course also free to clone [our repository](https://github.com/fablabcb/CitRad-SensorUnit) and flash the Teensy yourself.


<div class="d-flex justify-content-between">
  <a class="btn btn-sm btn-primary me-3 mb-4" href="../assembly-instructions/assembly">
<i class="fas fa-arrow-alt-circle-left me-2"></i> Previous step
  </a>
  <a class="btn btn-sm btn-primary mb-4" href="../measurement-instructions">
    Next step <i class="fas fa-arrow-alt-circle-right ms-2"></i>
  </a>
  </div>