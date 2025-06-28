---
title: Connecting Audioshield and Teensy
description: >
  Preparation of the Audioshield for assembly with the developer board
date: 2024-01-09
weight: 2
---
## What you need

<div class="row">
    <div class="col-md-6">
       <h3>Tool</h3>
       <ul>
       <li><img src="/icons/string-cutter.webp" alt="Side cutter" width="200"/>Side cutter</li>
       <li><img src="/icons/spitzzange.webp" alt="Pointed pliers" width="200"/>Pointed pliers</li>
       <li><img src="/icons/soldering-iron.webp" alt="Soldering iron" width="200"/>Soldering iron + solder</li>
       <li><img src="/icons/abiso.webp" alt="Soldering iron" width="200"/>Soldering pliers</li>
       </ul>
</div>
    <div class="col-md-6">
<h3>Parts</h3>
<ul>
       <li>Teensy developer board</li>
       <li>Audio shield</li>
        <li>2-core cable (4cm)</li>
        <li>40-pin header</li>
        <li>Battery socket</li>
        <li>Battery pack (only for checking the correct polarity when soldering)</li>
       </ul>
       </div>
</div>

## How it works

<div class="row">

### Shorten the pin header
<div class="col-md-6">
       {{< imgproc audio_pinleiste Fit "600x400 webp" >}} Shorten the pin header to the length of the audio shield {{< /imgproc >}}
</div>
    <div class="col-md-6" style="display: flex; flex-direction: column; justify-content: center;">


 The 40-pin strip is too long for the audio shield. Simply insert it flush on one side onto the row of holes in the audio shield and cut off the excess with the side cutter.

 Do the **same** for the opposite side. You should now have two strips of the same length (14 pins) and a shorter remaining piece.
 
 The remaining piece is no longer needed. It is best to put it aside so that you don't use it by mistake.
    </div>
</div>
<hr class="my-4"> <!-- dividing line -->

<div class="row">

### Solder the pin headers
<div class="col-md-6">
       {{< imgproc soldered Fit "600x400 webp" >}} The short ends of the shortened pin headers are soldered to the audio shield. {{< /imgproc >}}
</div>
    <div class="col-md-6" style="display: flex; flex-direction: column; justify-content: center;">


 Now insert your two pin headers of the same length into the audio shield with the short side from above (side with jack connection and Micor SD card slot) and solder the headers to the back of the audio shield pin by pin.
    </div>
</div>
<hr class="my-4"> <!-- Separation line -->

<div class="row">

### Set up Teensy and customize pins
<div class="col-md-6">
       {{< imgproc modified_pins Fit "600x400 webp" >}} Clip off the pins (cyan) or bend them (red). {{< /imgproc >}}
</div>
    <div class="col-md-6" style="display: flex; flex-direction: column; justify-content: center;">


 <ul><li>Now place the Teensy on the long pins. The USB socket points upwards and in the same direction as the audio shield's jack connection.</li
 <li style="border: 2px solid #a6113aff"> Use needle-nose pliers (<img src="/icons/spitzzange.webp" alt="Spitzzange" width="50"/>) to bend the pins on 5V and GND diagonally forwards as shown in the photo.</li>
 <li style="border: 2px solid #7adef1ff">
  In order to be able to solder the voltage transformer properly later on, use the side cutter (<img src="/icons/string-cutter.webp" alt="Side cutter" width="50"/>) to cut off pins 21, 22, 23.</li>
  <li>Now solder all the pins to connect the two boards.
 </ul>
    </div>
</div>
<hr class="my-4"> <!-- Separation line -->



<div class="row">

### Prepare the socket for the power supply
<div class="col-md-6">
       {{< imgproc cable_plug Fit "600x400 webp" >}} Solder the socket cable together {{< /imgproc >}}
</div>
    <div class="col-md-6" style="display: flex; flex-direction: column; justify-content: center;">


 <ul>
 <li>In the picture you can see <span style="border: 2px solid #7adef1ff">the two-core cable (4 cm) framed in cyan and the connection socket.</span> The connection socket still contains a plug (with cable) that was included in the scope of delivery. This can be a help when soldering. However, you will no longer need the plug and cable in the following steps.
 <li> Cut the two-core cable (4 cm) a little on both sides and strip all ends. (Already done in the photo)</li>
 <li>Now solder the cable <strong>to the socket</strong> so that the <strong>polarity matches the plug of the battery pack</strong>.
 </li>
 </ul>
 {{% alert color="primary" %}}
Caution: Some socket/plug sets have the polarity reversed. Always compare whether the plug has the same polarity as the battery pack and only then solder the socket to the cable accordingly.
{{% /alert %}}
    </div>
</div>
<hr class="my-4"> <!-- Separation line -->

<div class="row">

### Solder the socket with strain relief
  <div class="col-md-6">
       {{< imgproc stecker1 Fit "600x400 webp" >}} Solder the socket cable together {{< /imgproc >}}
</div>
    <div class="col-md-6" style="display: flex; flex-direction: column; justify-content: center;">

 <ul><li>Now route the cable of the button cell holder (already soldered to the Teensy) over the Teensy in the direction of the USB socket. Then feed the black cable of the battery pack socket from the previous step (coming from the button cell) through the shrink tubing. </li>
 <li>Solder the <span style="background-color:black; color:white">black</span> cable to the bent <span style="background-color:black; color:white">GND pin</span> and the <span style="background-color:red; color:white">red</span> cable to the likewise bent <span style="background-color:red; color:white">5V pin</span>.</li>
 <li>In order to relieve the soldering points for the cables of the button cell holder against tension, all cables are "fixed" in the shrink tubing by heating them. To do this, push the cables of the button cell holder back slightly in the direction of their soldering points so that there is no longer any tension on these cables. Now carefully heat the shrink tubing with a heat gun or lighter.</li>
 </ul>
    </div>
</div>
<hr class="my-4"> <!-- Separation line -->

<div class="d-flex justify-content-between">
  <a class="btn btn-sm btn-primary me-3 mb-4" href="../developer-board">
<i class="fas fa-arrow-alt-circle-left me-2"></i> Previous step
  </a>
  <a class="btn btn-sm btn-primary mb-4" href="../preparation-radar-connection">
    Next step <i class="fas fa-arrow-alt-circle-right ms-2"></i>
  </a>
</div>