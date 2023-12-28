# Exp-6-Synchornous-counters - up counter and down counter 
### AIM: To implement 4 bit up and down counters and validate  functionality.
### HARDWARE REQUIRED:  – PC, Cyclone II , USB flasher
### SOFTWARE REQUIRED:   Quartus prime
### THEORY 

## UP COUNTER 
The counter is a digital sequential circuit and here it is a 4 bit counter, which simply means it can count from 0 to 15 and vice versa based upon the direction of counting (up/down). 

The counter (“count“) value will be evaluated at every positive (rising) edge of the clock (“clk“) cycle.
The Counter will be set to Zero when “reset” input is at logic high.
The counter will be loaded with “data” input when the “load” signal is at logic high. Otherwise, it will count up or down.
The counter will count up when the “up_down” signal is logic high, otherwise count down

Since we know that binary count sequences follow a pattern of octave (factor of 2) frequency division, and that J-K flip-flop multivibrators set up for the “toggle” mode are capable of performing this type of frequency division, we can envision a circuit made up of several J-K flip-flops, cascaded to produce four bits of output.
The main problem facing us is to determine how to connect these flip-flops together so that they toggle at the right times to produce the proper binary sequence.
Examine the following binary count sequence, paying attention to patterns preceding the “toggling” of a bit between 0 and 1:
Binary count sequence, paying attention to patterns preceding the “toggling” of a bit between 0 and 1.

Note that each bit in this four-bit sequence toggles when the bit before it (the bit having a lesser significance, or place-weight), toggles in a particular direction: from 1 to 0.



 
 

Starting with four J-K flip-flops connected in such a way to always be in the “toggle” mode, we need to determine how to connect the clock inputs in such a way so that each succeeding bit toggles when the bit before it transitions from 1 to 0.

The Q outputs of each flip-flop will serve as the respective binary bits of the final, four-bit count:

 
 

Four-bit “Up” Counter
![image](https://user-images.githubusercontent.com/36288975/169644758-b2f4339d-9532-40c5-af40-8f4f8c942e2c.png)



## DOWN COUNTER 

As well as counting “up” from zero and increasing or incrementing to some preset value, it is sometimes necessary to count “down” from a predetermined value to zero allowing us to produce an output that activates when the zero count or some other pre-set value is reached.

This type of counter is normally referred to as a Down Counter, (CTD). In a binary or BCD down counter, the count decreases by one for each external clock pulse from some preset value. Special dual purpose IC’s such as the TTL 74LS193 or CMOS CD4510 are 4-bit binary Up or Down counters which have an additional input pin to select either the up or down count mode.
![image](https://user-images.githubusercontent.com/36288975/169644844-1a14e123-7228-4ed8-81a9-eb937dff4ac8.png)


4-bit Count Down Counter

### PROCEDURE 
write te steps involved

### PROGRAM 
/*
Program for flipflops  and verify its truth table in quartus using Verilog programming.
Developed by: LAKSHMI PRIYA V
RegisterNumber:  212223220049
*/




UP COUNTER :

![Screenshot 2023-12-28 215019](https://github.com/Lakshmi-v-Priya/Exp-7-Synchornous-counters-/assets/151720706/1ab465ae-15f2-4804-88c9-52f12ef460b2)


DOWN COUNTER :

![Screenshot 2023-12-28 215207](https://github.com/Lakshmi-v-Priya/Exp-7-Synchornous-counters-/assets/151720706/d7e24e48-9041-4471-84d3-57ae14275ee8)








### RTL DIAGRAM

UP COUNTER :

![up diagram](https://github.com/Lakshmi-v-Priya/Exp-7-Synchornous-counters-/assets/151720706/c4815825-3ccf-4026-a20f-e4ee7111f30d)


DOWN COUNTER :

![Screenshot 2023-12-28 215721](https://github.com/Lakshmi-v-Priya/Exp-7-Synchornous-counters-/assets/151720706/0b7a7d32-39bb-42bf-9d54-fd6e948a4d4f)






### TIMING DIGRAMS FOR COUNTER  


UP COUNTER :

![up wave](https://github.com/Lakshmi-v-Priya/Exp-7-Synchornous-counters-/assets/151720706/d803f10f-5913-4c42-968b-90955103e4e1)

DOWN COUNTER :

![down wave](https://github.com/Lakshmi-v-Priya/Exp-7-Synchornous-counters-/assets/151720706/5fcb1b61-00c9-49bf-b906-21d6d4d6002b)




### TRUTH TABLE 

UP COUNTER :

![Screenshot 2023-12-28 220234](https://github.com/Lakshmi-v-Priya/Exp-7-Synchornous-counters-/assets/151720706/c588b66e-527e-41a9-aa94-82f07ecb8b7a)


DOWN COUNTER :

![Screenshot 2023-12-28 220331](https://github.com/Lakshmi-v-Priya/Exp-7-Synchornous-counters-/assets/151720706/1de44c38-53c5-4ba7-b362-9b5e2beb29ae)


### RESULTS 

Thus the Program executed Successfully
