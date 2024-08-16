NB: took prelim notes in #a/liquid-text 
parent::[[215-LAoE]]

This lab focuses on MOSFET applications, as a power switch, as a logic switch, as an analog switch. Applicatios are [[Example - Power Switch BJT vs MOSFET]] (goes over temperature calcs),  [[Switched Capacitor Filter]], [[Example - Sample and Hold]] (which explores drawbacks of the CMOS)

Also touches on "Flying Capacitors" used to generate voltage above the supply input. 


## 12L.1 Power Mosfet 
- ➡️ [[MOSFET Power Switch]]

- [!] Careful of the specs - for $V_{GS(th)}$ and power dissipation

![](../attachments/694722ddd99c97b42cb2d4f710663de6.png)

### Temperature Considerations

![](../attachments/5212a7619660983a5ae14af928801eea.png)
![](../attachments/68d68aca35d7a8c5f909a0a8c7bf2b2f.png)
![](../attachments/55ec64cfa11fe5bf966faf7999b80490.png)
![](../attachments/e2f9aaa0c6186f48a48fc32b171ed1d4.png)

### 12L.1.4 Power Dissipation vs BJT

🔴 Subsume notes into [[MOSFET vs BJT]]

![](../attachments/056ebf2c83bdc114abe36e5591903ce4.png)

From $V_{DS}$ or $V_{CE}$ we can calculate the $R_{ON}$ for the FET/BJT. 

## 12L.2 Analog Switch Applications

🔴 ➡️ [[Analog Switch]]

### Sample and Hold 

🔴 ➡️ [[Example - Sample and Hold]]

![](../attachments/35acabbd1c9db17a807f652e03204274.png)

### Flying Capacitor

Can generate a higher voltage than input.

Such circuits often are put onto an integrated circuit that would otherswise require either a negative  supply or a second positive supply, higher than the main supply. 

![](../attachments/d78cf84c80fd11a7f4f605e9776c41c4.png)

### Chopper

This circuit automatically switches given a clock input - allows for displaying two signals on one scope channel. 

![](../attachments/a03b27fed7cb702ceaa2690362befca1.png)

