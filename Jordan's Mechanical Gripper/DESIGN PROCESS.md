# Mechanical Gripper - Design Process

This document summarizes the design process and final dimensions of the custom components used in the mechanical gripper.

All dimensions are in millimetres.

For the SolidWorks part files, see the **"Parts" folder**.

For the engineering drawings, see the **"Drawings" folder**.

For views of the completed assembly, see the **"SolidWorks Angles" folder**.

---

# 1. Gripper Base

The base provides the main structural support for the mechanism. It supports the two finger pivots and provides a guide slot for the center slider.

## Final Dimensions

| Feature | Dimension |
| --- | ---: |
| Overall base | 120 × 120 × 8 mm |
| Main pivot holes | 2 × Ø6.5 mm |
| Pivot spacing | 80 mm center-to-center |
| Left pivot center | X = 20 mm, Y = 80 mm |
| Right pivot center | X = 100 mm, Y = 80 mm |
| Center opening | 50 × 70 mm |
| Opening side spacing | 35 mm |
| Opening bottom | 50 mm from base bottom |
| Lower opening fillets | R5 mm |
| Outer fillets | R5 mm |
| Slider slot width | 7 mm |
| Slider slot overall length | 35 mm |
| Slot center X | 60 mm |
| Slot center Y | 24.1 mm |

A large center section was removed from the original base because the area was unused and blocked visibility and movement around the fingers.

The outside edges were also reduced to make the final base more compact.

See the finished base model in the `parts` folder and its dimensioned drawing in the `drawings` folder.

---

# 2. Gripper Fingers

Two identical fingers form the main moving arms of the gripper.

Each finger rotates about an M6 bolt mounted to the base and connects to a linkage near the bottom.

## Final Dimensions

| Feature | Dimension |
| --- | ---: |
| Quantity | 2 |
| Overall size | 16 × 115 × 8 mm |
| Holes | 2 × Ø6.5 mm |
| Hole centerline | 8 mm from either side |
| Lower linkage-hole center | 10 mm from bottom |
| Main pivot-hole center | 35 mm from bottom |
| Hole spacing | 25 mm center-to-center |

The fingers were constrained using limit-angle mates to prevent the mechanism from being dragged beyond its intended range.

Final angle range:

- Minimum: 70°
- Maximum: 90°

See the finger model in the `parts` folder and its drawing in the `drawings` folder.

---

# 3. Connecting Links

Two connecting links transfer the vertical motion of the center slider into rotation of the two gripper fingers.

## Final Dimensions

| Feature | Dimension |
| --- | ---: |
| Quantity | 2 |
| Overall size | 59 × 14 × 5 mm |
| Holes | 2 × Ø6.5 mm |
| Hole spacing | 45 mm center-to-center |
| Hole centers from ends | 7 mm |
| Rounded ends | R7 mm |

Each connecting link is mounted between one finger and the center slider.

See the connecting-link model in the `parts` folder and its drawing in the `drawings` folder.

---

# 4. Center Slider

The center slider provides the main linear input to the mechanism.

Moving the slider vertically causes both connecting links to move at the same time, producing approximately symmetric finger movement.

## Overall Dimensions

| Feature | Dimension |
| --- | ---: |
| Overall size | 40 × 30 × 8 mm |
| Holes | 4 × Ø6.5 mm |

## Hole Locations

Locations are measured from the bottom-left corner of the slider.

| Hole | X | Y |
| --- | ---: | ---: |
| Left linkage hole | 10 mm | 15 mm |
| Right linkage hole | 30 mm | 15 mm |
| Lower guide-pin hole | 20 mm | 7.5 mm |
| Upper guide-pin hole | 20 mm | 22.5 mm |

Guide-pin spacing:

**15 mm center-to-center**

Two pins guide the slider through the vertical base slot.

An additional guide pin was used as the manual handle for operating the mechanism.

See the slider model in the `parts` folder and its drawing in the `drawings` folder.

---

# 5. Gripper Jaws

Small jaw pads were added to the ends of the fingers to improve gripping contact.

## Final Dimensions

| Feature | Dimension |
| --- | ---: |
| Quantity | 2 |
| Overall size | 10 × 20 × 8 mm |
| Gripping-edge fillets | R2 mm |
| Number of grooves | 3 |
| Groove size | 6 × 1 mm |
| Groove depth | 0.75 mm |
| Groove spacing | 5 mm center-to-center |

The three groove centers are located approximately:

- 5 mm from the bottom
- 10 mm from the bottom
- 15 mm from the bottom

The grooves were added to provide more surface texture at the gripping face.

See the jaw model in the `parts` folder and its drawing in the `drawings` folder.

---

# 6. Guide Pins

The guide pins are simple cylindrical parts used with the center slider.

## Dimensions

| Feature | Dimension |
| --- | ---: |
| Diameter | Ø6 mm |
| Length | 16 mm |

Two guide pins are used to control the center slider.

A third pin of the same design is used as the manual handle.

See the guide-pin model in the `parts` folder.

---

# 7. Linkage Pivot Pins

Custom pivot pins were created for the four linkage joints.

## Dimensions

| Feature | Dimension |
| --- | ---: |
| Quantity | 4 |
| Shaft diameter | Ø6 mm |
| Shaft length | 13 mm |
| Head diameter | Ø10 mm |
| Head thickness | 2 mm |

These pins allow the connecting links to rotate relative to the fingers and center slider.

See the pivot-pin model in the `parts` folder.

---

# 8. Main Pivot Hardware

The two gripper fingers are attached to the base using standard M6 hardware.

## Hardware Used

- 2 × M6 × 25 mm ISO 4017 hex bolts
- M6 ISO 7089 plain washers
- M6 ISO 4032 nuts

The hardware was inserted using the SolidWorks Toolbox.

---

# 9. Assembly

After the individual components were modeled, they were inserted into a SolidWorks assembly.

The main assembly process included:

1. Fixing the gripper base.
2. Mounting each finger to the base.
3. Adding the two connecting links.
4. Connecting the links to the center slider.
5. Adding linkage pivot pins.
6. Adding M6 finger pivot hardware.
7. Adding the slider guide pins.
8. Adding the gripper jaw pads.
9. Adding the manual slider handle.
10. Adding motion limits.

The completed mechanism allows the user to manually move the slider and open or close both jaws.

Different views of the completed assembly are available in the `solidworks angles` folder.

---

# 10. Design Changes

Several changes were made while developing the final design.

## Base Clearance

A large section was removed from the center of the base because the original solid plate blocked the fingers and contained unused material.

Final opening:

**50 × 70 mm**

The lower corners were given:

**R5 mm fillets**

## Reduced Base Width

Unused material along the outside edges of the original base was removed to create the final:

**120 × 120 mm base**

## Finger Travel Limits

When the mechanism was dragged too far, the links and fingers could move into unrealistic positions.

Limit-angle mates were therefore added to keep the fingers within their intended range:

**70° to 90°**

## Manual Handle

A guide pin was added to the center slider and used as a simple manual handle.

This allows the mechanism to be operated without adding a motor or actuator.

## Jaw Grooves

Three grooves were added to each gripping surface to improve the jaw geometry and provide additional gripping texture.

---

# 11. Final Motion Measurements

The completed CAD mechanism was manually moved between its open and closed positions.

## Measurements

| Measurement | Value |
| --- | ---: |
| Maximum jaw opening | 44.00 mm |
| Minimum jaw opening | 1.05 mm |
| Total jaw-gap change | 42.95 mm |
| Slider travel | 9.14 mm |
| Approximate travel per jaw | 21.48 mm |

The center slider and handle travel approximately:

**9.14 mm**

between the measured open and closed positions.

---

# 12. Engineering Drawings

Engineering drawings were created after completing the final CAD design.

The drawing set includes:

- Mechanical gripper assembly
- Gripper base
- Gripper finger
- Connecting link
- Center slider
- Gripper jaw

All drawings are available in the:

**"Drawings" folder**

---

# 13. SolidWorks Models

Individual component models can be found in:

**"Parts" folder**

The completed assembly views can be found in:

**"SolidWorks Angles" folder**

The repository also contains the final STEP assembly file for viewing the complete model in compatible CAD software.

---

# 14. Skills Practiced

This project was used to practice:

- SolidWorks part modeling
- Assembly design
- Mechanical mates
- Limit-angle mates
- Mechanical linkage design
- Pivot joints
- Standard hardware
- Interference checking
- Basic motion testing
- Engineering drawings
- Basic kinematic measurements
- Design iteration

---

# Final Design

The final result is a manually actuated, symmetric two-finger mechanical gripper.

The project was primarily focused on learning mechanical CAD design and understanding how individual components interact inside a working linkage mechanism.

Material was not specified because the project focused on geometry, assembly design, and mechanism development rather than manufacturing material selection.
