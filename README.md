# PETSCIIRobots
The start of a port of PETSCIIRobots, by David Murray, to the 68k Macintosh. This work is based on the SDL port by Vesa Halttunen <vesuri@jormas.com>. 

# About
- petrobots.cpp is the main game logic ported line by line from the 6502 files PETROBOTS.ASM and BACKGROUND_TASKS.ASM
- Platform.h is essentially an interface with platform specific implementation classes
- Various #defines starting with PLATFORM_ can be used to build a variant with different features using the same platform implementation
- To port to a new platform, create a new PlatformXYZ.cpp/h implementation based on the existing ones and instantiate it in main() (petrobots.cpp)

# Building
This work doesn't currently build, but work on it is being carried out using Symantec Think C++.  SDL will be replaced with Ingemar Ragnemalm's [Sprite Animateion toolkit](http://www.lysator.liu.se/~ingemar/sat.html) 

# License
This work inherits the license of the work on which it is based. 

This work is licensed under the Creative Commons Attribution 4.0 International License. To view a copy of this license, visit http://creativecommons.org/licenses/by/4.0/ or send a letter to Creative Commons, PO Box 1866, Mountain View, CA 94042, USA.

#TODO
Create a PlatformSAT.cpp/h file using Sprite Animation Toolkit.
