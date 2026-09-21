# Jordan's Mechanical Gripper

A manually actuated mechanical gripper designed in SolidWorks.

The mechanism uses a vertically moving center slider connected to two links. The links rotate two opposing fingers around fixed pivots, creating symmetric opening and closing motion at the jaws. A manual handle attached to the slider provides the input motion.

![Mechanical Gripper Front View](SolidWorks-Images/mechanical-gripper-front.png)

## Project Overview

This project was created to practice mechanical CAD, linkage design, assembly mates, motion constraints, engineering drawings, and basic kinematic analysis in SolidWorks.

The final design includes:

- Symmetric two-finger gripping mechanism
- Center slider actuation
- Connecting-link mechanism
- Replaceable grooved jaw pads
- M6 pivot hardware
- Guide pins and manual slider handle
- Limited finger travel using angle mates
- Reduced-material base plate
- Engineering drawings for the main custom components

## Final Performance

| Parameter | Final Value |
| --- | ---: |
| Maximum jaw opening | 44.00 mm |
| Minimum jaw opening | 1.05 mm |
| Total jaw-gap change | 42.95 mm |
| Slider travel | 9.14 mm |
| Individual jaw travel | 21.48 mm |
| Average total jaw-motion ratio | 4.70:1 |
| Average individual-jaw motion ratio | 2.35:1 |

## Main Dimensions

| Component | Dimensions |
| --- | --- |
| Base plate | 120 × 120 × 8 mm |
| Center opening | 50 × 70 mm |
| Finger | 16 × 115 × 8 mm |
| Connecting link | 59 × 14 × 5 mm |
| Center slider | 40 × 30 × 8 mm |
| Jaw pad | 10 × 20 × 8 mm |
| Guide pin / handle pin | Ø6 × 16 mm |
| Linkage pivot pin | Ø6 × 13 mm shaft, Ø10 × 2 mm head |
| Main pivot hardware | M6 × 25 mm |

Material was not specified because the focus of the project was mechanical design and CAD development.

## Engineering Drawing

![Mechanical Gripper Engineering Drawing](Engineering-Drawings/mechanical-gripper-final-drawing.png)

Individual drawings for the base, fingers, connecting links, center slider, and jaws can be found in the `Engineering-Drawings` folder.

## Mechanism Demonstration

A manual motion demonstration of the completed assembly is included here:

[View the mechanical gripper motion demo](Videos/mechanical-gripper-motion-demo.mp4)

The handle moves the center slider vertically. The connecting links transfer this motion to the fingers, causing the jaws to open and close symmetrically.

## CAD Files

The final complete assembly is available as:

`Mechanical-Gripper-Final.step`

Individual SolidWorks part files are located in the `Parts` folder.

## Repository Structure

```text
Mechanical-Gripper/
├── README.md
├── Mechanical-Gripper-Final.step
├── Engineering-Drawings/
├── SolidWorks-Images/
├── Parts/
├── Videos/
└── Design-Process/
