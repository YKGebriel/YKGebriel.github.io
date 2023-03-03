---
title: "Print-in-place Pliers"
excerpt: "Pliers composed of multiple materials printed on dual extrusion printer"
header:
  image: /assets/img/MM-Plier.png
  alt: "Mult-material, print-in-place plier"
  teaser: /assets/img/MM-Plier.png
gallery:
  - url: /assets/img/MM-Plier.png
    image_path: /assets/img/MM-Plier.png
    alt: "Mult-material, print-in-place plier"
  - url: /assets/img/MM-Plier-Rendering_IsometricView.png
    image_path: /assets/img/MM-Plier-Rendering_IsometricView.png
    alt: "Isometric view of mult-material, print-in-place plier"
  - url: /assets/img/FlexPlierJoint-Rendering_IsometricView.png
    image_path: /assets/img/FlexPlierJoint-Rendering_IsometricView.png
    alt: "Isometric view of print-in-place flexible plier joint"
  - url: /assets/img/MM-Plier-Rendering_TopView.png
    image_path: /assets/img/MM-Plier-Rendering_TopView.png
    alt: "Top view of mult-material, print-in-place plier"
  - url: /assets/img/FlexPlierJoint-Rendering_TopView.png
    image_path: /assets/img/FlexPlierJoint-Rendering_TopView.png
    alt: "Isometric view of print-in-place flexible plier joint"
  - url: /assets/img/MM-Plier-Rendering_AngledSideView.png
    image_path: /assets/img/MM-Plier-Rendering_AngledSideView.png
    alt: "Angled side view of mult-material, print-in-place plier"
   
---
## Project Description

|  Print-in-place models are functional multiple-component designs which work immediately after removal from the print bed. Unlike other multiple-component models, these models require no post-processing or assembly.

|  Print-in-place models can be created through the extrusion of a single material by carefully designing models and orienting the prints to allow for clearance between printed joints where motion or rotation is needed. However, even with optimized print settings, print-in-place models can be plagued by discrete, non-fluid movement due to the irregularities of plastic extrusion. As such, an alternative method to obtain useful motion in print-in-place models is to include a flexible component in the model, such as a thin piece of a rigid plastic or a second elastomeric material. This flexible component allows for an easier transmission of force within the model resulting in a more fluid movement as the model moves through its range of motion.

|  The objective of this project was to design and fabricate a needle nose plier capable of picking up pellets with an approximate diameter of 3 cm. The pliers need to be able to grip the pellets before then moving them to another location and releasing them. Additionally, the pliers needed to contain a spring component made from a flexible material, in this case thermoplastic polyurethane (TPU) 95A, that would return the pliers to their open position when not in use.

## Design Features


## Plier Specifications
* Jaw Length: 3 cm
* Jaw Capacity: 0.5 cm
* Jaw Thickness: 0.6 cm

## Print Settings
### Filament Settings

| Filament | PLA | TPU 95A |
| :---: | :---: | :---: |
| **Extruder Temp** | 215 C (*first layer*), 210 C (*subsequent layers*) | 240 C |
| **Bed Temp** | 60 C | 60 C |
| **Max Print Speed** | --- | 25 mm/s |
| **Retraction Speed** | 40 mm/s | 15 mm/s |

### Printer Settings

|  The optional wipe tower feature was enabled during the print of the multi-material print-in-place pliers. In order for the MakerGear M3 IDEX 3D printer to transition between materials during the printing process, both nozzles must be keep near the printing temperature for their corresponding filament. This means that as one nozzle is extrudes filament the other, while not programmed to extrude anything at this point in the process, still leaking molten filament away from the build plate. This leaked material can then be caught on the designed part the next time the nozzles change.
  
|  By enabling the wipe tower feature, every time there is a nozzle/tool change, the new extruder will lay down a layer of filament away from the desired part before then moving to lay down the next layer of the designed part. This allows the extruder time to purge the discharged filament as well as any molten material in the nozzle and prime new filament for the next layer of the designed part. As this process occurs with every tool change, the end result is the creation of a distinct structure separate from the desired part composed of material from both extruders.

## CAD Model
<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH35dfcQT936092f0e4374907dc0d2424dfb?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

{% include gallery caption="Print-in-place Plier Gallery" %}
