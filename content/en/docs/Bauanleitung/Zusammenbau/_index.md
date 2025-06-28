---
title: Assembly
description: After you have finished the electronics, the housing must be prepared and everything assembled.
categories: []
tags: []
weight: 6
---

## What you need

<div class="row">
    <div class="col-md-6">
       <h3>Tool</h3>
       <ul>
       <li><img src="/icons/screwdriver.webp" alt="Screwdriver" width="200"/>Screwdriver</li>
        <li><img src="/icons/threads.webp" alt="Soldering iron" width="200"/>Tap cutter Mx</li>
        <li><img src="/icons/cutter.webp" alt="Cutter knife" width="200"/>Cutter knife</li>
       </ul>
    </div>
    <div class="col-md-6 col-sm-6 col-xs-12">
    <h3>Parts</h3>

    
  - Housing
  - Battery pack
  - Lasercut feet
  - Lasercut adapter plate
  - Radar bracket
  - Radar module
  - MicroSD card
  - Everything assembled so far
  - 5x M3x5mm screws
  - 4x M3x14mm cylinder head screws



        
      </div>
</div>

## How it works

<div class="row">

### Mount the adapter plate


<div class="col-md-6">
       {{< imgproc gewinde Fit "600x400 webp" >}}All four holes must be fitted with an M3 internal thread
{{< /imgproc >}} </div>
    <div class="col-md-6" style="display: flex; flex-direction: column; justify-content: center;">
For mounting on street lamps or the tubes of street signs, we need an intermediate piece between the box and the post.
Use the M3 tap to cut an internal thread in each of the four holes in the adapter plate from the laser cutter
    </div>
</div>

<div class="row">
<div class="col-md-6">
       {{< imgproc bplattefest Fit "600x400 webp" >}}Use an Allen key to insert all four cylinder head screws from the inside through the opening and the spacer washer and screw them into the adapter plate.
{{< /imgproc >}} </div>
    <div class="col-md-6" style="display: flex; flex-direction: column; justify-content: center;">
Now take the 4 M3x14mm cylinder head screws, insert them through the recesses at the corners of the housing (from the inside to the outside) and screw them to the adapter plate.
    </div>
</div>
<hr class="my-4"> <!-- Dividing line -->



### Attach base plate
<div class="row">
    <div class="col-md-6">
       {{< imgproc grundplatte_eingebaut Fit "600x400 webp" >}}Base plate with Velcro tape for the battery{{< /imgproc >}} </div>
    <div class="col-md-6" style="display: flex; flex-direction: column; justify-content: center;">

<ul><li>First insert the Velcro tape into the middle opening with the soft side facing upwards and guide it towards the cut-out</li>.

<li>Then place the base plate in the housing with the loose Velcro ends facing upwards and screw tight with M3x5mm screws. The orientation of the plate within the housing does not matter.</li>
</ul>
    </div>
</div>
<hr class="my-4"> <!-- Dividing line -->



<div class="row">

### Attach battery
<div class="col-md-6">
       {{< imgproc akku Fit "600x400 webp" >}}Battery pack in the housing{{< /imgproc >}}</div>
    <div class="col-md-6" style="display: flex; flex-direction: column; justify-content: center;">
Attach battery to base plate with Velcro fastener.
    </div>
</div>
<hr class="my-4"> <!-- Dividing line -->


<div class="row">


### Insert radar module into frame
<div class="col-md-6">
       {{< imgproc 3d Fit "600x400 webp" >}} Front {{< /imgproc >}}
       {{< imgproc _back Fit "600x400 webp" >}} Back {{< /imgproc >}}
</div>
    <div class="col-md-6" style="display: flex; flex-direction: column; justify-content: center;">
 Carefully insert the radar module into the 3D print holder so that the 4 pins protrude through the gap in the holder and the 6 pins on the opposite side protrude through the large opening. The module should be firmly inserted into the 3D printed part at the end.
    </div>
</div>
<hr class="my-4">
<div class="row">

### Attach and screw on Teensy/Audioshield
<div class="col-md-6">
       {{< imgproc all Fit "600x400 webp" >}} Front {{< /imgproc >}} </div>
<div class="col-md-6" style="display: flex; flex-direction: column; justify-content: center;">

- When attaching the Teensy&Audoshield to the pins of the radar module, you just have to make sure that the holes for the screws in the audio shield match those of the 3D print holder.
- Then you can connect the 6-pin connector first and then
- Plug in the 4-pin connector so that the cable is soldered to the second pin (as seen from the jack connection).
- Then attach the audio shield to the bracket with 3 M3x5mm screws.
    </div>
</div>
<hr class="my-4"> <!-- Separation line -->

<div class="row">

### Screw the radar module frame to the adapter plates
<div class="col-md-6">
       {{< imgproc standfuss Fit "600x400 webp" >}} Screwed-on feet {{< /imgproc >}} </div>
<div class="col-md-6" style="display: flex; flex-direction: column; justify-content: center;">

- Now you can screw the feet from the laser cutter to the 3D print holder using one M3x5mm screw each. Do not screw them on too tightly so that you can still move the module.
- The longer of the two long edges points towards the wide end of the 3D print holder, while the overhang on the short edge points away from the radar module.


The feet are only in the base plate for the photo. You do not need the base plate here, it can remain screwed into the housing.  
    </div>
</div>
<hr class="my-4"> <!-- Dividing line -->

<div class="row">

### Insert micro SD card
<div class="col-md-6">
       {{< imgproc microsd Fit "600x400 webp" >}} MicroSD card in the slot of the audio shield {{< /imgproc >}} </div>
<div class="col-md-6" style="display: flex; flex-direction: column; justify-content: center;">
The slot for the MicroSD card is now located between the Teensy and the Audioshield. The micro SD card must be carefully pushed into the Audioshield slot with the contacts facing downwards as far as they will go.
    </div>
</div>
<hr class="my-4"> <!-- Separation line -->

### Button cell holder
<div class="row">
    <div class="col-md-6">
       {{< imgproc knopfzelle Fit "600x400 webp" >}} Button cell holder with button cell {{< /imgproc >}} </div>
    <div class="col-md-6" style="display: flex; flex-direction: column; justify-content: center;">
Now insert the button cell into the button cell holder. The positive pole of the button cell must point towards the cover. Make sure that the switch on the housing of the button cell holder is set to "ON" and only switch it to "Off" if you have to change the button cell anyway.
    </div>
</div>
<hr class="my-4"> <!-- dividing line -->s


<div class="row">

### Electronics in the housing
<div class="col-md-6">
       {{< imgproc alltogether Fit "600x400 webp" >}} Front {{< /imgproc >}} </div>
<div class="col-md-6" style="display: flex; flex-direction: column; justify-content: center;">
Insert the radar unit next to the battery in the slots provided. The slot for the MicroSD card faces away from the battery. The radar unit is held in place by the screwed-on cover, so you can easily access the MicroSD card at any time.
<br>
{{% alert color="primary" %}}
Space is somewhat limited here. But with a little dexterity, you can insert the radar unit without it getting jammed. If necessary, loosen the battery slightly to allow more play.  
{{% /alert %}}
 </div>
</div>
<hr class="my-4"> <!-- dividing line -->

<div class="row">

### Seal the housing cover
<div class="col-md-6">
       
{{< imgproc dichtung_schneiden Fill "400x300 webp" >}}
Shortening the rubber seal.
{{< /imgproc >}}

       
</div>
    <div class="col-md-6" style="display: flex; flex-direction: column; justify-content: center;">
Insert the rubber seal into the groove once all the way around and cut off the excess with a cutter knife. <br>

{{% alert color="primary" %}}
This step is important to prevent moisture from penetrating the housing.
{{% /alert %}}


</div>
</div>
<hr class="my-4"> <!-- separator line -->

**Congratulations! The hardware part is complete!** Before you can screw the cover onto the housing (supplied or M4x20mm security screws), you still need to flash the <a href="/docs/softwareinstallation/">software onto the Teensy developer board</a>

<hr class="my-4">

<div class="d-flex justify-content-between">
  <a class="btn btn-sm btn-primary me-3 mb-4" href="../electronics/preparation-radar-connection">
<i class="fas fa-arrow-alt-circle-left me-2"></i> Previous step
  </a>
  <a class="btn btn-sm btn-primary mb-4" href="../../software-installation/">
    Next step <i class="fas fa-arrow-alt-circle-right ms-2"></i>
  </a>
</div>