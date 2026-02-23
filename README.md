## Experiment No: 5
### ASTABLE MULTIVIBRATOR USING 555 TIMER Using Proteus
## Aim
To design and simulate an Astable Multivibrator using NE555 in Proteus Design Suite and observe the continuous square wave output.
## Apparatus Required
<img width="463" height="214" alt="image" src="https://github.com/user-attachments/assets/4b5d6ff8-0c90-4238-9fa4-a4a7b3d21084" />

## Circuit Diagram
<img width="1920" height="1200" alt="Screenshot 2026-02-03 141605" src="https://github.com/user-attachments/assets/c023b1e7-80b3-472b-92b4-183c8da9551d" /><br/>

Pin Configuration of 555 Timer:<br>
•	Pin 1 → Ground<br>
•	Pin 2 → Trigger<br>
•	Pin 3 → Output<br>
•	Pin 4 → Reset (Connected to Vcc)<br>
•	Pin 5 → Control Voltage (Bypass with 0.01 µF capacitor optional)<br>
•	Pin 6 → Threshold<br>
•	Pin 7 → Discharge<br>
•	Pin 8 → Vcc<br>
## Connections:
•	R1 → Between Vcc and Pin 7<br>
•	R2 → Between Pin 7 and Pins 2 & 6<br>
•	C → Between Pins 2 & 6 and Ground<br>
•	Output → Pin 3<br>
## Theory
•	The NE555 timer is a widely used integrated circuit for generating precise time delays and oscillations. When operated in astable mode, it functions as a free-running oscillator that continuously produces a square wave without any external triggering signal.<br>
• In this mode, a capacitor connected to the circuit charges through resistors R1 and R2 and discharges through R2 repeatedly. The internal voltage divider of the 555 timer creates two reference levels at 1/3 Vcc and 2/3 Vcc. <br>
•	When the capacitor voltage reaches 2/3 Vcc, the upper comparator resets the flip-flop and turns ON the discharge transistor, causing the capacitor to discharge. When the voltage falls to 1/3 Vcc, the lower comparator sets the flip-flop, turning OFF the discharge transistor and allowing the capacitor to charge again. <br>
• This continuous charging and discharging process generates a square wave at the output (Pin 3) and an exponential waveform across the capacitor. The time period of oscillation is given by T=0.693(R1+2R2)CT = 0.693 (R1 + 2R2) CT=0.693(R1+2R2)C, and the frequency depends on the values of R1, R2, and C. <br>
• Thus, the 555 timer in astable mode acts as a simple and reliable square wave generator used in clock circuits, LED flashers, and pulse generation applications.<br>
## Procedure
1.	Open Proteus software.<br>
2.	Select NE555 IC, resistors, capacitor, and CRO.<br>
3.	Connect circuit in astable configuration.<br>
4.	Apply 5V supply.<br>
5.	Run simulation.<br>
6.	Observe square wave output at Pin 3.<br>
7.	Measure time period and frequency.<br>
## Tabulation
<img width="675" height="60" alt="image" src="https://github.com/user-attachments/assets/27bdc28d-57a3-4899-a4c5-a659288bc7ed" />

## Waveforms
<img width="1380" height="881" alt="Screenshot 2026-02-03 141732" src="https://github.com/user-attachments/assets/c0cee5a8-27f4-4217-8bf1-275480f36a0c" /><br/>

•	Output (Pin 3) → Square wave<br>
•	Capacitor voltage → Exponential charging & discharging waveform<br>
## Result
The Astable Multivibrator using NE555 Timer IC was successfully designed and simulated in Proteus.<br>
A continuous square wave output was obtained.<br>
The practical frequency closely matches the theoretical frequency.<br>
## Conclusion
•	The 555 timer works as a free-running oscillator in astable mode.<br>
•	Frequency depends on R1, R2, and C values.<br>
•	Increasing R or C decreases frequency.<br>
•	Used in clock generation, LED flashing, and tone generation.<br>
## Viva Questions
**1.	What are the operating modes of 555 timer?**

The 555 timer operates in three modes: monostable, astable, and bistable mode. These modes are used for one-shot pulse, continuous oscillation, and flip-flop operation.<br>

**2.	What are the threshold levels in astable mode?**

In astable mode, the capacitor voltage varies between 1/3 Vcc and 2/3 Vcc. These levels control the charging and discharging of the capacitor.<br>

**3.	Write the frequency formula.**

The frequency of astable multivibrator is given by f = 1.44 / ((R1 + 2R2)C). It depends on resistor and capacitor values.<br>

**4.	What is duty cycle?**

Duty cycle is the percentage of time the output remains HIGH in one cycle. It indicates the ratio of ON time to total time.<br>

**5.	What happens if R2 increases?**

If R2 increases, the charging and discharging time increases. So the frequency decreases and time period increases.<br>
