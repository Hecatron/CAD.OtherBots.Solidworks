# MakerSmith.Cad

## Overview

This is just a working directory for my translation of the original MakerSmith DXF Files into Solidworks Documents.
Note that I am not associated with the MakerSmith Association, this is just my attempt to build one of these devices from scratch using parts I have to hand.
Also I can't guarantee that the dimensions of the parts here match up with the original.
For the 1.0 and 1.1 directories I've attempted to match up the original dimensions as much as possible,
but there may be some degree of misalignment, use at your own risk.

The full assembly will be contained within Assembly-Root, this is the one to look for to load the whole diagram

  * [Notes on the different File Versions](docs/FileVersions.md)
  * [Notes on Different Material Thickness] (docs/MaterialThickness.md)

## Version 2.0

Version 2.0 is my own modified version of the design using 12mm thickness material and linear bearings. <br />
Note this is currently incomplete / still being worked on

## 2.0

### Changes Made

  * Dimensions and nuts all in metric / mm, typically M8 threaded rod
  * Sides thickned for additional height for experimentation with 3D Printing
  * Added Linear Bearings / Radial Bearings
  * Using Acrylic parts to cover the linear rods / to hold the bearings in place
  * Using mdf with a thickness of 12.4mm Metric (Europe) instead of Quater Inch
  * Using Stepper Motors instead of servo's for the rotation
  * Added Anti-Backlash nuts on each of the Axis

Note I haven't looked at the correct sizing for the servo mounts or gears.
I'm not sure if servo's would have enough power for the additional weight
but it should be possible to make some brackets to fit them using the new design (assuming they have enough power)

