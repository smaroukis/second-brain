parent::[[Advanced Rectifier Circuits]], [[03-Diode-Circuits]]

![](../attachments/e537d38bf76520790a7c9aabd5e15dde.png)

Summary::Ripple in power supply design results from the charging and discharging of the output capacitor during the AC mains input cycle, impacting the smoothness of the output voltage. The calculation of ripple involves estimating the current using the formula $I = C \frac{dV}{dt} \Rightarrow dV = \frac{I \Delta t}{C}$, considering worst-case scenarios with maximum supply current and a dt=8ms discharge time. The implications for transformer sizing include the need for a higher-rated transformer due to current spikes during the charging portion, with a small ripple requiring more significant oversizing.

The output capacitor (normally pretty large, in the hundreds of microfarad range) acts to smooth the output voltage so it doesn't drop to 0V at the reversal point of the sinusoidal input. 

Under load the capacitor discharges after the rectifier output reaches its peak and starts its sinusoidal descent. The exact slope is an exponential decay curve. We can approximate the time period of the ripple ($\Delta t$) as just a half cycle of the 60Hz input, although in reality it is smaller (since the decay ends when the capacitor begins charging up again). 

The ripple can be estimated from $I=C\frac{dV}{dt}$ where dV is the ripple, $I$ is the load current, and dt is the discharge time. Usually we will define a maximum allowable ripple and then calculate the capacitor size with the other parameters given. Worst cases are:
- $I$ as the maximum of the supply
- $dt$ ($\Delta t$) as 8ms (since the ripple component will be at 120Hz, twice that of the supply frequency)
see [[Example - Full Bridge Rectifier]] for a worked example.

An important implication of ripple to power supply design is that the **spikes in current from the ripple call for a higher rated transformer** than under steady load current. The transformer has to "work harder" to replenish the capacitor during the charging portion of the cycle. If the charging portion is 3/8 of the 8ms cycle and the load current is $I_{LD}$ then **the capacitor will charge at $\frac{8}{3}\cdot I_{LD}$ to replace the current lost in the discharge portion of the cycle** (since $I_{LD}$ needs to average to itself over the cycle). 

Ripple effect on peak power sizing of a transformer #anki-todo 

The calculation for this current's RMS value (which gives the amount of heating and thus size of the transformer) is:
$$ I_{rms}=\sqrt{(\text{charging fraction})\times(\text{current})^2}$$
so for a 3/8 charging fraction
$$I_{rms}=\sqrt{(3/8)\times(8I_{LD}/3)^2}\approx 1.6 I_{LD}$$

A **small ripple is clearly worse** in the sense that we will need to oversize our transformer the smaller the ripple (we can use solid state voltage regulators to smooth out these power supply ripples to much smaller values without requiring huge transformers).

| Charging Portion  | $I_{LD}$ Factor| 
| --- |---|
| 3/8 |1.6 |
| 1/5 | 2.2|
| 1/20 | 4.4|
