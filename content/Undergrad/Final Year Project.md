
# Abstract
##### What i do?
The design and development of a multi-modal gripper part of a robotics platform; capable of prehensile contact, in-hand manipulation, form & force closure, universal adaptability while being mechanically simple.

So basically, start with how typical grippers lack universal adaptability and how soft robots have complex control schema. While it possible mechanically to do within-hand simulations and stuff, they are very complex. Numerous motors for control. An elegant approach with the help of underactuated systems is taken into account in this picture.
Gives bg context (answers what and why)

Now, how:
Here, we have ideated two concepts to achieve these requirements while being mechanically simple. The first concept is a multi-segmented links and rollers system powered by a serial geartrain. A series of prototypes were built to understand the working of this gripper. Ultimately this concept faces issues with grasping as the rollers come into contact with object. The rollers have discontinuities in between and tend to lose grip of the object. This concept was further redefined

##### Introduction
underactuation: controllable degrees of freedom, I have lots but i choose to control few

##### Motivation:
To build a kinematically scalable, unique multifunctional universal gripper that can traverse structured and unstructured terrain, perform different modes of grasping, and be capable of in-hand manipulation while being mechanically simple. 
but should also be precise.

To build a kinematically scalable unique multifunctional universal gripper that can perform multiple modes of grasping, traverse structured and unstructured terrain, be capable of in-hand manipulation with minimal number of actuators while keeping the mechanical complexity minimal.

To navigate a complex, unstructured environment where the grasping and manipulation of an unknown object is required

The end effector of the manipulator is the most vital part. It focuses on grasping and in-hand manipulations. The end effectors in such systems have very complex mechanisms and control schema resulting in the end effector being isolated from the locomotive platform, thereby increasing the total number of actuators and complexity. GML (Grasping Manipulation Locomotion) platforms like Graspman unifies these platforms, but the design remains complex. Simplifying these systems still remain a key challenge.

To build a multifunctional gripper with a platform that can grasp a wide range of objects (universal), manipulate them within hand and traverse any structured and unstructured environment (locomotion) while keeping the mechanical complexity to a minimum.


##### Methodology:
A serial geartrain mechanism was initially developed and was made viable as a gripper through successive iterations. This led to the development of a gear-train with multi-segmented links with rollers as a grasping surface. Addressing the discontinuity created by the rollers led to the development of multi-segmented links with belts, where the belts are the contact surface with the object.

