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

![Screenshot 2024-12-28 211237](https://github.com/user-attachments/assets/28c6d703-de8f-4d8c-81c1-1279a4eac652)


Developed by:SATHANA.V

RegisterNumber:24901144


**RTL LOGIC UP COUNTER**


![Screenshot 2024-12-28 211247](https://github.com/user-attachments/assets/c99c6080-a68d-4770-9d64-36bb52970f03)


**TIMING DIAGRAM FOR IP COUNTER**

![WhatsApp Image 2025-01-06 at 10 33 28_b19ff70e](https://github.com/user-attachments/assets/b891a21a-4e86-4f25-af10-e6e5290892f4)





**TRUTH TABLE**


![WhatsApp Image 2025-01-03 at 14 03 42_e8b0abfe](https://github.com/user-attachments/assets/47ddfec9-4e1b-439c-8052-bd8f8ee2583c)




**RESULTS**

SYNCHRONOUS UP COUNTER has studied and verified successfully using quartua software.
