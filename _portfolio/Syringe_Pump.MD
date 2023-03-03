---
title: "Syringe Pump"
excerpt: "DIY syringe capable of a 1 uL/min flow rate up to a 10 mL/min flow rate."
header:
  image: /assets/img/Syringe-Pump_ IsometricView.jpg
  alt: "Isometric view of syringe pump rendering"
  teaser: /assets/img/Syringe-Pump-Rendering_IsometricView.png
gallery:
  - url:/assets/img/Syringe-Pump-Rendering_IsometricView.png
    image_path: /assets/img/Syringe-Pump-Rendering_IsometricView.png
    alt: "Isometric view of syringe pump rendering"
  - url:/assets/img/Syringe-Pump_IsometricView.png
    image_path: /assets/img/Syringe-Pump_IsometricView.png
    alt: "Isometric view of syringe pump"
  - url:/assets/img/Syringe-Pump-Rendering_Alt-IsometricView.png
    image_path: /assets/img/Syringe-Pump-Rendering_Alt-IsometricView.png
    alt: "Alternate isometric view of syringe pump rendering"
  - url:/assets/img/Syringe-Pump-Rendering_SideView.png
    image_path: /assets/img/Syringe-Pump-Rendering_SideView.png
    alt: "Side view of syringe pump rendering"
  - image_path: /assets/img/Syringe-Pump- Rendering_ SideView.jpg
    alt: "Side View of Syringe Pump Rendering"
  - url:/assets/img/Syringe-Pump_SideView.png
    image_path: /assets/img/Syringe-Pump_SideView.png
    alt: "Side view of syringe pump"

---
## Features

## Required Parts

| Off-the-Shelf parts | 3D Printed parts |
| :---: | :---: |
| 200 mm lead screw w/ 2 mm pitch & lead | Pump Base (Bottom) |
| 1/4" x 8 mm flexible coupler | Pump Base (Top) |
| 200 mm linear rod with 8 mm diameter | Syringe Body Support |
| LM8UU linear bearing for 8 mm diameter rod | Syringe Plunger Support |
| Nema 17 Stepper Motor |Motor Mount |
| MEAN WELL RQ-65D AC-DC Power Supply Quad Output 5V 12V 24V 12V 4 Amp |
| Arduino Uno |
| A4988 Stepper Driver |
| Small Breadboard |
| Panel Mount Latching Push Buttons |
| Limit Switch |
| RGB Common Cathode LED |


<!--
#### 3D Printed parts
| Pump Base (Bottom) |
| Pump Base (Top) |
| Syringe Body Support |
| Syringe Plunger Support |
| Motor Mount |
-->

## Arduino Code
[Syringe Pump Arduino Code](/assets/img/Syringe_Pump_Arduino_Code.MD)

## CAD Model
<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH35dfcQT936092f0e4320bbce97815dc8f2?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

## Operation Procedure

  To operate syringe pump, make sure the middle support structure is directly in front of the coupler at the “starting position”. Place the syringe (20mL or 5mL) into the corresponding “mold” that supports the body of the syringe. The nose of the syringe should be resting on the smaller semicircle depression with the wings of the pump secured in the slits. Ensure that the circular back end of the plunger is firmly fixed in the slits of the middle support structure that will be operating along the lead screw. Specify the desired flow rate in the Arduino IDE program. The LED on the syringe pump should be red. Once the red button on next to the LED is pressed, the LED should turn from red to green. Simultaneously, the stepper motor will begin to turn the flexible coupler, which in turn will rotate the lead screw at a calculated rate of steps per millimeter, pushing the middle support structure and the back end of the plunger forward along the linear rod and compressing the syringe. If the red button is pressed at any time after the green light and before the syringe is completely compressed, the LED will turn yellow and the system will pause. If the button is pressed once more, the LED will turn green again and the motion of the system will continue. When the syringe is completely decompressed, the switch will be triggered and the LED will turn red. Simultaneously, the stepper motor will stop turning the flexible coupler, stopping the rotation of the lead screw. The back support of the plunger will also stop moving along the linear rod. 

{% include gallery caption="Syringe Pump Gallery" %}
