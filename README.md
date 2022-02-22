# CMOS-3-bit-Wallace-Tree-Multiplier

This repository contains the design, test and chracterization of a CMOS 3-bitm Wallace Tree Multiplier designed in Synopsys Custom Compiler using a 28nm PDK. <br/>
This project was done as a part of Analog Hackathon conductued by IITH, Synopsys and VSD.

# Table of Contents
 * [Introduction](#Introduction)
 * [Circuit Details](#Circuit-Details)
 * [Differential End Current Starved VCO](#Differential-End-Current-Starved-VCO)
 * [Tools Used](#Tools-Used)
 * [Pre-Layout Schematics and Simulations](#Pre-Layout-Schematics-and-Simulations)
 * [Netlist of the Circuit](#Netlist-of-the-Circuit)
 * [Results](#Results)
 * [Author](#Author)
 * [Acknowledgements](#Acknowledgements)
 * [References](#References)

# Introduction

A Wallace multiplier is a hardware
implementation of a binary multiplier, commonly used in
digital computers. It is a digital circuit that multiplies
two integers. It uses multiple AND gates, half and full
adders to sum partial products in stages until two
numbers are left.This is also called the Wallace tree or
Wallace reduction. Wallace multipliers were devised by
the Australian computer scientist Chris Wallace in 1964

# Circuit Details

The Wallace tree has three steps: </br>
• Multiply each bit of one of the arguments, by each
bit of the other.  </br>
• Reduce the number of partial products to two by
layers of full and half adders.  </br>
• Group the wires in two numbers, and add them with
a conventional adder.  </br>
</br>First we need to multiply each bit of first factor(A)
by each digit of the other factor(B). Each of this partial
products will have weight equal to the product of its
factors. The final product is calculated by the weighted
sum of all these partial products. Next the resulting bits
are reduced to two numbers, this is done by using a
full adder to sum three components and half adder to
sum two components. Finally the two resulting numbers
are given as input to an adder and the final product is
obtained. </br>


# Author:
• Subham Mohapatra, B.Tech(EEE), National Institute of Technology Karnataka, Surathkal. <a href='https://www.linkedin.com/in/subham-nitk/'>LinkedIn</a></br>


# Acknowledgements:
• <a href='https://www.iith.ac.in/events/2022/02/15/Cloud-Based-Analog-IC-Design-Hackathon/'>Cloud Based Analog IC Design Hackathon</a></br>
• <a href='https://www.synopsys.com/'>Synopsys India</a></br>
• <a href='https://www.vlsisystemdesign.com/'>VLSI System Design (VSD) Corp. Pvt. Ltd India</a></br>


# References:
[1] Implementation of a CMOS Wallace-tree Multiplier, Xiaoping
Li, Xingguo Xiong, Hassan Bajwa, Prabir Patra Department of
Electrical and Computer Engineering, University of Bridgeport,
Bridgeport, CT 06604 </br>
[2] N. Sureka, R. Porselvi and K. Kumuthapriya, ”An efficient high
speed Wallace tree multiplier,” 2013 International Conference on
Information Communication and Embedded Systems (ICICES),
2013, pp. 1023-1026, doi: 10.1109/ICICES.2013.6508192
