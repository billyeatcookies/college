---
tags:
  - BEC
---

- What is a PN jn?
The P-N jn is created by the method of doping. The **p-side** has excess **holes** and it will be a **trivalent** doped (BAlGaInTl) sc, is also the **positive** side of diode. 

- Formation of PN jn?
By the process of doping. Adds pentavalent impurity to p-type silicon sheet. this will make part of the sheet n-type. due to difference in **concentration** of holes and electrons, holes diffuse to n-side. then diffusion current is produced. when electron diffuses to p side, **immobile ionised donor** is left behind, this eventually forms a layer of positive charge in the n side. similarly ionised acceptors left behind due to holes diffusing to n-side creates a negative charge layer in p-side. both these layers combined is termed depletion region. Due to positive charge region, an **electric field** from positive charge towards negative charge is forme. Due to this electric field, electron on p side moves to n side which causes **drift current.**

- What is forward bias?
positive terminal of diode is connected to positive terminal of the battery.
built in electric fields and the applied electric fields are in opposite directions. when both electric fields add up the magnitude of resultant electric field is lesser than built in. since the free electrons in n side move towards p side and recombine with the immobile ionised acceptors and holes the other way, thinner depletion region, less resistive. the depletion region's resistance becomes negligible when applied voltage is larger than 0.6 in silicon and 0.2 in Germanium.
(case: guards trying to keep doors closed while students trying to enter classroom)

|E|V|Id(mA)|
|--|--|--|
|0.1|0.3|0|
|0.2|0.3|0|
|0.3|0.3|0|
|0.4|0.3|0.1|
|0.5|0.3|0.2|
|0.6|0.3|0.3|

- so then reverse bias?
the complete opposite. the direction of electric fields will be same and the resistance of depletion region will be larger and it will become thicker. more applied voltage means more resistance and thicker depl region.
(case: the more you ask the less you get)

|E|V|Id(mA)|
|--|--|--|
|1|1|0|
|2|2|0|
|3|3|0|
|...|...|...|
|50|50|0.1|
|51|50|0.2|
|52|50|0.3|

![[Pasted image 20230912203100.png]]


## Diode Capacitance

- capacitance for diodes? how?
the n side and p side acts like electrodes of capacitor as they have low resistance. the depl region is the high resistance dielectric like thing then! 

Two types of capacitance for the diode tho
1. transition capacitance
2. diffusion capacitance

- what is transition capacitance?
it's the extra! the amount of capacitance changed with increase in applied voltage. So for that the depl region should be thicker => **reverse bias case**!

**C<sub>T</sub> = dQ/dV = Aε/W** 
A - area of depl
**ε** - permittivity of depl
W - width of depl

- what is diffusion capacitance?
in the forward bias case! it's the storage capacitance. the free electrons in n side will move to p side and recombine with immobile ionised acceptors. also the other way for holes. the depl region will become thinner. the majority carriers (electrons) become minority carries of p region and holes the other way. so this transport of charge carries causes diffusion capacitance


$$C_D = \frac {\tau I_d}{\eta V_f}$$

τ - mean life of charge carriers
I<sub>d</sub> - diode current
η - 1 (indirect sc), 2 (direct sc)
V<sub>f</sub> - barrier potential
## Diode Resistance

r = V/I

## Load Line
- what is a.c/d.c load line?
provides linear operation of the diode.

- what is the q point?
the operating point or quiescent point represents the direct current and direct voltage through the diode. it gives information about the safe operating voltage and current of the diode.


## Temperature dependancy of diode

- How temperature affects a diode in forward bias?
as T rises, **barrier Voltage decrease** (2mV/ºC)

- and reverse bias?
as T rises, reverse current I<sub>r</sub> will increase (about 7-10% / ºC) (about double / 10ºC)

- the diode current eqn?
I<sub>d</sub> = I<sub>0</sub> (e<sup>qV/ηKT</sup> - 1)


## Half wave Rectifier

- How does a half wave work?
consists of only one diode. for the positive half cycle the diode acts like a closed circuit and for the negative half cycle acts like an open circuit.

![[Pasted image 20230914203617.png]]

resulting in a waveform only consisting positive half cycles of the a.c signal
![[Pasted image 20230914203845.png]]

- What is ripple and ripple factor?
amount of ac fluctuations remaining. 

$$\text{Ripple factor, } \gamma = \sqrt{ (\frac{ V _ { r m s } }{ V _ { d c } }) ^ { 2 } – 1 } = \sqrt{ (\frac{ I _ { r m s } }{ I _ { d c } }) ^ { 2 } – 1 }$$

$$V_{rms} = \frac {V_m} 2, V_{dc} = \frac {V_m} \pi$$

**ripple factor ≈ 1.21**

## Full wave center-tapped rectifier

two diodes and step down center tapped transformer. in positive half cycle, D1 is forward and D2 is reverse biased. D2 will be open circuit. in negative, D2 is forward, D1 will be open.

![[Pasted image 20230914212354.png]]

## Full wave bridge rectifier

four diodes. 

![[Pasted image 20230914220608.png]]

in positive half cycle, D1 becomes forward biased and D2 becomes open. then after load resistance signal passes through lower potential D3. then on negative half cycle, D4 becomes forward biased, D3 becomes open. then after load resistance signal passes through D2 which is at lower potential atm.

$$\text{Ripple factor, } \gamma =\sqrt{(\frac{{V_{rms}}^2}{V_{DC}})-1}$$

$$V_{rms} = \frac {V_m} {\sqrt{2}}, V_{dc} = \frac {2V_m} \pi$$

## Filter circuit

combination of capacitors to eliminate ripples. as the charging time of capacitors <<< discharging time, before the discharge completes, next cycle begins.

![[Pasted image 20230914222506.png]]

## Zener Diode

- what's the difference bw a normal PN jn diode and a zener diode?
a zener is a special type of PN jn diode that is heavily doped. it can conduct in both reverse and forward  directions. to conduct in reverse direction the voltage shall be higher than the zener breakdown voltage.

![[Pasted image 20230920221001.png]]

- why depletion region width of zener diode is smaller than a normal PN jn?
because it is heavily doped, so concentration of charge carriers is high, and hence a small width of depletion region will give a barrier voltage required. 

- what's avalanche breakdown?
occurs in both kinda diodes. at high voltages. valence electrons pushed into conduction due to energy imparted by accelerated electrons, which gain velocity due to collision with other atoms.

- temperature and avalanche breakdown voltage dependency?
temperature increases -> avalanche breakdown voltage increases

- what's zener breakdown?
5-7 v, valence electrons are pulled into conduction due to high electric field across the narrow depletion region.

- temperature and zener breakdown voltage dependency?
temperature increases -> zener breakdown voltage decreases
## Applications of Zener Diode

### Voltage Regulation

- line voltage regulation
- load voltage regulation

Makes use of the zener breakdown in reverse bias.

![[Pasted image 20230921000741.png]]






















