# Amiga-external-3x-FDD

![20251017_163530](https://github.com/user-attachments/assets/bb7866ed-46f4-41a4-8de2-53a95b0d27c0)

Allows you to connect an original 1.44MB 3.5" PC FDD without any modifications or  PC FDD modified for AMIGA. It also allows you to connect a GOTEK emulator (SFR1M44-U100 or SFR1M44-U100K).
(GOTEK, must be set to position S0)
You can connect 3 mechanics in any combination to FDD1, FDD2 and FDD3.
It all depends on the setup of the juper.

NOTICE:
Unconnected drives are displayed in the Workbench system as "DFx:????" it's not a bug, but a function of the adapter.


Settings:
For each drive port (FDD1,FDD2,FDD3)
there are two jumpers available to set the function of the adapter.

JP1 – JP4 for FDD1
JP2 – JP5 for FDD2
JP3 – JP6 for FDD3
The first jumper (JP1, JP2, JP3) is set by DISK CHANGE for the particular drive.
Jumper (JP1,JP2,JP3) positions 1-2 for Gotek or modified PC drive.
Jumper (JP1,JP2,JP3) positions 2-3 for unmodified PC drive.

Second jumper (JP4,JP5,JP6) 
sets the SELx signal (DS0 or DS1)
Jumper (JP4,JP5,JP6) positions 1-2 for Gotek or modified PC drive.
Jumper (JP4,JP5,JP6) positions 2-3 for unmodified PC drive.



Example:
Connect the Gotek to the FDD1 port and set JP1 and JP4 to position 1-2.
Connect the original PC FDD to the FDD2 port, then set JP2 and JP5 to position 2-3.
Connect the modified PC FDD to the FDD3 port and set JP3 and JP6 to position 1-2,

Both jumpers from a given pair (JP1-JP4,JP2-JP5,JP3-JP6) are always connected to the same position.
Unless we had a partially modified PC FDD where only the SEL signal was modified to DS0 and DISK CHANGE was not modified, then we would have to set: the first jumper position 2-3 and the second jumper position 1-2.

Important:
Jumper JP7 can be connected either with a piece of wire or with a 0 Ohm smd resistor, but do this only if you really need 12V for the drive. Standard FDDs use only 5V.
If you activate 12V, it can easily lead to the power connector being inserted backwards and subsequently destroying the drive or Gotek.


Components:
6x  3 pin 2.54mm (jumper) JP1 to JP6    
2x  IC  74LS38 DIP14  U1,U4 
2x  IC  74LS74 Dip14  U2,U3
6x  resistor 0,25W 2k2 Ohm  R1 to R6
2x  ceramic capacitor  100nf  104    C1,C2
3x  4 pin 2.54mm KF2510-A (Male header) power FDD   J1,J2,J3
1x  DB23 male (d-sub 23)  J4 



![20251018_103336](https://github.com/user-attachments/assets/930e9d4d-9dd0-410f-8968-f6ca6372ad63)



More information about the project and the PCB   https://www.pcbway.com/project/shareproject/Amiga_External_3x_FDD_16dd8842.html 
