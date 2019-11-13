# solo-business-card
A flex PCB business card that also works as a Solo

# BOM

|  Ref | value  | type  | package  | quantity  | Required? |
|---|---|---|---|---|--|
| C1-C9,C11  | 4.7u  | capacitor  | 0402  | 10  | yes |
| C10,C12  | \* xx, yy  | C0G capacitor  | 0402  | 10  | yes |
|  ST1 | STM32L432KU  |  Microcontroller | QFN32  | 1  |yes |
| N1  | AS3956-ATDM-S4  | NFC IC (SPI version)  | MLPD 3x3  | 1  |  yes |
|  R1 | 500R  | resistor  | 0402  | 1  |  no |
|  L1 | CL-505S-X-SD-T  | RGB LED  | 0606  | 1  |  no |

\* C10 and C12 are tunning capacitors connected in parallel.  I have not yet measured what the nominal value for them should be, but will be somewhere around 45pF.

# Assembly instructions

Assemble BOM on badge. 

# Programming

Connect programmer to debug port.  Connector uses the following cable.

http://www.tag-connect.com/TC2030-CTX-NL

Connect cable to an ARM debugger/programmer.  And program one of the "bundle" builds from the latest Solo release.

https://github.com/solokeys/solo/releases
