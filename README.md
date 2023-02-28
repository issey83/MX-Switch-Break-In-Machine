# MX Switch Break-In Machine
A simple machine designed to actuate/ break-in MX style switches consistently and repetitively for a smoother push feel. Watch the [assembly process and operation](https://www.youtube.com/watch?v=iYIlCdo38ZM&list=PLLd9RKaLkD3lO_kQBJ3w394Xko4Nm3RR9) of the machine here.

![alt text][snapshot]

[snapshot]: /Images/DSC05789.jpg "Machine Snapshot"

## Specifications
- Max number of switches: 36
- Compatibility: 
  -  MX style switches with total travel distance of 4mm
  -  MX style switches with total travel distance less than 4mm (tweaks required for this)

## Notes ⚠️
- The provided files are to be used at your own risk.
- The dimensional tolerances may vary between 3D printers. See acceptable tolerances under [`Production/Technical-Drawings`](/Production/Technical-Drawings).
- The complete units showed in pictures and videos shared in this repo were printed with [JLCPCB 3D printing service](https://cart.jlcpcb.com/quote), with material of 8000 Resin, and remarked to print at an 30/45 angle for better Z-axis accuracy.
- Do ensure to run the machine at a ventilated area or fan-cooled to prevent the motor from overheating.

## Bill of materials (BOM) 📜
The following is the number of quantities required for each part to assemble a complete unit. The part files required to print are under the [`Production`](/Production) folder.

Parts required to print:
| Part                                                 | Qty        | Comment |
| ---------------------------------------------------- | ---------- | ------- |
| Actuation Plate                                      | 2          | -       |
| Off Center Actuation Plate                           | 4          | -       |
| Switch Holder                                        | 4          | -       |
| Flat Profile Keycap *or 10xFlat Profile Keycap*      | 36 *or 4*  | -       |
| Machine Housing                                      | 1          | -       |
| Machine Housing 1 *or 4xMachine Housing 1*           | 2 *or 1*   | -       |
| Motor-Adjuster                                       | 1          | -       |
| Scotch Yoke                                          | 1          | -       |

Parts required to purchase:
| Part                                 | Qty | Comment | References |
| ------------------------------------ | --- | ------- | ---------- |
| TT 1:90 Gearbox DC Motor             | 1   | Measured about 155 actutations/min, 5.4 hours for 50k actuations (measurement based on my purchased motor) | [link 1](https://shopee.sg/Large-Price-Metal-Gear-Robot-Smart-Car-Reduce-Speed-Motor-Tt-Motor-i.191993938.3917622642) |
| *or TT 1:48 Gearbox DC Motor*        | 1   | Motor runs hot over long run, measured about 400 actutations/min, 2.1 hours for 50k actuations (measurement based on my purchased motor) | [link 2](https://www.adafruit.com/product/3777) |
| HK 0306 Needle Roller Bearing        | 2   | - | [link 1](https://www.skf.com/us/products/rolling-bearings/roller-bearings/needle-roller-bearings/drawn-cup-needle-roller-bearings/productid-HK%200306%20TN) |
| M3 x 8mm Screw                       | 6   | - | - |
| M3 x 12mm Screw                      | 2   | - | - |
| M3 x 25mm Screw                      | 2   | - | - |
| Female USB C to 2-pin 22 AWG Wires   | 1   | - | [link 1](https://www.aliexpress.com/item/1005001388133794.html?spm=a2g0o.productlist.0.0.5eb0510fZ1x7CB&algo_pvid=72711e6a-5844-4e73-a4a4-c90b141b40e0&algo_exp_id=72711e6a-5844-4e73-a4a4-c90b141b40e0-16&pdp_ext_f=%7B%22sku_id%22%3A%2212000015898874380%22%7D) <br> [link 2](https://www.aliexpress.com/item/1005002271810476.html?spm=a2g0o.productlist.0.0.2819510fomHmwf&algo_pvid=a239c4db-a4cf-4337-b6a1-f4db0c4cff98&algo_exp_id=a239c4db-a4cf-4337-b6a1-f4db0c4cff98-2&pdp_ext_f=%7B%22sku_id%22%3A%2212000019849627354%22%7D) |
| 8mm Diameter Bumpons                 | 4   | Optional | [link 1](https://shopee.sg/MAGIC-100PCS-Sheet-Soft-Buffer-Sticker-Furniture-Accessories-Gel-Shock-Absorber-Rubber-Silicone-Pads-Cabinets-Door-Stop-Anti-collision-Toilets-Bumpers-Non-Slip-Self-Adhesive-Multicolor-i.299069493.11802920607) |

## To-Do 📝
- A guide on breaking-in switches that have shorter travel distance will be shared soon.

## Changelog 📒
- `05/02/2022:` Initial part files commit 

## Reach me at 📩
- Discord: https://discordapp.com/users/Yū#0001
  - Feel free to send me your enquires if you have doubt reproducing a unit for yourself.

---------------------------------------------------------------------------------------------------------
# FDM Printed, with modifications
Replaceable fan/motor without soldering, to be used with 12v power supply, or USB QC/PD trigger module for 12v output.

![alt text][snapshot2]

[snapshot2]: /Images/20220801_144157.jpg "FDM Printed, with fan." 

![alt text][snapshot3]

[snapshot3]: /Images/20221003_125454.jpg "PD/QC trigger, LM2596 with display, new fan mount" 

![alt text][snapshot4]

[snapshot4]: /Images/20221102_024117.jpg "Main housing with brass inserts, cable tie points." 

![alt text][snapshot5]

[snapshot5]: /Images/20221102_024127.jpg "Micro switch location, access hole." 

![alt text][snapshot6]

[snapshot6]: /Images/20221102_024145.jpg "8 digit counter." 

![alt text][snapshot7]

[snapshot7]: /Images/20221102_024512.jpg "Off center plate, with borders, fan mount with brass inserts, 42mm test hook." 

## Utilizing 
- QC/PD trigger module for 12v input, because QC/PD power brick better than regular usb port/charger
- LM2596 power supply module for voltage control, controling motor speed
- 12v 40x10mm fan, should be easy to source, and normally they come in XH connector
- XH 2.54 2pin header for fan
- 28mm aligator clips / 42mm test hook
- M3 x 4mm or M3 x 4.5mm brass inserts for frequent change of gearbox/motor assembly
- 8 digit counter found on taobao, https://item.taobao.com/item.htm?id=547288386556, I use H7EC-BLM, no need external power, battery last for 3-5 years according to description. 
- some soldering work
you can make this end user friendly, changing parts without soldering.

Changes made to STL files for 3d FDM printing.
1. Added marking to off center actuation plate, 3/3.5/4mm version. Mix and match to use with different switch's total travel, also to offset some printing errors, if any.
1.1. Added borders on off center plate, to prevent plate to press into main housing and causing arch.
2. Added fan mount, can be used with m3 x 8mm screw (might strip easy), or use with m3 x 12mm screw for a better hold. Screw length for the fan will depend on thickness of the fan you are getting, and if there's fan guard. for 10mm thick, I use m3 x 16mm.
2.1 New fan mount design, closer to motor, using motor's mounting screw, less material needed for printing. Brass insert optional, files provided.
3. Added keycap file for FDM printing, more tolerance, fit better. Can be used with dustproof stem as well. Closed off part is for east/west side of the stem, opening side face north/south, north/south is the leaf/led side of the switch.
4. New addition to main housing, some rings for cable management, soldered joint on wire is brittle, might break if they are moved frequent, tie them down. Also some place for fixing a micro switch, I think I got the right side position correct for a micro switch with lever + wheel attached, left side might not be. Use size M2 screw for holding the switch.

How I build and run them.
1. Ironing enabled for main housing, making sure the floor is flatter than regular printed parts.
2. Brass inserts, 3x4mm or 3x4.5mm, depth don't really matter, 3-4mm is fine.
3. Scotch yoke printed in nylon, actuation plate printed in ABS, fan mount printed in nylon/ABS.
4. Lubricate the floor of main housing, neck of actuation plate, scotch yoke with sw92sa from aliexpress, or any kind of lube for plastic (205g0 works too, expensive).
5. Lubricate internals of gearbox with PTFE dry lube from WD-40, or any spray lube for plastic.


# JGA25-370 motor housing, mounting, scotch yoke update
Using a more powerful motor, this should be able to run 36x cherry hg black 80g easy, and require a lot less motor replacement (TT motors)
Updated: Main housing, actuation plate housing lock, motor mounting plate, scotch yoke, bearing
Retained: Switch carriage, actuation plate, off center actuation plate, flat profile keycaps

Parts list to purchase:

1. JGA25-370 - https://item.taobao.com/item.htm?id=691467377622
I'm using 12v 282rpm myself, with voltage control, 200rpm to 300rpm, translate to 400-600 actuations per minute, 576k to 864k actuations per 24 hour.
12v 169rpm and 282rpm should work fine, I'm not sure about 6v, you should test this yourself if you want to run it with direct usb power.

2. Small bearing with screw embedded - https://item.taobao.com/item.htm?id=672727759613
JS6837-3C1L6M3
I've found that the previous bearing choice has a bit too much wobble/free-play, and if fastened tight, the bearing won't spin, if not fastened tight, screw may dislodge over time. This new one allows tightening and a lot less free-play, less maintenance.

Special durable material choice:
Nylon: actuation plate, scotch yoke, they last very long compared to PLA and ABS. Haven't tried PETG yet, YMMV.
High temperature resistant material: motor mounting plate. It might get hot, just in case.
Everything else can be printed in cheap PLA, and last quite some time.

![alt text][snapshot8]

[snapshot8]: /Images/20230223_011432.jpg "My setup/config, with fan, voltage control, double 8 digit counter." 

![alt text][snapshot9]

[snapshot9]: /Images/20230228_090258.jpg "Cheap SW-92SA lube." 

![alt text][snapshot10]

[snapshot10]: /Images/20230228_090425.jpg "JGA25-370." 

![alt text][snapshot11]

[snapshot11]: /Images/20230228_090528.jpg "New scotch yoke and bearings." 

![alt text][snapshot12]

[snapshot12]: /Images/20230228_100809.jpg "Lube between actuation plate and scotch yoke." 

![alt text][snapshot13]

[snapshot13]: /Images/20230228_100818.jpg "Scotch yoke should sit flush with motor shaft." 


Good luck and have fun building.

You can reach me through discord
issey83's corner - https://discord.gg/jTNPmTvsRC
