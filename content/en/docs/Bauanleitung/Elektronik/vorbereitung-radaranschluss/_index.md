---
title: Preparation of radar connection
description: >
  You must install a voltage converter for the power supply of the radar module. You also need to prepare connections for data exchange between the components.
date: 2024-01-09
weight: 3
---
## What you need

<div class="row">
    <div class="col-md-6">
       <h3>Tool</h3>
       <ul>
       <li><img src="/icons/spitzzange.webp" alt="Spitzzange" width="200"/>Spitzzange</li>
       <li><img src="/icons/soldering-iron.webp" alt="Soldering iron" width="200"/>Soldering iron + solder</li>
       </ul>
</div>
    <div class="col-md-6">
<h3>Parts</h3>
<ul>
       <li>Teensy developer board + audio shield from previous step</li>
        <li>Voltage converter</li>
        <li>Header 6-pin</li>
        <li>Header 4-pin</li>
        <li>Cable (approx. 4 cm)</li>
       </ul>
       </div>
</div>

## How it works

<div class="row">

### Connect voltage transformer and Teensy
<div class="col-md-6">
       {{< imgproc spannungswandler1 Fit "600x400 webp" >}} Voltage transformer, soldered to GND and 3.3V of the Teensy {{< /imgproc >}}
</div>
    <div class="col-md-6" style="display: flex; flex-direction: column; justify-content: center;">

<p>Not in the photo: Place the voltage transformer in front of you with the label facing up and the feet pointing towards you. Now bend the two left feet upwards by 90° as close to the voltage transformer as possible.</p>
<p>See photo: Now place the voltage transformer on the Teensy with the label facing downwards. Make sure that the bent feet are on the left of the two single pins that protrude from the 3.3V contact and GND contact (to the right).</p>
<p>Now you can solder both contact points.</p>
    </div>
</div>
<hr class="my-4"> <!-- Separation line -->




<div class="row">

### Preparing the plug connection (part 1: header 6-pin)
<div class="col-md-6">

{{< tabpane text=true right=true >}}
  {{% tab header="Bend:" disabled=true /%}}
  {{% tab header="1." %}}
  
{{< imgproc 6-pin-rem-pin Fit "600x400 webp" >}} Pin 1 pulled out {{< /imgproc >}}

  {{% /tab %}}
  {{< tab header="2.">}}
    
{{< imgproc 6-pin_bend1 Fit "600x400 webp" >}} Pin 5 and 6: First bend 90° backwards {{< /imgproc >}}

  {{< /tab >}}

  {{% tab header="3." %}}

{{< imgproc 6-pin_bend2 Fit "600x400 webp" >}} Second bend down {{< /imgproc >}}
  {{% /tab %}}

  {{< tab header="4.">}}
    
{{< imgproc shield_line_in Fit "600x400 webp" >}} Both pins soldered to the line-in of the audio shield {{< /imgproc >}}

  {{< /tab >}}
{{< /tabpane >}}

</div>
    <div class="col-md-6" style="display: flex; flex-direction: column; justify-content: center;">

- Click through the bending tabs (1.-4.) to see detailed photos of the individual steps.
- Pull pin 1 (far left) out of the connector. It is no longer needed.
- First bend pins 5 and 6 (far right) backwards by 90°. Then bend them downwards by approx. 75 degrees with a gap of approx. 4 mm. Both pins must reach the line-in contacts of the audio shield and be soldered there.

</div>
</div>
<div class="row">
<div class="col-md-6">
       {{< imgproc prep_spannung Fit "600x400 webp" >}} Soldered header 6-pin {{< /imgproc >}}
</div>
<div class="col-md-6" style="display: flex; flex-direction: column; justify-content: center;">

<ul>
<li>The header 6-pin must fit on the end of the radar module. It can help if you attach the radar module to the audio shield to bend the pins. The necessary steps are explained <a href="/docs/bauanleitung/zusammenbau/#radarmodul-in-rahmen-stecken">from here</a> in the "Assembly" chapter.
<li style="border: 2px solid #7adef1ff"> Bend enable (pin 2) to pin 17 of the Teensy and solder together (just fits).</li>
<li style="border: 2px solid #a6113aff"> Connect Gnd (pin 4) and Vcc (pin 3) diagonally to the output of the voltage converter (see photo). You may have to bridge this with solder or a short wire. The photo at the bottom of the page shows another top view that may be helpful.</li
</ul>
{{% alert color="primary" %}}
Make sure there are no cross connections. If necessary, bend the wires slightly apart.
{{% /alert %}}

</div>
</div>
<div class="row">

</div>
<hr class="my-4"> <!-- separator line -->

<div class="row">

### Preparing the plug connection (part 2: header 4-pin)
<div class="col-md-6">
       {{< imgproc radar_stecker Fit "600x400 webp" >}} Prepared header 4-pin. {{< /imgproc >}}
</div>
    <div class="col-md-6" style="display: flex; flex-direction: column; justify-content: center;">

 - You must solder one end of the cable (4cm) to one of the inner contacts of the header 4-pin.

     </div>
</div>
<hr class="my-4"> <!-- Separation line -->
<div class="row">

### Final result
<div class="col-md-6">
       {{< imgproc radar_stecker_prep2_pin Fit "600x400 webp" >}} Final result after executing all steps {{< /imgproc >}}
</div>
    <div class="col-md-6" style="display: flex; flex-direction: column; justify-content: center;">

- Solder the other end of the cable coming from the header 4-pin to GND (lineout or mic) of the audio shield.
- In the end, everything should look like the photo.

    </div>
</div>
<hr class="my-4"> <!-- Separation line -->

<div class="d-flex justify-content-between">
  <a class="btn btn-sm btn-primary me-3 mb-4" href="../preparation-radar-connection">
<i class="fas fa-arrow-alt-circle-left me-2"></i> Previous step
  </a>
  <a class="btn btn-sm btn-primary mb-4" href="../../assembly/">
    Next step <i class="fas fa-arrow-alt-circle-right ms-2"></i>
  </a>
</div>