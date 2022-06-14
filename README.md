# Discrete AY-3-8910

This is a WIP project to make a complete and fully compatible AY-3-8910 out of discrete and readily avaiable 74-series logic ICs.

## Background

Whilst there are many software implementations both for PC and microcontrollers like an AVR as well as implemntations in Verilog to be used in a FPGA I haven't seen any real hardware level implementations of it yet.

The chip is fairly well analyzed and documented and even had its die analysed and a schematic of it on the transistor-level has been made. More info about that can be found github.com/lvd2/ay-3-8910_reverse_engineered

## Digital simulation

Being a fan of Helmut Hneemanns project _Digital_ which is a circuit simulator for digital designs (much like Logisim) I started by making a design of the AY-3-8910 in it ending up in just a bit over 104 ICs.

This sounds a lot and complicated, but my design is quite modular and most of the modules are quite simple and eyas to build. The most complex module is the envelope generator that can generate eight different envelopes that is used to vary the volume of the tones over time.  This part I have a copy as a separate module with testcases inorder to verify the correct function of each mode.

Below is a shrunk and blurry overview of the entire schematic - click here for a [highres version](https://raw.githubusercontent.com/mengstr/Discrete-AY-3-8910/main/Images/AY-3-8910-full-large.png) of it.

![reduced overall schematic](Images/AY-3-8910-full-small.png)
