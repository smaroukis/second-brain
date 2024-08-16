parent::[[04-Transistors-1]]

Summary:: For the emitter follower, negative inputs can clip the output due to the asymmetry of the circuit (driving with transistor, pulling with resistor). We can add a pull down (p-type) transistor to replace the resistor which turns ON for the negative swings ;→ this is the [[push pull emitter follower]]

See [[04-Transistors-1#Voltage Follower]]


![](../attachments/060e5ef63c8627f0aeae08266441d072.png)

![](../attachments/e3bdbba3df806b84cdd3f8337683ff19.png)
A true push pull will fix the crossover distortion by biasing the bases of the transistors apart so that there isn't a section of time that both V_BEs are < 0.6V.

![](../attachments/5fc1135e0aa924f1bce346de15366ef1.png)

