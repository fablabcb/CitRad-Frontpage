---
title: Teensy developer board
description: >
  All preparation steps for the Teensy developer board
date: 2024-01-09
weight: 1
---
## What you need

<div class="row">
    <div class="col-md-6">
       <h3>Tool</h3>
       <ul>
       <li><img src="/icons/cutter.webp" alt="Cutter knife" width="200"/>Cutter knife</li>
       <li><img src="/icons/soldering-iron.webp" alt="Soldering iron" width="200"/>Soldering iron + solder</li>
       <li>Micro USB cable + 5V power supply/USB port of the laptop</li>
       </ul>
</div>
    <div class="col-md-6">
<h3>Parts</h3>
<ul>
       <li>Teensy developer board</li>
        <li>Button cell holder</li>
        <li>Shrink tubing (1cm)</li>
       </ul>
       </div>
</div>

## This is how it works



<div class="row">

<div class="row">

### Function test
<div class="col-md-6">
      {{< imgproc control Fit "600x400 webp" >}} The red LED should flash when powered via USB.
{{< /imgproc >}}

</div>
    <div class="col-md-6" style="display: flex; flex-direction: column; justify-content: center;">

The Teensy should basically work before you start with the customizations. Connect the Teensy developer board to a power source via USB. The red indicator light should flash. Now disconnect the USB cable again.<br>
    </div>
</div>
<hr class="my-4"> <!-- Separation line -->

### Disconnect contact for USB power supply
<div class="col-md-6">
       
{{< imgproc cut_contact_done Fit "600x400 webp" >}} The connection between the two rectangular contacts (circled in red) must be removed. Circle 1 and 2 show how.
{{< /imgproc >}}

</div>
    <div class="col-md-6" style="display: flex; flex-direction: column; justify-content: center;">
<p>The Teensy developer board is to be powered by a battery pack for this project. To ensure that it is not inadvertently supplied with power via battery pack and USB, we must first deactivate the power supply via USB. </p>

<p>In the photo, two square contacts are <span style="border: 2px solid #a6113a">circled in red</span>. The two traces are connected by a small trace (<span style="border: 2px solid #00ffffff">see arrow in circle 1</span>). You have to scrape this away with the cutter knife until it looks something like <span style="border: 2px solid #00ffffff">in circle 2.</span> </p>
<p>To check, connect the Teensy to a power source via USB again. The red LED from the first step should no longer flash/light up.
{{% alert color="primary" %}}
You can only continue if the Teensy's red indicator light **no longer** flashes/lights up. Otherwise you will have to rework.
{{% /alert %}}</p>
    </div>
</div>
<hr class="my-4"> <!-- separator line -->



<div class="row">

### Prepare the button cell holder
<div class="col-md-6">
      {{< imgproc knopfzelleschrumpfschlauch Fit "600x400 webp" >}} Button cell holder with shrink tubing over the connection cables
{{< /imgproc >}}

</div>
    <div class="col-md-6" style="display: flex; flex-direction: column; justify-content: center;">

- A button cell also supplies the Teensy with power when it is not connected to the battery. This means it does not lose its time and date settings while you are charging the battery.
- Before you can solder the button cell holder to the Teensy, a small piece of shrink tubing (1 cm) must be pulled over both cables (but not yet heated). This will provide strain relief later.<br>
{{% alert color="primary" %}}
Please only insert the button cell when you are asked to do so in the instructions. Otherwise there is a risk of short circuits during soldering.
{{% /alert %}}
</div>
</div>
<hr class="my-4"> <!-- Separation line -->
<div class="row">

### Solder on the button cell holder
<div class="col-md-6">
      {{< imgproc teensy_knopf Fit "600x400 webp" >}} Soldered button cell holder
{{< /imgproc >}}

</div>
    <div class="col-md-6" style="display: flex; flex-direction: column; justify-content: center;">
The red cable must be soldered to pin 32, the black cable to pin 28. The pin designations can be found on the back of the Teensy<br>

{{% alert color="primary" %}}
It is important that the cables on the underside of the board do not protrude. The SD card slot from the audio board will be located here later. This must not come into contact with the solder joints.   
{{% /alert %}}
</div>
</div>
<hr class="my-4"> <!-- Separation line -->

<div class="d-flex justify-content-between">
  <a class="btn btn-sm btn-primary me-3 mb-4" href="../">
<i class="fas fa-arrow-alt-circle-left me-2"></i> Previous step
  </a>
  <a class="btn btn-sm btn-primary mb-4" href="../audioshield">
    Next step <i class="fas fa-arrow-alt-circle-right ms-2"></i>
  </a>
</div>