---
description: >-
  Basic setup of using controllers to be able to pick up and interact with
  objects
---

# Basic Interactable Objects

### XR Ray Interactor Setup

Navigate to the _Left Hand Controller_ in the _Hierarchy_

Find the **XR Ray Interactor** component in the _Inspector_

* If there isn't an _XR Ray Interactor componen_t, add one&#x20;

Within XR Ray Interactor component

* Disable **Anchor Control**
* Enable **Hide Controller on Select**

Do the same for **Right Hand Controller**

<figure><img src="https://lh4.googleusercontent.com/7YIvK9A64NBGnzXgXy662hrDX-Le39jAaI0dzqewoqKGxUHKO9r3AaZRJK2DcCqSj2VSJ9iCx6EtJ8p99DfZyK4ywehgjop1JCxuqeXcE_SenznTUAuZBqrDVOhZqF1ODzzJjPHnPKWhGQmXc_0FcpA" alt="" width="375"><figcaption></figcaption></figure>

### Making Objects Grabable&#x20;

1. Add the XR Grab Interactable component to your object
   * <mark style="background-color:yellow;">Note: This will automatically add a Rigidbody component as well</mark>
2. In your Rigidbody component:
   * Select Continuous Dynamic for your collision detection method
3. In your XR Grab Interactable component:
   * Set your movement type to Kinematic
   * Check on Smooth Position
   * Check on Smooth Rotation
4. (Optional) Add a specific Attach point to Model
   1. Make an empty game object named “Attach” as a child of the grabable object.&#x20;
   2. Transform the Attach game object to the correct orientation using the transform tools
   3. In the XR Grab Interactable component of your object locate the Attach Transform property.&#x20;
5. Drag and drop your new Attach object to assign it to the Attach Transform property.
