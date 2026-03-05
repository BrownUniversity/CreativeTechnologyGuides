---
description: Step-by-step guide to using the large format inkjet printer
cover: >-
  ../.gitbook/assets/EPSON-SureColor_-P9000-Standard-Edition-Printer-EPSON-1683067358.jpeg
coverY: 136.36533333333333
---

# 🖨️ 3D Printing using SimplyPrint

**BEFORE using the 3D printers you must**:

* [ ] Complete the online quiz
* [ ] Meet with a Creative Technology Assistant

For more information go to [https://go.brown.edu/cats-3dprinting](https://go.brown.edu/cats-3dprinting)

***



CATS uses the online platform SimplyPrint to handle all 3D printing. Attempting to print using the printers directly or via USB is not permitted.

### Only print from the Physical Media Lab

While SimplyPrint is an online platform for handling 3D printing we require all users to start prints while they are physically present in the Physical Media Lab in order to ensure that the print starts successfully. Failure to be present when printing can result in loss of printing privileges.

### Log in to SimplyPrint

During your training with the Creative Technology Assistant they will create a SimplyPrint account. You can log in to your account at [https://simplyprint.io/panel/login](https://simplyprint.io/panel/login)

After you log in you should see your dashboard which looks something like this:

<figure><img src="../.gitbook/assets/SimplyPrint-01-Dash.png" alt="Screenshot of the SimplyPrint dashboard"><figcaption></figcaption></figure>

### Uploading your 3D model

SimplyPrint accepts a variety of 3D model formats including:

* STLs
* OBJs
* STEP

In addition advance users can upload gcode files directly to SimplyPrint. **Any gcode upload must be  designed specifically for the Prusa MK4S printers we have in the lab.**&#x20;

If you have questions about using gcode please consult with the CTA or email cats@brown.edu

#### Choose slicing

When you upload your 3D model it will ask you if you want to save the model file, slice it or add to queue. Saving will save the unsliced model file for later use. We want to slice the file so choose that.

<figure><img src="../.gitbook/assets/SimplyPrint-02-SaveSliceQueue.png" alt="Screen shot of screen showing Save, Slice and Add to queue buttons."><figcaption></figcaption></figure>

We do not use queues so never use the "Add to queue" option.

### Slicing settings

**We recommend that beginners use the "Basic" settings for slicing.**&#x20;

<figure><img src="../.gitbook/assets/SimplyPrint-03-SliceSettings.png" alt="Screenshot of the slicing window with Basic settings selected"><figcaption></figcaption></figure>

#### **Select preset**&#x20;

Choose **0.20mm SPEED @MK4S HF 0.4**. This is a good default setting for most prints.

#### **Infill Density**

Choose **20% infill.** &#x20;

Prints rarely need more than 20-30% infill. For increase print strength the Wall Count is a more important setting. Higher infill increases print time and wastes filament.

#### Wall Count <a href="#id-8fyl8oaxcd7o" id="id-8fyl8oaxcd7o"></a>

Choose _**2 perimeter walls**_.

This setting has the most effect on print strength. If you need a stronger prints you can increase the perimeter walls to 3 or 4.

#### Bed adhesions <a href="#idiq8243anp3" id="idiq8243anp3"></a>

**Add a Brim if needed**. Adding a b**rim** can help secure prints to the bed preventing them from falling off the bed. This is important for prints with small bed footprint or long prints that might begin to warp as the print continues.

#### Use supports <a href="#l3ykjhsr26e3" id="l3ykjhsr26e3"></a>

**Turn on supports if needed**. Adding supports is important for any prints that have parts that overhanging parts.

### Adjusting the model

In addition to the slicing you can make adjustments to the model or add additional objects to the bed before slicing.

<figure><img src="../.gitbook/assets/SimplyPrint-04-AdjustObject.png" alt="Screenshot of 3D view of SimplyPrint show button location of key features."><figcaption></figcaption></figure>

#### Move, rotate and scale

The three buttons to the left of the 3D view allow you to move, rotate or scale your object. You can either adjust them with the dialog next to the button or use the transform Gizmo/Tool on the object itself.

#### Add objects

You can add more than one object/model to the bed and slice them together.

#### Arrange objects

This option allows you to space multiple objects on the bed.

#### Smart rotate

SimplyPrint can analyze your model and identify what it thinks is the best face to rest on the bed.&#x20;

#### Lay on side

This option lets you choose a specific face and SimplyPrint will place that face on the bed.



### Additional resources

For more information about our services please visit the CATS website: [https://go.brown.edu/cats-3dprinting](https://go.brown.edu/cats-3dprinting)



<figure><img src="https://lh5.googleusercontent.com/T5b1wgMSzgYoKdukfrH5lmBYpeKcFvKVRqCnXzkpFYMxThyPpWUJT0_yfmJe_gk-MZaqABs-8i76cM1A-bBx8B9zDBcN06DIeHRA5yOJbBqOwzplEYU-kKSsppfA_PsoOOMvhdX92KVbGGy1AQiPxXbXeFvaE9BAzYFdS5pqr5AXuIBGO34Gvz6kNt5GOQ" alt="" width="188"><figcaption></figcaption></figure>

