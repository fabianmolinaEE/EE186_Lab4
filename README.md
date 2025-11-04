# EE186_Lab4
This is a private repository for EE186 Lab 4

## Part 2: ADC

### What are the different bit resolutions can you set the ADC? What is the maximum sampling rate at each of these resolutions? Where did you find this information in the datasheet?

The ADC uses 6, 8, 10, and 12 bit resolutions. For each, the max sampling rates are: 

12 bit- 5.33 Msps
10 bit- 6.15 Msps
8 bit- 7.27 Msps
6 bit- 8.88 Msps

This information can be found in section 6.3.21 of the datasheet in table 81 - ADC Characteristics. 

### Why do you need a voltage divider circuit? What would happen if the photodiode is directly connected to the board?

The voltage divider is needed because the photodiode produces a current proportional to light intensity and not a voltage. Because of this, we need a resistor in the voltage divider to allow us to measure the voltage and measure the voltage within the range of the ADC since it has a maximum voltage it can read. This allows us to make a proportional voltage and not have a voltage that is readable and not floating or outside of our measurable levels for voltage. 

### Circuit Diagrams
![Circuit Diagrams](part-2-ADC/circuits.png)

### Video Demo of photoresistor
Source Code: [photoresistor_read.c](part-2-ADC/photoresistor_read.c)

<video controls src="part-2-ADC/IMG_1424.mov" title="Title"></video>

## Part 3: DAC 
