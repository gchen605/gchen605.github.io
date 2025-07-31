---
title: "3D Printing for Life Scientists"
date: 2025-07-30
permalink: /resources/3d-print
collection: resources
author_profile: true
---

This is a short primer on getting started with 3D printing for the laboratory.

# Sections

1.  [Definitions](#definitions)
2.  [Basic workflow (aka: I found something online I want to print)](#basic-workflow)
3.  [Advanced workflow (aka: I want to design my own stuff to print)](#advanced-workflow)

# Definitions

## What is 3D printing? 
3D printing is an automated additive manufacturing process. There are numerous technologies for 3D printing, but for the purposes of this guide, we will ficus on the most commonly used one, called FFF (Fused Filament Fabrication) in which an object is created layer by layer by melting a strand of plastic.

## What printer do we have?
We currently have a [Prusa Core One](https://www.prusa3d.com/product/prusa-core-one/)

## What can we print?
Anything that can fit in the build volume (unless you want to break a model up into multiple pieces.

## Are 3d-printed parts food-safe?
I wouldn't try it, unless they are coated in a food-safe epoxy.

## What types of materials can we print?
The most frequently used filaments are PLA, PETG, and ASA. 

### PLA
**Pros:**
* It’s easy to print. 
* No unpleasant odor during printing
* Low thermal expansion compared to other materials. It does not warp, and sticks to the printing platform nicely. This is why it’s suitable for printing large objects.
* PLA comes in a wide variety of colors.
* One of the cheaper materials

**Cons:**
* PLA is hard and brittle. It has a tendency to break and shatter under pressure.
* PLA is not temperature-resistant, it starts to soften at around 60 °C (140 °C), which makes it a less-than-ideal choice for printing things like car smartphone holder.
* Compared to the rest of popular materials, PLA has the worst weather resistance.

### PETG & ASA
**Pros:**
* More flexible than PLA
* Shinier finish
* UV Stable, lower thermal expansion

**Cons:**
* Tend to bend and warp during printing
* Noticeable odor during printing

### TPU/TPE
* Rubber-like flexibility

---

# Basic workflow
**AKA I found something online I want to print** <br>
There are 3 main steps to 3D printing:
1. Get a printable 3D model: Usually an STL or OBJ file, these are widely shared online
2. Prepare the file for printing: Using a 'slicer' software package, prepare the model file for printing. The slicer exports a 'G-code,' which is a printer-specific set of instructions that include information about temperature, output speed, etc.
3. Print it

## 1. Get a printable 3D model
- [Printables](https://www.printables.com/)
- [Thingiverse](https://www.thingiverse.com/)
- [MyMiniFactory](https://www.myminifactory.com/)
- [Cults3d](https://www.cults3d.com)
- [Yeggi 3D model search engine](https://www.yeggi.com)
- [NIH 3D Print Exchange](https://3d.nih.gov/)

## 2. Prepare the file for printing
Slicing is the process of turning a 3D object into a machine code called G-code using a software tool called a slicer. The input for the G-code generation is not just a 3D object, but various settings as well – like the toughness of the model, amount of details or printing speed. It’s also possible to modify the objects – scaling, rotating, cutting and other tools are available. Last, but not least – you can use slicers to position the object(s) on the virtual printing surface. 

The most common slicer software:
- [PrusaSlicer](https://www.prusa3d.com/page/prusaslicer_424/)
- [Ultimaker Cura](https://ultimaker.com/software/ultimaker-cura/)

### Basic things to consider:
1. Layer height/Level of detail/Resolution: Higher values = faster prints but more visible layers. PrusaSlicer has an "Adaptive layer height" option to change height based on geometry.
2. Perimeters: How thick are the walls?
3. Infill: How much of the interior is filled. Generally 10-20% is enough for most parts. Load-bearing parts should be made 50-70% infill. Rarely is 100% necessary.
4. Supports: Scaffolding structures that support overhangs or parts that start mid-air. These are designed to be easy to remove but they may leave marks on the model. "Organic supports" mimic tree growth and result in faster printing and less waste
5. Orientation: Since the model is printed layer by layer, if force is going to be applied to it, it will easily shear on those layer lines; recommend rotating the model 30-45 degrees for increased strength
6. Adhesion to build plate:
	* Brim: Additional flat surface to prevent object from warping/detaching mid-print
	* Skirt: An outline around all the models on the print bed. Doesn't help the model adhere but helps quickly verify that first layer is sticking properly
	* Raft: A heavy-duty support structure to prevent warping/lifting from the print surface

## Printing the model
1. Save the G-Code to a flash drive
2. Turn on the printer (rear of machine)
3. Check to see that the correct filament is loaded (If not, see Changing Filament)
4. Clean build plate (Use a kimiwipe + isopropyl alcohol)
5. Plug in flash drive
6. Print
7. With gloves, remove build plate once cool and **gently** bend to pop off the model (may need to use plastic spatula to help remove model.
	**DO NOT USE METAL OBJECTS ON BUILD PLATE!**
8. Clean up any extra plastic in printer
9. Turn off machine

---

# Advanced Workflow
**AKA I want to design my own stuff to print** <br>

I am going to rely on you learning how to CAD on your own, but here are some software packages to get you started.
* [Tinkercad](https://www.tinkercad.com): Super intuitive and easy to use. Free but registration is required. 90% of what I've needed to design I can at least get started on Tinkercad.
* FreeCAD
* Autodesk Fusion
* Solidworks

## Things to consider when designing a model:
1. Try to minimize the need for supports
2. Decide how the model will be positioned on the printer - will shear forces be applied in any direction? Does a surface need to be smoother than others?
3. Consider splitting a model into multiple parts if there are overhangs/low adhesion points (eg. a sphere printed as 2 halves and glued together will look better than printed all at once.
4. Consider tolerances when modeling parts to fit together. There's no universal rule, but generally a minimum of 0.15mm difference should be included.
5. Circular holes printed vertically won't be perfectly circular.
6. Walls must be about 0.45mm at minimum

---

# Other Resources
* [Reddit 3D Printing](https://www.reddit.com/r/3Dprinting/)
* [Making Models](https://www.reddit.com/r/3Dprinting/wiki/makingmodels)