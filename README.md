# 4 Elements Fullsize Yagi Antenna for 20m Band (7.5 m boomlength)
Here is presented a model of 4 elements fullsize yagi antenna for 20m band.
The model is optimized for the **boomlength of 7.5 meters** while keep maintain good **VSWR < 1:1.2 throughout 20m band**, gain, and F/B ratio. These can be achieved by using 3 elements basic model and then adding a director which is closely coupled to the driven element. This added director actually become the first director. With this arrangement, the first director will resonates at the upper portion of the band while the driven element itself resonates at the lower portion of the band. Therefore, actually this is 3 element yagi with extra "driven element". The model is simulated for the installation height of 24 meters using 4nec-2 software package.

![](./NEC2-Models/4E-20-YAGI_7M5_3DStructure.png)

## Dimensions
The picture below will tell thousands words. Please left click / right click + open in new tab for the full view of the picture.
![](./DrawIO/Dimension.png)

## 4NEC-2 Models Download
Right Click -> Save As, Then change the file type as **.NEC**
Open with 4NEC-2 software.
* [4 Element 20m Yagi without tower](https://raw.githubusercontent.com/handiko/4E-20M-YAGI/master/NEC2-Models/4E-20-YAGI_7M5.NEC)
* [4 Element 20m Yagi with tower](https://raw.githubusercontent.com/handiko/4E-20M-YAGI/master/NEC2-Models/4E-20-YAGI_7M5_towerTop.NEC)

![](./NEC2-Models/4E-20-YAGI_7M5_3DStructure2.png)

### About The Telescopic Element sizing
Each of the element is constructed and simulated as a telescopic alumunium tubing. Telescopic taper sizing is considered as **1 inch dia. alu. tubing at the center and 3/8 inch dia. alu. tubing at the tip** Taper schedule from the center to the tip can be adjusted to the alu. tubing dia. which can be purchased locally.
**The models are correct only for the taper sizing mentioned above. If you, for example, want to swap the taper sizing with another size, the model still can be constructed and be adjusted to your working freq but will not deliver the performances predicted in my model.**

### Tuning procedure:
* Mount the antenna at the real installation height.
* **USE A GOOD 1:1 BALUN or CHOKE BALUN** at the feed point.
* Do the tuning procedure using Antenna Analyzer or SWR Analyzer using 50 Ohm Coax as short & practical as possible. Here, you want to eliminates tuning error caused by the long coax. Therefore, use a short coax.
* Tune the driven element for the lowest VSWR at 14.05 MHz and tune the first director for the lowest VSWR at 14.25 MHz. Adjust both end simultaneously.

### Typical VSWR:
(derived from simulation)

|**Parameter**           |**VSWR**   |**Comments**                         |
|:----------------------:|:---------:|:-----------------------------------:|
|**14.0 MHz**            | 1:1.1     |                                     |
|**14.1 MHz**            | 1:1.03    |                                     |
|**14.2 MHz**            | 1:1.07    |                                     |
|**14.3 MHz**            | 1:1.12    |                                     |
|**14.35 MHz**           | 1:1.14    |                                     |
|**VSWR Bandwidth 1:1.5**| n/a       | practically flat throughout 20m band|

### Typical Gain and F/B
* **Forward Gain**: 13.9 dBi nominal
* **F/B**: 22 dB nominal
* **3 dB beamwidth**: 66 degrees nominal
* **RDF**: 14 dB nominal

## Simulation Results
![](./NEC2-Models/4E-20-YAGI_7M5_towerTop.NEC.png)
![](./NEC2-Models/4E-20-YAGI_7M5_2DPattern.png)

## Propagation Map Simulation (VOACAP Online, April 2020 at 12 UTC, 160 W of transmit power)
![](./NEC2-Models/4E-20-YAGI_7M5_Coverage_VOACAP.png)

## Contributing
1. Fork it [https://github.com/handiko/4E-20M-YAGI/fork](https://github.com/handiko/4E-20M-YAGI/fork)
2. Create new branch (`git checkout -b myfeature`)
3. Do some editing / create new feature
4. Commit your works (`git commit -m "Adding some myfeature blah blah.."`)
5. Push to the branch (`git push -u origin myfeature`)
6. Create a new Pull Request
