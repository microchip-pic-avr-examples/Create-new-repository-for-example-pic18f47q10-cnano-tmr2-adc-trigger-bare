<a href="https://www.microchip.com" rel="nofollow"><img src="images/MicrochipLogo.png" alt="MCHP" width="300"/></a>

# PIC18F47Q10 Using TMR2 as Auto-conversion trigger for ADCC module

The PIC18F47Q10 features Three 8-bit Timers/Counters and a 10-bit ADC with computation (ADCC) module.
In this demo, uses TMR2 peripheral to trigger the ADCC to make conversions at a fixed frequency rate, that can be adjusted with the period of TMR2.

## Related Documentation
- Technical Brief Link [(linkTBD)](http://www.microchip.com/)
- [PIC18F47Q10 Product Family Page](https://www.microchip.com/design-centers/8-bit/pic-mcus/device-selection/PIC18F47Q10)
- [PIC18F47Q10 datasheet](http://ww1.microchip.com/downloads/en/DeviceDoc/40002043D.pdf) for more information or specifications.

## Software Used

- MPLAB® X IDE 5.30 or newer [(microchip.com/mplab/mplab-x-ide)](http://www.microchip.com/mplab/mplab-x-ide)
- MPLAB® XC8 2.10 or newer compiler [(microchip.com/mplab/compilers)](http://www.microchip.com/mplab/compilers)

## Hardware Used
- PIC18F47Q10 Curiosity Nano [(DM182029)](https://www.microchip.com/Developmenttools/ProductDetails/DM182029)
- Curiosity Nano Base for Click Boards™ [(AC164162)](https://www.microchip.com/Developmenttools/ProductDetails/AC164162)
- POT click board™ [(MIKROE-3402)](https://www.mikroe.com/pot-click)

## Setup

- The PIC18F47Q10 Curiosity Nano Development Board [(DM182029)](https://www.microchip.com/Developmenttools/ProductDetails/DM182029) is used as the test platform.
- Insert it into the Curiosity Nano Base for Click Boards™ [(AC164162)](https://www.microchip.com/Developmenttools/ProductDetails/AC164162) along with the POT click board™ [(MIKROE-3402)](https://www.mikroe.com/pot-click).
    <br><img src="images/HWsetup.jpg" alt="HardwareSetup" width="480"/>

The following pin configurations must be made for this project:

|Pin           | Configuration         |
| :----------: | :-------------------: |
|RA0           | Analog input for ADCC |
|RE0           | Digital output (LED0) |

## Operation
1. Build demo firmware, make and program the generated code onto the PIC18F47Q10 Curiosity Nano.
2. Plug the POT click board™ into the mikroBUS™ slot (1) of the Curiosity Nano Base board.
3. Run the code, LED0 will blink with `Timer2Period` frequency.
4. LED0 will blink if Potentiometer value is below `DesiredThreshold`, and if above `DesiredThreshold`, LED0 will be ON. 
    <br><img src="images/HWsetup-TMR2-trigger.gif" alt="Hardware Setup"/>


## Summary

This project showcases how easy it is to use the TMR2 of PIC18F47Q10 as a Auto-conversion trigger for ADCC module.
