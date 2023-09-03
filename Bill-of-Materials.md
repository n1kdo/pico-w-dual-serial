# Bill of Materials for Pico-W Dual Serial

| Item | Qty | Reference(s)               | Description                            | MANUFACTURER           | Part Number                  |
|------|-----|----------------------------|----------------------------------------|------------------------|------------------------------|
| 1    | 7   | C1, C2, C3, C4, C5, C6, C7 | .1 uF 35V tantalum capacitor           | Kemet                  | T350A104M035AT               | 
| 2    | 1   | D1                         | 1N5819 1A Schottky Diode               | STMicroelectronics     | 1N5819                       |
| 3    | 1   | D2                         | White LED                              | LiteOn                 | LTW-420D7                    |
| 4    | 1   | F1                         | Resettable fuse 0.9A                   | Littelfuse             | RUEF090                      |
| 5    | 2   | J1, J2                     | DB9_Male                               | Amphenol               | L717SDE09PA4CH4RC309         |
| 6    | 1   | J3                         | DC Coaxial Power Connector 2 mm pin    | Switchcraft            | RAPC722X                     |
| 7    | 1   | R1                         | 330 Ohm 1/4 watt through hole resistor | YAGEO                  | CFR-25JT-52-330R             |
| 8    | 1   | SW1                        | Pushbutton switch                      | NKK Switches           | GB215AHB                     |
| 9    | 1   | n/a                        | Switch cap                             | NKK Switches           | AT4063                       |
| 10   | 1   | U1                         | Raspberry Pi Pico W                    | Raspberry Pi Ltd       | SCO918                       |
| 11   | 1   | U2                         | MAX3232 *or* ADM3202ANZ                | Analog Devices / Maxim | MAX3232ECPE+ *or* ADM3202ANZ |
| 12   | 1   | U3                         | 5 volt linear voltage regulator        | STMicroelectronics     | L7805CV                      |
| 13   | 1   | n/a                        | 16-pin DIP socket                      | Mill-Max               | 110-47-316-41-001000         |
| 13   | 1   | n/a                        | Flanged plastic enclosure              | Hammond Manufacturing  | 1591XXSFLBK                  | 
| 14   | 1   | n/a                        | Printed Circuit Board                  | your choice            | n/a                          |

## Notes

The MAX3232 is crazy expensive, I have found that the ADM3203ANZ works just as well in this circuit.  If you feel that
you need the additional ESD protection, by all means, use the more expensive part.  

The specified IC socket is a 'machined-pin' style socket.  Cheaper alternatives exist.

There is no need to use a white LED, you can use whatever color you like.  I just think the white ones look cool.

Almost all of these parts were ordered from Mouser.  I was surprised to see they are stocking the Raspberry PI Pico W.
They were pretty scarce at first.  Also Digikey.

The circuit board is up to you.  I have bought these from both [Oshpark](https://www.oshpark.com) and 
[DKRed](https://www.digikey.com/en/resources/dkred) -- neither is inexpensive in small prototype runs.  I think the 
last order for Oshpark was about $60 for three boards, and DKRed was a little cheaper.  Both seem to be of good 
quality.  DKRed can accept Kicad files directly, even though it asked for Gerbers.  

I built the prototype on perf-board, there is no requirement for the printed circuit board, it is just
easier and less error-prone than point-to-point wiring.

The board is designed to fit into the specified Hammond enclosure.  You will need to cut out holes for the DE9 
connectors, the power socket, and the LED and push button.