# matt-poe-prototype
This is a KiCad design containing a schematic & PCB layout for a prototype PoE (Power over Ethernet) PD (Powered Device).

It provides for output isolation between the PoE delivery and the output power rails.  It provides for both 12V and 5V output rails, with a common ground for those two rails.

This is a prototype.  I'm happy to accept issues with questions or suggestions for improvement, and would very happily review any pull requests that come in.

This design utilizes the 3Peak TPE15017 and/or Monolithic Power Systems MP8017 -- they're interchangeable in this design.  This tiny IC handles the PoE power detection and classification and provides an active-clamp flyback controller with integrated low-side & clamp MOSFETs.  This part, in conjunction with an appropriate transformer provides a 12V output rail, which is further routed in this design to an inexpensive buck converter to provide for a 5V output rail.

In my testing up to this point, this design easily provides at least 10W of usable power out the 5V rail.  I've had it pulling 5V/2A on my DC test load continuously for several days.

![3D view](visuals/pcb-3d-f.png)

![Schematic](visuals/schematic.png)

[Bill of Materials](matt-poe-prototype.csv)

![Top view](visuals/matt-poe-prototype-topview.png)

[More visuals](visuals/)
