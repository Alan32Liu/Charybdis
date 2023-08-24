# Charybdis


An ergonomic keyboard with integrated trackball.

Engineered to be a full mouse replacement solution with high-quality, custom-developed components.

There are 4x6 and 3x5 Nano versions.

Made to be used with the [Scylla](https://github.com/Bastardkb/Scylla) or [Skeletyl](https://github.com/Bastardkb/Skeletyl) on the other half.

![](pics/1ae.jpg)

![](pics/1af.jpg)


# Sourcing the components

## Electronic components

Depending on which version you print, you will need more or less of each component.

The 3d files are designed around a custom sensor PCB:

https://github.com/Bastardkb/charybdis-pmw-sensor

You will need to source all of the components from the sensor PCB's BOM.

Otherwise, you can also use other sensor PCBs, but you will need to modify the 3d adapter files.

Components necessary:

| Part name                         | Amount (4x6) | Amount (3x5) | Link                                                                                       |
| --------------------------------- | ------------ | ------------ | ------------------------------------------------------------------------------------------ |
| Elite-C                           | 2            | 2            | [Keebio](https://keeb.io/products/elite-c-low-profile-version-usb-c-pro-micro-replacement-atmega32u4) |
| Elite-C adapter for the Charybdis | 2            | 2            | https://github.com/Bastardkb/Elite-C-holder                                                |
| Cables                            |              |              | 28 AWG recommended                                                                         |
| Audio jack, SMD                   | 2            | 2            | [TRRS](https://keeb.io/collections/diy-parts/products/trrs-jack-3-5mm)                     |
| Button, 4x4x1.5                   | 2            | 2            | https://www.aliexpress.com/item/1005001304569553.html?spm=a2g0s.9042311.0.0.27424c4dDwgcp7 |
| Sensor PCB                        | 1            | 1            | see details below                                                                          |
| Bearing, MR63-3x6x2.5mm           | 3            | 3            | [Amazon](https://www.amazon.com/MR-2RS-Deep-Groove-Ball-Bearing/dp/B09BTTDTT1?th=1)        |
| Flexible PCB for the plate (4x6)  | 2            | 0            | https://github.com/Bastardkb/Scylla-PCB-Plate                                              |
| Flexible PCB for the thumbs       | 1            | 1            | https://github.com/Bastardkb/PCB_thumbs_Charybdis                                          |
| Flexible PCB for the thumbs (4x6) | 1            | 0            | https://github.com/Bastardkb/Scylla-PCB-thumb-cluster                                      |
| SOD123 Diodes                     | 8            | 35           | [Digik](https://www.digikey.com.au/en/products/filter/discrete-semiconductor-products/diodes/rectifiers/single-diodes/sod-123/280?s=N4IgjCBcpgbFoDGUBmBDANgZwKYBoQA3AOygBcAnAV3xAHsoBtEAFgAYWAOAJhZAF0CABzJQQAZUoBLYgHMQAXyVA)|
| BAT54C Diodes                     | 24           | 0            | [1](https://www.amazon.com/dp/B0BL6PCPT7?tag=opebrobar-20&linkCode=osi&th=1&psc=1), [2](https://www.amazon.com/dp/B06WRNN7ND?tag=opebrobar-20&linkCode=osi&th=1&psc=1)  |
| M4 8mm Torx Screw                 | 16           | 12           | Conrad, [Amazon](https://www.amazon.com/uxcell-M4x8mm-Screws-Replaces-Carbide/dp/B07KY8QJC6/ref=sr_1_1?content-id=amzn1.sym.918a99dd-4826-4c0a-be33-a6705d69c4cf%3Aamzn1.sym.918a99dd-4826-4c0a-be33-a6705d69c4cf&keywords=Screws&pd_rd_r=97a7b1be-f6be-4778-882f-903a0b0aecdf&pd_rd_w=8OYjX&pd_rd_wg=BttCv&pf_rd_p=918a99dd-4826-4c0a-be33-a6705d69c4cf&pf_rd_r=0KVABRZ0HQDXVJT4M17R&pid=86exCdD&qid=1692883413&refinements=p_n_feature_five_browse-bin%3A3177290011%2Cp_n_feature_twenty-eight_browse-bin%3A19043859011&s=industrial&sr=1-1) |
| M4 screw insert, M4 X D6.0 X L5.0 | 16           | 12           | [aliexpress](https://fr.aliexpress.com/item/4000232925592.html?spm=a2g0s.12269583.0.0.6aef4f282LZO4v)    |
| Screws, M3 8mm Torx               | 8            | 8            | [Amazon](https://www.amazon.com/dp/B01D8L4XVE?tag=opebrobar-20&linkCode=osi&)              |
| Heated screw insert, M3x5x5       | 5            | 5            | [aliexpress](https://fr.aliexpress.com/item/1005005220632314.html?spm=a2g0o.productlist.main.5.35de11b34IXUpa&algo_pvid=d15248ab-3830-4259-a2ca-363436415617&algo_exp_id=d15248ab-3830-4259-a2ca-363436415617-2&pdp_npi=4%40dis%21AUD%2110.85%210.77%21%21%2150.39%21%21%402101e9d416928837462348642e7119%2112000032238859319%21sea%21AU%210%21A&curPageLogUid=X44qKjVjlO5T)                                                                                           |


If you want RGB, you will also need:

| Part name          |  Amount (4x6) | Amount (3x5)  | Link       |
| ------------------ | ------ | ---------- | ---------- |
| SK6812 Mini-E LEDs | 58  | 35  | [Aliexpress](https://fr.aliexpress.com/item/1005005956813491.html?spm=a2g0o.productlist.main.1.fc852531dA2cKc&algo_pvid=2a4c8f79-da04-40a7-9c02-71613ab11d67&algo_exp_id=2a4c8f79-da04-40a7-9c02-71613ab11d67-0&pdp_npi=4%40dis%21AUD%2114.99%2114.99%21%21%219.56%21%21%402101e9d416928839526482288e7119%2112000035024278716%21sea%21AU%210%21A&curPageLogUid=mdTrydzk6Daf) |
| Capacitor, 1uF          | 4  |  4   | 1206, [aliexpress](https://fr.aliexpress.com/item/32973259342.html?spm=a2g0o.productlist.main.1.14111e3fQfuumk&algo_pvid=98833444-9676-4ea5-8f03-27e481e39e6b&algo_exp_id=98833444-9676-4ea5-8f03-27e481e39e6b-0&pdp_npi=4%40dis%21AUD%210.65%210.56%21%21%213.03%21%21%402101e9d416928839884072589e7119%2166651074262%21sea%21AU%210%21A&curPageLogUid=MfWtThVRr3Qq)                                  |
| Resistor, 330Ohms       | 4   |  4  | 1206, [Amazon](https://www.amazon.com/dp/B07QH5PFG3?tag=opebrobar-20&linkCode=osi&th=1)                                  |
| Wires                   |     |    | 28 AWG recommended, Black, Red, Color. [Amazon](https://www.amazon.com/BNTECHGO-Silicone-Flexible-Strands-Stranded/dp/B07HGT77R5/ref=sr_1_1_sspa?keywords=28+awg+wire&qid=1692884402&sprefix=28+AWG+%2Caps%2C315&sr=8-1-spons&sp_csd=d2lkZ2V0TmFtZT1zcF9hdGY&psc=1) |
| Ribbon cables Flexstrip | 6    | 6  | [Digik](https://www.digikey.com.au/en/products/detail/te-connectivity-amp-connectors/FSP-22A-12/5591822?utm_adgroup=&utm_source=google&utm_medium=cpc&utm_campaign=Pmax_Focus%20Supplier&utm_term=&utm_id=go_cmp-20193105734_adg-_ad-__dev-c_ext-_prd-5591822_sig-Cj0KCQjw_5unBhCMARIsACZyzS0ldfSiOn4i5GuByEKcSBIuPog4oslJEGRk3z689VjsMcxxYmswdqAaAqPIEALw_wcB&productid=5591822&gad=1&gclid=Cj0KCQjw_5unBhCMARIsACZyzS0ldfSiOn4i5GuByEKcSBIuPog4oslJEGRk3z689VjsMcxxYmswdqAaAqPIEALw_wcB)  |             


## Mods

There are some mods to add BTUs or ball bearings, check the *mods* folder.


![](pics/1ac.png)


## Print the case

The STL files are included in this Github.
Feel free to use and modify them at length. The files are on a non-commercial license, so this is for personal projects only - please do not use those to sell them.

Please find detailed instructions on how to print the case here:
https://docs.bastardkb.com/hc/en-us/articles/360020031180-Print-settings-for-Dactyls

You will need to print:

- ball adapter, top
- ball adapter, bottom

Please note the adapter of the 3x5 is not compatible with the 4x6, and vice-versa.

On top of that, for each part of the keyboard you decide to print (case, plate, tent) you will need to print the other side from the normal keyboard (eg. left Scylla/right Charybdis 4x6, left Skeletyl / right Charybdis Nano 3x5)

## Printing the tents and plates

If you are printing a Charybdis 4x6, just print the plates and optional tent.

If you are printing a Charybdis Nano 3x5, there are multiple options available - take a look at the `readme` in the `3x5` folder

## Get a kit from BastardKB

You can get a full Kit, including case and all PCBs and electronics required on the shop:
https://bastardkb.com/

If you want to print the case yourself, you can also get just the electronics Kit.

# Build guide

Find the build guide at https://docs.bastardkb.com/

# Finding help

- Discord: https://bastardkb.com/discord
- Website: https://bastardkb.com/
- Docs: https://docs.bastardkb.com

# Support me on Patreon

If you like the keyboard, please consider helping me with Patreon: https://www.patreon.com/bastardkb

I post regular updates and hindsight on my work. I work full time on keyboard innovation, and this helps a lot !

# License 

This work is licensed under a Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License.
