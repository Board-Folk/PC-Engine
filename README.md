# NEC PC Engine PCB Reproductions

This repository contains a recreation of the main board PCB for NEC's PC
Engine console. The recreation is based on the available schematics for the
TurboGrafx-16 and reverse engineering using scanned images of an original
board's copper layers, so should be a reasonably accurate reproduction.


## PCB Production

Minimum track widths, clearances and via sizes are within the standard
offering of modern PCB fabricators. Development was done using JLCPCB and
the boards therefore have their order number placeholder on the silkscreen,
which you may wish to remove if using another service.

The design is verified to work as a 2-layer PCB.


## Bill of Materials

Most parts are marked on the board and it is expected that these will be reused
from a donor board. It is completely possible that your particular board uses
different (but compatible) parts so it's advisable to take photos before starting.
Below is therefore a partial bill of materials for parts whose values are not
marked on the boards and/or look otherwise alike. For a complete BOM, consult the
generated [Interactive BOM][IBOM] or the KiCad project itself.

Some parts may not be present on revisions other than the particular `PWD-623A`
board this reproduction is based upon. There is at least one revision that is
missing some of the higher numbered (`R16x`) resistors. These do not appear to be
essential but this has not yet been verified.

Capacitor voltages may exceed those given, within reason. E.g. you may
substitute 16V for a 10V part. You may well find that the original 1uF parts
are 50V, for example. Do not, however, use a lower voltage than specified.
No voltage is specified for the ceramic capacitors; any 0805 or 1206 part is
expected to exceed the required voltage anyway. Note that while all the
footprints are the same, a mix of 0805 and 1206 capacitors were used in some
cases. The footprints below are therefore those of the actual part, not the
pads on the PCB. Again, your particular donor board may vary. If in doubt, or for
less fiddly soldering, you could use 1206 parts throughout.

The "Possible Markings" column is a (likely incomplete) list of labels we've come
across on original boards. Yours may be similar or wildly different.

| Reference | Value | Footprint | Possible Markings |
|:---------:|:-----:|:---------:|:-----------------:|
|C101 | 22uF 16V | THT 5mm | |
|C102 | 47uF 25V | THT 5mm | |
|C103 | 47uF 16V | THT 5mm | |
|C105 | 10uF 16V | THT 5mm | |
|C108 | 1uF 10V | THT 5mm | |
|C109 | 1uF 10V | THT 5mm | |
|C110 | 1uF 10V | THT 5mm | |
|C111 | 1uF 10V | THT 5mm | |
|C112 | 1uF 10V | THT 5mm | |
|C113 | 1uF 10V | THT 5mm | |
|C114 | 1uF 10V | THT 5mm | |
|C115 | 1uF 10V | THT 5mm | |
|C116 | 10uF 16V | THT 5mm | |
|C117 | 47uF 16V | THT 5mm | |
|C118 | 0.1uF | 0805 | |
|C119 | 0.1uF | 1206 | |
|C120 | 0.1uF | 0805 | |
|C121 | 0.1uF | 1206 | |
|C122 | 0.1uF | 1206 | |
|C123 | 0.1uF | 0805 | |
|C124 | 0.1uF | 0805 | |
|C125 | 0.1uF | 0805 | |
|C126 | 0.1uF | 0805 | |
|C127 | 0.1uF | 0805 | |
|C129 | 0.1uF | 0805 | |
|C130 | 0.1uF | 0805 | |
|C131 | 0.1uF | 0805 | |
|C132 | 0.1uF | 0805 | |
|C133 | 0.1uF | 0805 | |
|C134 | 0.1uF | 0805 | |
|C135 | 0.1uF | 0805 | |
|C136 | 0.1uF | 0805 | |
|C137 | 220pF | 1206 | |
|C138 | 220pF | 1206 | |
|C145 | 33pF | 1206 | |
|C146 | 0.1uF | 0805 | |
|C147 | 0.1uF | 0805 | |
|C148 | 0.1uF | 0805 | |
|C149 | 10uF 10V | THT 5mm | |
|C150 | 0.1uF | 1206 | |
|C151 | 15000pF | 1206 | |
|C152 | 220pF | 1206 | |
|C153 | N/P | 1206 | |
|D101 | IS954 | SOT-23 | 4, A4 |
|R101 | 4.7K | 1206 | |
|R102 | 4.7K | 1206 | |
|R103 | 4.7K | 1206 | |
|R104 | 33K | 1206 | |
|R105 | 4.7K | 1206 | |
|R106 | 4.7K | 1206 | |
|R107 | 4.7K | 1206 | |
|R108 | 4.7K | 1206 | |
|R109 | 4.7K | 1206 | |
|R110 | 4.7K | 1206 | |
|R111 | 4.7K | 1206 | |
|R112 | 4.7K | 1206 | |
|R113 | 4.7K | 1206 | |
|R114 | 4.7K | 1206 | |
|R115 | 56K | 1206 | |
|R116 | 56K | 1206 | |
|R117 | 56K | 1206 | |
|R118 | 56K | 1206 | |
|R119 | 4.7K | 1206 | |
|R125 | 9.1K | 1206 | |
|R126 | 15K | 1206 | |
|R128 | 9.1K | 1206 | |
|R134 | 4.7K | 1206 | |
|R137 | 6.2K | 1206 | |
|R138 | 8.1K | 1206 | |
|R141 | 27K | 1206 | |
|R142 | 3.3K | 1206 | |
|R143 | 1.5K | 1206 | |
|R144 | 1.5K | 1206 | |
|R145 | 20 | 1206 | |
|R146 | 100 | 1206 | |
|R149 | 2.7K | 1206 | |
|R152 | 4.7K | 1206 | |
|R155 | 5.6K | 1206 | |
|R156 | 1K | 1206 | |
|R157 | 13K | 1206 | |
|R158 | 9.1K | 1206 | |
|R159 | 5.1K | 1206 | |
|R160 | 1K | 1206 | |
|R161 | 680 | 1206 | |
|R162 | 10K | 1206 | |
|R163 | 1.2K | 1206 | |
|R164 | 1.2K | 1206 | |
|R165 | 100 | 1206 | |
|TR103 | 25C945 | SOT23 | LC |
|TR104 | 25A733 | SOT23 | M5 |
|TR105 | 25C945 | SOT23 | LC |


## Thanks

  * Rob Taylor ([@PeepoUK](https://github.com/PeepoUK)) for the initial
    groundwork, layout and footprints on which this project is based.

  * Simon "Aergan" Lock ([@Aergan](https://github.com/Aergan)),
    Chrissy ([@chris-jh](https://github.com/chris-jh)) and
    Dennis (@PointerFunction) for their insights, support and
    testing of the prototype boards.

  * The rest of the Board Folk for their support and general
    coolness.


## Legal

As the product of this project is a replica of a proprietary product, the
the author makes no claim of copyright to the schematics nor PCB layouts and
releases these into the public domain, solely for the purposes of study and
historical preservation.

You are free to produce PCBs based on this project's designs at your own risk
and without limitation, for your own use or for sale and/or repair at a
reasonable price. Attribution is appreciated. The authors are not obliged to
provide support of any kind.

Under no circumstances will the authors be held responsible or liable in any
way for losses, damages or costs resulting from the use of the information
and/or resources of this project.

The resources are provided "as-is" without warranty of any kind, either
expressed or implied, including, but not limited to, the implied warranties
of merchantability and fitness for a particular purpose.

[IBOM]: http://htmlpreview.github.io/?https://raw.githubusercontent.com/Board-Folk/pc-engine/main/bom/ibom.html
