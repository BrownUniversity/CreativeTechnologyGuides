---
description: >-
  Moving around, picking up objects and triggering events requires adding VR
  interaction components in Unity
---

# Enable Controller Movement + Teleportation

### Add a locomotion system

* In the Hierarchy select **the XR Origin Game Object**_._
* Click on the **Add Component** button. Search and select the **Locomotion System**
*   Drag the **XR Origin Game Object** in the _Hierarchy_ into the _XR Origin parameter_ drop-down box.&#x20;

    <figure><img src="../../../.gitbook/assets/Screen Shot 2023-07-13 at 10.40.49 AM.png" alt="" width="563"><figcaption></figcaption></figure>

### Set your left controller joystick to move foward, backward, and strafe left and right

* In the Hierarchy select **the XR Origin Game Object**_._
* Click on the **Add Component** button. Search and select the **Continuous Move Provider**

#### Within the Continuous Move Provider component**:**

* Drag the **XR Origin Game Object** in the _Hierarchy_ into the S_ystem_ drop-down box.&#x20;
* Check-on **Enable Strafe**
*   Under the _Left-Hand Move Action,_ Check-on **Use Reference**

    * The _Reference_ parameter should auto populate with the **XRI LeftHand Locomotion/Move** script
    * If it doesn't, click on the bullseye to the right of the drop down and select the **XRI LeftHand Locomotion/Move** script

    <figure><img src="../../../.gitbook/assets/Screen Shot 2023-07-13 at 10.20.28 AM.png" alt="" width="375"><figcaption></figcaption></figure>

### Set your right controller joystick to turn clockwise and counter-clockwise

* In the Hierarchy select **the XR Origin Game Object**_._
* Click on the **Add Component** button. Search and select the **Continuous Turn Provider**
*

    #### Within the Continuous Turn Provider component**:**

    * Drag the **XR Origin Game Object** in the _Hierarchy_ into the S_ystem_ drop-down box.&#x20;
    * Set _Turn Speed_ to **60.**&#x20;
      * Lower the number if you tend to get dizzy or nauseous
    *
    *   Under the _Right Hand Turn Action,_ Check-on **Use Reference**

        * The _Reference_ parameter should auto populate with the **XRI RightHand Locomotion/Turn** script
        * If it doesn't, click on the bullseye to the right of the drop down and select the **XRI RightHand Locomotion/Turn** script

        <figure><img src="../../../.gitbook/assets/Screen Shot 2023-07-13 at 10.34.52 AM.png" alt="" width="375"><figcaption></figcaption></figure>

## Teleportation

This will allow you to teleport instantaneously onto surfaces marked for teleportation

### Set up your XR Origin to Teleport

* In the Hierarchy select **the XR Origin Game Object**_._
* Click on the **Add Component** button. Search and select the **Teleportation Provider**
* Drag the **XR Origin Game Object** in the _Hierarchy_ into the _System_ drop-down box.
* <mark style="color:red;">Remember, you can only teleport on surfaces that have been marked for teleportation</mark>&#x20;

<figure><img src="../../../.gitbook/assets/Screen Shot 2023-07-13 at 10.47.15 AM.png" alt="" width="563"><figcaption></figcaption></figure>

### Mark game objects/surfaces for teleportation

**Select** the game object you want to enable teleportation on. This may be a floor, or different platforms in your VR project.

Click on the **Add Component** button. Add a **Collider** to your object. Often a plane or box collider are best.&#x20;

Click on the **Add Component** button. Search and select the **Teleportation Anchor** or **Teleportation Area**, whichever you prefer.

* **Teleportation Area:** Teleport to any point on the surface of the object&#x20;
*
* **Teleportation Anchor:** Teleport to the middle/center of the object

Under the parameter, _Interaction Layer Mask_, click the drop-down that says _default_ and select **Nothing**

<figure><img src="../../../.gitbook/assets/Screen Shot 2023-07-13 at 11.16.37 AM.png" alt="" width="375"><figcaption></figcaption></figure>

Click on the drop-down again and select **Teleport**

<figure><img src="../../../.gitbook/assets/Screen Shot 2023-07-13 at 11.16.55 AM.png" alt="" width="375"><figcaption></figcaption></figure>

1. If the option for _Teleport_ doesn't exist, select **Add Layer**
2. Write **Teleport** on any free space
3. Navigate back to the object in the _Hierarchy_ and sent the _Interaction Layer Mask_ to **Teleport**
4. <mark style="background-color:yellow;">Setting up and Using the</mark> <mark style="background-color:yellow;"></mark>_<mark style="background-color:yellow;">Teleport Interaction Layer Mask</mark>_ <mark style="background-color:yellow;"></mark><mark style="background-color:yellow;">Isn't technically necessary, but it is a best practice that will allow for more control over your project.</mark>&#x20;



<figure><img src="../../../.gitbook/assets/Screen Shot 2023-07-13 at 11.41.25 AM.png" alt="" width="375"><figcaption><p>A reference of default settings for the Telelportation Area when enabled correctly. </p></figcaption></figure>
