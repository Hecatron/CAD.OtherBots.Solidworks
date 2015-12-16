# File Versions / Releases

## SolidWorks/2.0 LaserCut Logan1 BFG

This is the new version I'm working on at the moment, this should be the final design I'll use for my own model.
I've recently managed to get a sheet of 12.4mm cheap from Wicks for around £8.

I've codenamed this one Logan 1, after the device in Logans Run (I think it was called the escapulator)

Main differences from the original will be:

  * Different dimensions used for the parts, rounded up metric mm values
  * Use of cheap linear and rotational bearings along the axis
  * Additional tidy up to get everything aligned
  * Diagrams for LaserCutting, including inkscape files
  * Adjustable thickness of material via External File formulae

Note if your planning on using 12mm thick mdf, it might be difficult to get access to a laser cutter that can cut that deep.
But I'm hoping to make the thickness adjustable in the diagram via a text file

## SolidWorks/1.1 LaserCut Assembly

This is an initial version using the original Makersmith dimensions which were probably in inches

  * I've added dimensions in mm
  * Re-modelled some of the sketches to include relationships.
  * Tried to tidy up dimensions such as 1.99999mm to 2mm
  * Created assemblies to get an idea as to how everything fits together
  * Added a global variable for the thickness of the material
  * Added some Mate References for snapping parts together within the Assemblies

However

  * Some of the parts do not align correctly, this is probably due to the conversion of inches to mm when I imported from the original dxf files
  * Not all the screws or nuts or bushings have been included
  * For this version I haven't done the threaded rod, gears or servo, just a rough approximation of a threaded rod
  * If you plan on using this as a laser template please note further cleanup is needed on the dimensions as there is some mis-alignment between parts.

I'll be doing additional cleanups on Version 2.0 of the model but this one will be re-sized so won't be compatible with parts from the original frame.
The main difference will be the move from mm with decimal places to mm with round numbers, and perhaps additional clearance for a 3D printer head.

I can't guarantee the sizes of the parts match up with the original, since it's just an experiment to see how everything fits together.
It assumes a thickness of MDF of 5.35mm which is a bit of an odd size, and there will be tolerances of the cut / kerf of the laser.
There is a global variable setup on each part for 5.35 wherever I've found that measurement, including the boss extrusion.
Don't expect to simply change this value and have everything fit together though that's something I'm aiming for later in 2.0.

## SolidWorks/1.0 LaserCut Original

This is an initial import of the dxf files into solidworks parts <br />
I've combined duplicates, set the axis to the origin and set the Extrusion depth to 5.35mm which seems to be the MDF thickness in use in the 3D models <br />
I've avoided adding dimensions on most parts, this should be considered a raw import of the dxf data

## OriginalDxf

These are the original DXF Files provided by MakerSmith

  * https://github.com/MakesmithAccessibleTech