### SYNCHRONOUS-UP-COUNTER

**AIM:**

To implement 4 bit synchronous up counter and validate functionality.

**SOFTWARE REQUIRED:**

Quartus prime

**THEORY**

**4 bit synchronous UP Counter**

If we enable each J-K flip-flop to toggle based on whether or not all preceding flip-flop outputs (Q) are “high,” we can obtain the same counting sequence as the asynchronous circuit without the ripple effect, since each flip-flop in this circuit will be clocked at exactly the same time:

![image](https://github.com/naavaneetha/SYNCHRONOUS-UP-COUNTER/assets/154305477/d5db3fa0-e413-404c-b80e-b2f39d82e7e8)


![image](https://github.com/naavaneetha/SYNCHRONOUS-UP-COUNTER/assets/154305477/52cb61eb-d04b-442d-810c-31185a68410b)

Each flip-flop in this circuit will be clocked at exactly the same time.
The result is a four-bit synchronous “up” counter. Each of the higher-order flip-flops are made ready to toggle (both J and K inputs “high”) if the Q outputs of all previous flip-flops are “high.”
Otherwise, the J and K inputs for that flip-flop will both be “low,” placing it into the “latch” mode where it will maintain its present output state at the next clock pulse.
Since the first (LSB) flip-flop needs to toggle at every clock pulse, its J and K inputs are connected to Vcc or Vdd, where they will be “high” all the time.
The next flip-flop need only “recognize” that the first flip-flop’s Q output is high to be made ready to toggle, so no AND gate is needed.
However, the remaining flip-flops should be made ready to toggle only when all lower-order output bits are “high,” thus the need for AND gates.

**PROGRAM**
![WhatsApp Image 2024-12-22 at 11 28 36_5613fb11](https://github.com/user-attachments/assets/73c61f8c-d20a-419a-bc45-24396f160b27)


Developed by: A Chandhna  RegisterNumber: 24900265
*/

**RTL LOGIC UP COUNTER**
![WhatsApp Image 2024-12-22 at 11 28 35_c984ed4a](https://github.com/user-attachments/assets/cb050984-5ffa-4566-8e73-b053c7c633f4)


**TIMING DIAGRAM FOR IP COUNTER**
![WhatsApp Image 2024-12-22 at 11 28 35_f2db108a](https://github.com/user-attachments/assets/900db2c3-06c9-4e6d-92ba-ff3d2049d241)

**TRUTH TABLE**
![WhatsApp Image 2024-12-20 at 12 54 36_d7e712cd](https://github.com/user-attachments/assets/72cbd09d-5a1c-4a96-a1ff-c9d52b3dffc6)

**RESULTS**
