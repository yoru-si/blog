---
aliases:
  - grippers
  - robots
  - concept design
---
	# What?
Graspman is a modular multi-modal robotic platform equipped with a universal grasper capable of within hand manipulation. Currently I am working on a concept which includes multi-segmented links with rollers.

refer [[graspman_paper.pdf]] for more details.

#projects/graspman #robotics

The idea has undergone through 3 iterations, with multiple concepts brimming. The progress overall has rather been quite slow. Currently the central theme has been diverged by two for faster ideation. The final product will be a combination of these two concepts.

This is currently my [[Final Year Project]], it is due by May. I need to start working on the report and the presentation. The problem is I might have to scrap the concept completely.

- [ ] The second finger
- [x] C-Link durability, stiffness
- [ ] Entire gripper construction
- [x] Optimize gear backlash using openSCAD, streamline the process for generating gear cutting code, include printer tolerance into play.
- [x] Dual bearing motor mounts? Is it even necessary? Check other designs, Suggest dual supported C-links
- [ ] Ball bearings quotation and purchase.
- [ ] Nylon filament purchase.
- [x] Filament desiccant preservation


# Why?


# The math behind graspman
#projects/graspman/math
1. Repeatability test: This test verifies the repeatability of the following within-hand manipulation commands: Translation and Rotation.
2. Grasp Force: Unsure about what to do, but to the best of what I know, this experiment understands the contact forces of the disc with the object. Calculates required dyanmixel servo motor torque to hold object with firm grasp.
3. Which motor to choose? The regular N20 motor or the big N20 motor? Looks confusing. Motor mount looks complicated. Sketch. How to find motor torque in this case?8

# Design Ideas and To-do
1. ~~Flexure bearing iteration~~
2. ~~Box cross section vs I-Beam cross section~~
3. *Potential variable stiffness mechanism. Removing/Adding leaf spring introduces/eliminates flexibility, check out that one paper which has an underactuated geartrain as a finger.*
4. Refer [[Mathematics for Designers]] for more ideas, working on origami based underactuated universal gripper.
5. Multi-segmented rollers with pairs of toothed belts as a new concept.
6. Toothed belt iteration
7. Simulation of Closed Kinematic Chains in Realistic Environments Using Gazebo
8. https://www.youtube.com/watch?v=cTdnpNoJXaw circlip for bearing
9. Four bearings per axis??
10. Globoid worm, mated pair is helical gear. Very efficient. Single start, multi-start better. 3-4 start. 
11. Crossed helical gear.
12. Need steel shafts, single shaft and axle throughout, not multiple.
13. Replace bearings with bushings at links, constrain bushings properly. Replace pulley sprocket with bearings at pulley. Will have like 2 bearings and 8 bushings per axle.
14. Bigger pulleys used for multisegmented links, teeth number =15 (prev was 12)
15. Geartrain with pulleys and belts. The idea about belt slack. And using a pulley with tapered edge to compensate or using a pulley with springs that can give tension.

# Updates
#projects/graspman/updates
#dailies
- [x] Unified model for graspman, discuss with Param
- [x] Discuss with Karthik sir and Mani sir for including bearings in motor mounts.
- [x] Simplified model for motor mounts
- [x] For now, direct drive is fine., model it.
- [x] Prepare a model with Idea 5 from Design Ideas and To-do
- [x] Print entire model by 26th Feb 2025
- [x] Circlip for bearing, too much wobble. 
- [x] Cleaner belt iteration, Z-retract is enabled tho... check it once. 
- [x] Dump all, choose belt from misumi/mcmaster/Gates/Fenner/Conti-tech and respective pulleys. Calculate center to center distance and design link.
- [x] Solid wobble-less design.
- [x] [Belt choosing wiki](https://reprap.org/wiki/Choosing_Belts_and_Pulleys) 
- [ ] Shank bolts, can be used as ball bearings too
- [x] Check misumi for belts nearby and buy it. ASAP send order request by March 4th evening
- [x] purchase rotary shafts
- [x] For belt in grooves, give 1-1.5mm clearance to prevent bites or just chamfer belt (if printed)
- [x] Different motor for mount, figure out position. Avoid previous design. Figure out merits from it and use it.
- [x] Cantilever motor mount. if XL330 is used, we get planned obsolescence
- [ ] Reduced weight model: Reduce weight by removing al-pulleys and use static shafts- i.e bearings replace the role of al-pulleys. But same 8 bearings or 6 bearings per axle. Further optimization tasks
- [x] Bigger pulley model: Increase the pulley size, and fabricate belts accordingly. XL type belt, 5.08mm pitch and 25 teeth. #belts 
- [x] Bigger pulleys used, teeth number : 15 (previous had 12 teeth)
397g without bearings and C-link (now 375g)
Bearings mass = 5g x 4 per axle x 9 axles == 180g
total mass = 580g excluding c-link
+100g == 680g per finger
now its around 375+180+100=655g
128mm hehe
# Issues
- [x] Some wobble, due to washers not being flat.
- [x] Belt bites, try filleting edges
- [x] A bit too tight.... figure why?
- [x] 8 Bearings per axle bro
- [ ] Per link, above horizontal axis range of motion is only 68 degrees. This is roofed to 68.
- [ ] 44.5mm shaft min, need 45mm shaft needed for idler gears
- [ ] 85mm shaft needed, on spot no room for extras. Need to verify if this approach is okay.
- [ ] so like 255+280+20 = 555g per finger

# Items
- [ ] [GT2 belt](https://in.misumi-ec.com/vona2/detail/110302652060/?HissuCode=GBN1162GT-90) required length is approx 115mm, around that range. pitch was 5.08mm, need xl or 3gt belt. Timing belt only. Thickness less than 1mm. A quote for approx 10 belts
- [x] [GT3 belt](https://in.misumi-ec.com/vona2/detail/110302652150/?HissuCode=GBN1173GT-150) 15mm thickness
- [ ] [Nylon filament](https://robu.in/product/esun-epa12-white-1kg-spool/) PA12 Rs. 6.5k
- [x] [Shafts](https://www.desertcart.in/products/241013218-sourcing-map-a15113000ux1262-5-pcs-5mm-x-100mm-diy-rc-car-model-straight-metal-round-shaft-rod-bars-pack-of-5) desert cart
- [x] [Shafts](https://www.amazon.in/Invento-2pcs-Smooth-Rod-5mm/dp/B078P46JZ5?source=ps-sl-shoppingads-lpcontext&ref_=fplfs&psc=1&smid=AJ6SIZC8YQDZX) Amazon, 5mmx300mm qty=2
- [x] [Pulleys](https://robu.in/product/aluminum-gt2-timing-pulley-6mm-belt-16-tooth-5mm-bore-2pcs/) checkout with grub screws, qty=2
- [x] 5x9x3 bearings from India Bearings @ Rs.40/piece
- [ ] [2GT with 3mm bore](https://www.amazon.in/MECCANIXITY-Aluminium-Synchronous-Printer-Machine/dp/B09VPRLCB7?th=1) Pack of 2 costs like Rs 2.2k
- [ ] [Flanged coupler](https://www.amazon.in/uxcell-Flange-Coupling-Coupler-Connector/dp/B07PDZCTLH) Decent option on amazon.
- [ ] [Double head pulley](https://www.amazon.in/3DINNOVATIONS-Double-Timing-Pulley-Printer/dp/B07K1LZ4CY) on amazon, for gear-pulley connection
- [ ] 210-40= 170 bearings
- [ ] 5mm shafts

# Report
Weight issues are a thing. Right now here is a split up of the total weight.
Total gripper weight: 2173 grams

Necessary mass: 655g, removing al-pulleys and shafts (basically use plastic shafts)
Below table is per gripper finger:

| Part              | Weight (g) |
| ----------------- | ---------- |
| 3d printed pulley | 102.41     |
| Links             | 46.82      |
| Al-Pulleys        | 280        |
| Bearings          | 371.2      |
| Shaft             | 146.36     |
| C-Link            | 102.44     |
| N20 motor setup   | 12         |
| Belts (10)        | 20.36      |
```chart
type: pie
labels: [3d printed pulley,Links,Al Pulleys,Bearings,Shaft,C-Link,N20,Belts]
series:
  - title: Weight distribution
    data: [102.41,46.82,280,371.2,146.36,102.44,12,20.36]
tension: 0.2
width: 70%
labelColors: true
fill: false
beginAtZero: false
bestFit: false
bestFitTitle: undefined
bestFitNumber: 0
```

[Tensioning of a belt, refer this setup and procedure](https://tameson.com/pages/v-belt-tensioning)

# Calculations
torque = 1.5 N.m
Spring travel angle is around 45 degrees
Spring rate constant= 1.5/45 -> 0.033 N.m/degree
XM540 motor specs : [[xm540_motor.pdf]]


## Spring Design
got it from McMasterr
![[Pasted image 20250523165954.png]]
Max torque: 0.33in-lbs -> 0.03 Nm
required -> 0.017 Nm

Springs configuration: Deflection angle: 315 degrees, for shaft dia: 6mm, wire diameter: 0.6mm, leg length: 2.5cm, number of coils: 8.63, Material: Music-wire steel
# Onsite to-do:
 - [ ] Detailed documentation for various graspman iterations.
 - [x] How to address the elephant in the room? (current belt andd gears not optimal enough)
 - [ ] Wiring problem. N20 motor wires can be routed inside the c-link (hollow)
 - [x] Purchase screws and bearings for final assembly. Missing M3 screws.
 - [ ] Pay Sivanand sir 1033.33 rs when reimbursed along with kc sir amount --> Pay KC sir.
 - [x] By wednesday-28 May 2025, complete tests for slipping. Add springs and belts and check.
 - [x] Basic model to engage and disengage motor like a clutch or sth. Sth like a knob to freewheel the motor.
 - [x] Purchase filament
 - [x] fatmax order
 - [x] coreless motor for freewheel operation
 - [ ] Purchase m1.5/m1 screws for n20 motor mount.
 - [ ] Future iteration: Remove geartrain, use multi-segmented links for conformance, have multiple smaller discs freely rotating and support the belt

## Freewheel the motor:
- Ratchet screw driver concept: turn a knob to freewheel in either directions
- Sliding motor concept: Slide the motor horizontally and lock it out of place to freewheel.
- Reaction torque concept: Use BambuLab AMS as an inspiration. The motor drive system consists of two gears (idk couple gears?) The motor engages the connecting gear () Initially it's disconnected. But the reaction torque connects it to the geartrain or drive system.


[[graspman_paper.pdf#page=3&selection=331,23,352,36|graspman_paper, page 3]]
what does this mean

![[Pasted image 20250528155230.png]]
Ft= F of Tight side
Fs= F of Slack side
Fc= circumferential force
[Link for the above](https://www.tec-science.com/mechanical-power-transmission/belt-drive/power-transmission-of-a-belt-drive/)
Pre-tension force (30N):
$$
F_t+F_s=2.F_p
$$
Torque required:
$$
\tau=r\times(F_t-F_s)
$$
and
$$
F_t-F_s=F_c
$$

$$
F=T_1+T_2=30
$$
$$
r\cdot(T_1-T_2)=\tau
$$


$$
K_{eff} = K_1+K_2
$$
$$
F_1 = I.T+K\cdot x_1
$$
Spring contact:
what details required to make spring?
we need around 6-8 springs.
Our springs spec:
- Spring outer diameter: 18mm
- wire diameter: 2.3mm
- free length: 75mm
- material: SWP-A (piano wire)
- Maximum load: 115.72 N
- Maximum Deflection: 25mm

GT2 belts very precise based on sdp book and the reprap society (they use gt2 pulleys for 3d printers)
GT2 vs trapezoidal belts, depends only on thickness and length. Although GT2 known to be slightly better than trapezoidal overall


## 16th June 2025
#meet

So in 45 days, need a product.
Gripper: 
Topology optimization of the frame for weight reduction (for entire graspman)
Revolute joint instead of prismatic joint
Question every screw? Value engineering
Another week for design
Maximum force aha, how much?
## karthik sir call on 18th June 2025
- proxxon tools
- intel i9 14900k vs i7 14700k
- amd 7 series 9800 x 3d 9700x 120w tdp 
- 100+tabs
- 20+videos
- gpu - 5060ti 16gb 48k and amd 9060xt tuf version


## Call and talk with sir the following points:
- What experiments?
- Focus on set few experiments and scale later
- Gripper very simple, why have within hand manipulation?

> [!NOTE] Note
> Everything is a suggestion, very hard to convince.

prioritising by list of exp? ask when we do that?
cart sliding

digressing da skicj to the agenda daw
inverted pendulum

actually we have modulur setup can we test the inverted pendulum? now!
then what motor?
what are the other experiments we should look at? 

things are going somewhere peacee..........
ask all the list of experiments now ask asap

then y sticking with dynamixel?
y not going that route

we will put effort over there
internal supplier gor motor is actually from india can we speak over there
class
locomotion (walking, legged)
control
inverted
manipulation with one g
pipe climbing
dynamic modelling
poition velocity and torque contol
gain tuning 
perturbation
force and form closure


2942rs
4644rs
purchase reimbursement


## Ideas 
#ideas
Alternate up and down of the drive GT2 pulley to keep space to a minimum.

bro apde chuma out of topic la ask him if he has 3d pen


40.04mm delta y, 19.64 delta x

offset adapter, used in japan cuz tight spaces crammed