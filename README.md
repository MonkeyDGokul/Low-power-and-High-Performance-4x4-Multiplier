Abstract


In this work, a low-power, high-performance 4x4 multiplier is designed and implemented. This multiplier is essential for several arithmetic operations in digital signal processing (DSP) and other computational activities. 
The goal of the multiplier design is to maximize precision and high-speed performance at the same power consumption. In this paper Multiplier is introduced using MGDI technique. These digital circuits were then compared to conventional CMOS transistors in terms of area, number of transistors, and power dissipation.
The Cadence Virtuoso tool with 45 nm technology with channel length 100nm was used for the design and simulations, and a 1 V power supply voltage was used.
Compared to CMOS logic, a multiplier constructed in MGDI logic requires less transistors. Because of this, MGDI multiplier uses a lot less energy than CMOS design.

Introduction

Currently, due to the exponential increase in IC chip design difficulties. Such power-saving methods that may offer low power consumption, less complicated design, high speed performance, and high reliability without sacrificing any circuit design functionality are desperately needed to be developed and investigated. 
The most widely used technology for circuit design nowadays is CMOS technology, yet it leaks current when not in switching mode and wastes a lot of power when transistors are switching.
       During multiplication every switching event produces energy/power transfer from the supply voltage to an output terminal or from the output nodes to the terrain terminal in traditional CMOS logic circuits.
 Following this, further methods were introduced, such as Gate Diffusion Input (GDI), Complementary PTL, and Pass Transistor Logic (PTL).
     PTL has a higher speed than static CMOS logic because of its low node capacitances, fewer transistors, which result in reduced power dissipation, and simpler design. Logic degradation in the lengthy chain of pass transistors was PTL's primary drawback.
    When GDI was first presented, it was seen as a promising method for high performance, low power consumption, low design complexity, and little chip space. A basic GDI cell has just two transistors, but those two transistors can perform a wide range of intricate logic operations. The GDI technique's drawback is that it cannot provide the full output swing of a desired output state. In this paper, we have studied the Modified GDI technique for developing and simulating numerous logic functions, and we compare its transistor utilization and overall power dissipation with that of the current CMOS logic.

Methodology

1. 	4x4 Multiplier
   
An essential part of digital circuitry, a 4x4 multiplier calculates the product of two 4-bit binary values. Its importance stems from its capacity to carry out multiplication operations quickly and effectively, which are essential for many mathematical and digital signal processing (DSP) applications. In its most basic form, a 4x4 multiplier creates partial products from each of the individual input operand bits using combinational logic, then adds them together to get the result

   <img width="683" height="313" alt="image" src="https://github.com/user-attachments/assets/04ec8af1-f304-457e-ab1d-814f54f9ecef" />

  
   4x4 Multiplier equation

2.	MGDI (Modified Gate Diffusion Input) Technique

   MGDI is a brand-new method for creating digital circuits with little power consumption. This method is based on the GDI method. Digital circuits can have their power dissipation, transistor count, and area reduced by using the MGDI approach.
With the exception of the bulks of PMOS (SP) and NMOS (SN), which are continuously linked to VDD and GND, respectively, MGDI also has three input terminals: G, which is an input of both PMOS and NMOS; P, which is an input to drain or source of PMOS; and N, which is an input to source or drain of NMOS. The shortcomings of the GDI cell are overcome by MGDI. The impact of source body voltage on transistor threshold voltage becomes more reduced as technology advances.


  <img width="278" height="313" alt="image" src="https://github.com/user-attachments/assets/ba2173d0-27f5-47a0-94e2-24d705409016" />

  Fig1. MGDI Circuit                               

  <img width="324" height="260" alt="image" src="https://github.com/user-attachments/assets/14219bc8-9d91-4884-85f0-8e327ba9b581" />

  Fig2. MGDI Symbol 

  Different functions, as indicated in the accompanying table, are obtained by altering the values of G, P, N, SP, and SN in the MGDI cell. SP and SN will stay continuously connected to VDD and GND.

  <img width="723" height="286" alt="image" src="https://github.com/user-attachments/assets/226b5931-08bc-4b17-9cdf-fca597cec1cd" />

  Table 1:Logic Functions from a Modified GDI Cell

   Table 1 shows that a single MGDI cell can be used to create logic in a variety of ways. Two transistors are all that are needed to construct an OR or AND gate; with normal CMOS, six transistors are needed. The primary benefit of the MGDI approach is that it results in lower power consumption by reducing the number of transistors and chip size. Therefore, utilizing the MGDI technique to construct complex circuits is simple.

  3.	4x4 Multiplier is Designed with the following components given below: (Static CMOS vs MGDI)

  3.1	Inverter

  Static CMOS consists of a complementary pair of metal-oxide-semiconductor field-effect transistors (MOSFETs), one p-channel (PMOS) and one n-channel (NMOS), connected in series between the power supply voltage (VDD) and ground (GND). The gate of each transistor serves as the input, while the output is taken from the junction of the transistors, forming the inverter's output node. 
  In MGDI, P terminal is connected to VDD, N terminal is connected to GND and G terminal acts as Input.

<img width="304" height="314" alt="image" src="https://github.com/user-attachments/assets/9305f2a1-187a-4c5d-9a5b-1b4fa2a8579c" />

Fig 2. Static CMOS Inverter

<img width="446" height="257" alt="image" src="https://github.com/user-attachments/assets/1da4f3bc-62cc-4ff8-8033-7c9b306ad2e3" />

Fig 3. MGDI Inverter

3.2 AND 

CMOS AND gate, where a number of NMOS transistors are linked in series between the ground (GND) terminal and the output node. A number of PMOS transistors are linked in parallel between the power supply voltage (VDD) terminal and the output node at the same time. The inputs are connected to the gates of PMOS transistors and NMOS transistors. And Complemented Outputs are connected to inverter. Here 6 transistors are used.
In MGDI, P terminal is connected to GND, whereas Gate terminal and N terminal are treated as Inputs. In this circuit only 2 Transistor are used.

<img width="609" height="452" alt="image" src="https://github.com/user-attachments/assets/20cd9ae4-96db-411f-a710-d8fc42b9612b" />


<img width="304" height="314" alt="image" src="https://github.com/user-attachments/assets/246bfe5e-3773-4fa9-917b-02cce3ed51dc" />

Fig 2. Static CMOS Inverter

<img width="446" height="257" alt="image" src="https://github.com/user-attachments/assets/721b90f5-9c44-4c2f-b808-fa970158aae8" />

Fig 3. MGDI Inverter

3.2 AND 

CMOS AND gate, where a number of NMOS transistors are linked in series between the ground (GND) terminal and the output node. A number of PMOS transistors are linked in parallel between the power supply voltage (VDD) terminal and the output node at the same time. The inputs are connected to the gates of PMOS transistors and NMOS transistors. And Complemented Outputs are connected to inverter. Here 6 transistors are used.
In MGDI, P terminal is connected to GND, whereas Gate terminal and N terminal are treated as Inputs. In this circuit only 2 Transistor are used.


<img width="609" height="452" alt="image" src="https://github.com/user-attachments/assets/9f8f81fb-b1b9-4e49-8126-8337d1dda591" />

Fig 4: Static CMOS AND

<img width="694" height="295" alt="image" src="https://github.com/user-attachments/assets/87753e59-6441-446f-bfb5-52afb13b6cc0" />

Fig 5. MGDI AND

3.3 OR

CMOS OR gate, a number of parallel NMOS transistors are connected between the ground (GND) terminal and the output node. A number of PMOS transistors are linked in series between the power supply voltage (VDD) terminal and the output node at the same time. The inputs are connected to the gates of PMOS transistors and NMOS transistors. And Complemented Outputs are connected to inverter. Here 6 transistors are used.
In MGDI, N terminal is connected to VDD, whereas Gate terminal and P terminal are treated as Inputs. In this circuit only 2 Transistor are used.

<img width="612" height="401" alt="image" src="https://github.com/user-attachments/assets/8471d47d-7b40-48ac-bcbc-e53f1adf8fed" />

Fig 6: Static CMOS OR

<img width="624" height="262" alt="image" src="https://github.com/user-attachments/assets/291004da-566f-406e-a4d1-a6840ffed5bc" />

Fig 7: MGDI OR

3.4 XOR

Several PMOS transistors are linked in series between the output node and the power supply voltage (VDD), and several NMOS transistors are connected in parallel between the output node and ground (GND) in a simple CMOS XOR gate. The complemented inputs (inputs inverted) are connected to the gates of PMOS transistors, and the inputs are connected to the gates of NMOS transistors. Here 12 Transistors are used.
In MGDI, Gate, N (inverted input of P), P terminal are treated as Inputs. Only 4 transistors are used.

<img width="523" height="408" alt="image" src="https://github.com/user-attachments/assets/e92d008f-a600-4c48-b403-295602d66122" />

Fig 7: Static CMOS XOR

<img width="598" height="325" alt="image" src="https://github.com/user-attachments/assets/ea7dc915-955f-4cf6-94c0-9499ffff7f2f" />

Fig 8: MGDI XOR

3.5 Half ADDER

In binary arithmetic, a half adder is a basic digital circuit that is used to add two single-bit integers. It has two outputs, usually labeled as the sum (S) and carry (C), and two inputs, usually labeled as A and B, denoting the two bits to be added.
A half adder is usually implemented using an AND gate for the carry and an XOR gate for the sum. As an alternative, NAND or NOR gates can be used to implement it.


<img width="684" height="193" alt="image" src="https://github.com/user-attachments/assets/7347cad4-7d60-44c6-8437-aa1f6d3b2dce" />

Fig 9: Circuit

<img width="665" height="310" alt="image" src="https://github.com/user-attachments/assets/d731ae2c-a726-4c5f-a096-05237c89ce20" />

Fig 10: Symbol

3.6 Full Adder

A full adder is a digital circuit used in binary arithmetic to add three single-bit numbers: two inputs (A and B) and a carry input (Cin). It produces two outputs: the sum (S) and a carry-out (Cout).
A full adder can be constructed from two half adders and an OR gate. Alternatively, it can be implemented using various combinations of logic gates, such as XOR, AND, and OR gates.

<img width="791" height="302" alt="image" src="https://github.com/user-attachments/assets/5df7780d-4359-4a51-b455-7cfa9d3e80a2" />

Fig 11: Circuit

<img width="604" height="331" alt="image" src="https://github.com/user-attachments/assets/2f005a1b-ec1f-4c0a-95e4-bacc3699918d" />


Fig 12: Symbol

3.7 Number of transistors

Below table shows total number of transistors used in both Static CMOS and MGDI.

<img width="860" height="246" alt="Screenshot 2025-10-15 222140" src="https://github.com/user-attachments/assets/903fb69d-5e2a-4d15-81b7-e62a040413e5" />


From above data, it shown that MGDI uses less numbers of Transistors compared to the Static CMOS. Hence the area has significantly reduced.

4. Proposed Model


<img width="993" height="587" alt="image" src="https://github.com/user-attachments/assets/471c028b-ea2f-4757-8581-9ca9c13b77d2" />


5. 4x4 Multiplier testbench

   <img width="822" height="487" alt="image" src="https://github.com/user-attachments/assets/06e27d19-5dc7-4f88-a7ed-5dc49f4cb126" />

   For Standard CMOS design:
       Technology: gpdk45
       Channel Length = 45nm
       VDC   = 1.2v
        Vpulse= 1.2v
         Vpulse Time:

<img width="791" height="291" alt="image" src="https://github.com/user-attachments/assets/371b1925-0144-4f5a-b5de-cd95cca59fec" />

For MGDI design:
       Technology: gpdk45
       Channel Length = 100nm
       VDC   = 1v
        Vpulse= 1v
         Vpulse Time:

<img width="794" height="288" alt="image" src="https://github.com/user-attachments/assets/0c491396-87bb-4fb9-b3f3-4569ad3cdfb0" />


6. Results

6.1 Transient Waveform of 4x4 Multiplier (Standard CMOS)

<img width="1300" height="697" alt="image" src="https://github.com/user-attachments/assets/480cce33-7d89-4782-89be-62303ea7f4ad" />

6.2 Transient Waveform of 4x4 Multiplier (MGDI)

<img width="1292" height="693" alt="image" src="https://github.com/user-attachments/assets/acc1f455-2550-495d-bb76-47fd3aaf4c34" />

6.3 Power Dissipation Waveform of 4x4 Multiplier (Static CMOS).3 Power Dissipation Waveform of 4x4 Multiplier (Static CMOS)  

<img width="1310" height="636" alt="image" src="https://github.com/user-attachments/assets/92345729-c843-4cbf-8706-85f0c04f861d" />

6.4 Power Dissipation Waveform of 4x4 Multiplier (MGDI)

<img width="1292" height="664" alt="image" src="https://github.com/user-attachments/assets/02a00ec6-4c38-4345-b425-0c91c036ab68" />

6.5 Power Dissipation Value

The Power Dissipation in Calculated by taking Average Value of Power dissipation waveform in calculator tool in virtuoso&.

<img width="370" height="295" alt="image" src="https://github.com/user-attachments/assets/30e2ceef-eb22-41b9-bd45-8110b48a5a06" />

Standard CMOS based 4x4 Multiplier

<img width="406" height="295" alt="image" src="https://github.com/user-attachments/assets/14f683f4-0872-4ba7-90e9-295346e3e7c5" />

MGDI based 4x4 Multiplier

Power reduced by = (6.129 x 10^-6 / 12.32 x 10^-6) x 100 = 49.74%

Conclusion

•	The following circuits are designed using static CMOS and MGDI and performed comparative analysis.
•	We have observed the  power dissipation primarily stems from dynamic power consumption, driven by switching activities during multiplication operations.
•	It’s observed that power dissipation has reduced almost 50% by using MGDI compared to Static CMOS.
•	Number Of Transistors has been reduced significantly in MGDI compared to Static CMOS.
•	However there is certain limitation of using MGDI, occurred was it was not able to produce a strong ‘0’ or ‘1’.


                       
































 




