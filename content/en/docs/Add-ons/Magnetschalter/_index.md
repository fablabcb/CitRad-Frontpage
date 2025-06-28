---
title: Magnetic switch
description: With the magnetic switch you can start/stop the sensor without having to unscrew the housing every time.
categories: []
tags: []
weight: 5
---
## Preliminary remark
The magnetic switch allows you to start and stop the sensor from the outside. We use a reed contact (normally closed contact) for this purpose, which we attach to the housing wall from the inside. If a magnet is now held in the right place from the outside, the circuit is interrupted. So if you take the magnet with you after installation, the sensor starts to measure. When you come back to dismantle the sensor, push the magnet back on and stop the measurement.

You are completely free to decide where you install the reed contact in your circuit and where it is positioned on the housing. The main thing is that the power supply to the Teensy can be interrupted by the contact.


The 3D printed parts linked below are aligned to the reed contact also linked and kept as small as possible. If you want to make changes to the parts, you can use this [FreeCad project file](https://github.com/fablabcb/CitRad-SensorUnit/raw/refs/heads/develop/Hardware/Addons/magneticOnOFF-CitRad.FCStd).
{{% alert color="primary" %}}
It depends on the correct alignment of the magnet to the reed contact. If you use other contacts, you may have to construct your own magnet holder, depending on how it works.
{{% /alert %}}

## What you need

<div class="row">
    <div class="col-md-6">

### Tool
<ul>
       <li><img src="/icons/soldering-iron.webp" alt="Soldering iron" width="200"/>Soldering iron + solder</li>
       <li><img src="/icons/abiso.webp" alt="Soldering iron" width="200"/>Soldering pliers</li>
       <li>Shrink tubing (5cm, optional)</li>
       <li>Second glue</li>
       </ul>

</div>
    <div class="col-md-6">

### Parts
- finished sensor
- Reed contact (normally closed contact)](https://www.amazon.de/dp/B088CQL44X)
- [Contact holder inside](/parts/ReedSensorHolder_mOO-Citrad.stl) (3D printed part)
- [Magnet holder](/parts/MAgnetMount_mOO-Citrad.stl) (3D printed part)
- Magnet holder](/parts/MagnetSlider_mOO-Citrad.stl) (3D print part)
- Some extra cable (optional)
       </div>
</div>

## This is how it works
<div class="row">

### Preparation

<div class="col-md-6">
       {{< imgproc MagneticSwitch_allparts.png Fit "600x400 webp" >}} All required 3D printed parts {{< /imgproc >}}
</div>
    <div class="col-md-6" style="display: flex; flex-direction: column; justify-content: center;">


 You need to produce these three parts using a 3D printer. They are designed so that both the reed contact and the magnet rest directly on the housing wall. If you want to use your own designs, you must also take this into account so that the reed contact is triggered.
    </div>
</div>
<hr class="my-4"> <!-- Dividing line -->
<div class="row">

### Gluing on the holder

<div class="col-md-6">
       {{< imgproc reedHolder.jpg Fill "600x300 webp Top" >}} All required 3D printed parts {{< /imgproc >}}
       {{< imgproc magnetMount.jpg Fill "600x300 webp Top" >}} All required 3D print parts {{< /imgproc >}}
</div>
    <div class="col-md-6" style="display: flex; flex-direction: column; justify-content: center;">

1. first glue the reed contact holder into the housing. Make sure that the small triangle points towards the housing and that the tip of the triangle is not positioned higher than the indentation on the edge of the housing where the cover will later click into place.
2. Now glue the magnet holder on the outside so that the triangle is aligned and positioned at the same height (eye measurement is sufficient) as the triangle on the reed contact holder on the inside. It is also important that the narrow part of the bevel points towards the housing. Otherwise it will be impossible to slide the magnet on later.

 
    </div>
</div>
<hr class="my-4"> <!-- Dividing line -->
<div class="row">

### Wiring of the reed contact

<div class="col-md-6">
       {{< imgproc wiringReed.jpeg Fit "600x400 webp" >}} Pluggable integration variant makes the use of the magnetic switch optional. {{< /imgproc >}}
</div>
    <div class="col-md-6" style="display: flex; flex-direction: column; justify-content: center;">

You can freely choose where to install the reed contact in the circuit. You can solder it permanently or make it pluggable with an extra plug and socket as an optional part, as shown here.

As soon as the wiring is complete, the reed contact must be inserted into the holder with the square protrusion pointing towards the inside of the housing. Make sure that it really is fully seated against the housing wall.
    </div>
</div>
<hr class="my-4"> <!-- Dividing line -->

<div class="row">

### Test the correct orientation of the magnet

<div class="col-md-6">
       {{< imgproc magnetMountMagnet.jpg Fill "600x300 webp Top" >}} Magnet test plugged in to test orientation {{< /imgproc >}}
       {{< imgproc magnetHolderMagnet.jpg Fill "600x300 webp Center" >}} Magnet glued into the magnet holder. {{< /imgproc >}}
</div>
    <div class="col-md-6" style="display: flex; flex-direction: column; justify-content: center;">

The reed contact will only reliably interrupt the circuit if the magnet is applied in the correct orientation. It therefore depends on which side of the magnet points to the left and which to the right. To find out the correct orientation, insert the magnet without its holder (3rd 3D printed part) into the holder and connect the rest of the circuit. If the sensor remains off (no LEDs light up/flash), you have already found the correct orientation. Otherwise, turn the magnet around and repeat the test. Alternatively, you can of course also measure for continuity with a multimeter.

Now that you know the correct orientation, you can glue the magnet into the holder. The holder is designed so that it can only be slid open in one direction (small locking lugs at one end). Glue the magnet into the holder so that it is correctly oriented when you slide it on. Make sure you press the magnet fully into the holder so that the distances are correct afterwards.
    </div>
</div>
<hr class="my-4"> <!-- Dividing line -->

<div class="row">

### The final "off" position

<div class="col-md-6">
       {{< imgproc offPosition.jpg Fill "600x300 webp Center" >}} This is what the off-position looks like {{< /imgproc >}}
</div>
    <div class="col-md-6" style="display: flex; flex-direction: column; justify-content: center;">

When everything is glued and plugged together, you can connect the circuit completely. As long as the magnet is in place, no current will flow. Only when you remove the magnet holder/magnet does the measurement begin.  
    </div>
</div>
<hr class="my-4"> <!-- Separation line -->