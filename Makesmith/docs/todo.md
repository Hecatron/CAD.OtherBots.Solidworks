# TODO

## After initial cut test:

  * On assembly A on the cross beam where the nut sits, try partially drilling out the nut hole, and putting a bunch of washers in to pad the nut
  * Also on assembly A use the longer self tapping screws next to where the nut sits

## TODO Later:

  * Look into housing for opto end stops / acrylic addon to Assemby A and clearances
  * ServoMount Dimensions
  * Look at the holes for the wiring in the support beams underneath

  * Check we have M4 bolts long enough to go through the bracket and the mdf with a nut on the other end
  * we may need to adjust the thread length or use different size bolts for distance between the sensor and magnet
  * look at the distance required for the magnetic sensor, we may need longer bolts for 2 sets of nuts at the end
    available is 40mm, 50mm, 60mm, also extend the plate to cover them from nocking
  * Check cut dimensions are around 240mm / 240mm / 240mm, additional clearance on Z Axis for 3D Printing
  * Check the main baseplate on the X Axis is the correct size for the additional clearance / size 

## TODO Make

First we need to mark off the cut lines using the old Laser cutter
  * Put Masking Tape onto the work piece
  * use the laser on the lowest setting to mark off the lines

for lasering:

Run some tests with laser safe MDF / Ply, MDF should be the more stable one for rigidity
(Ply is stronger and less susceptable to moisture, but for rigitity you need the expensive stuff)
laser mdf is sometimes called medite
  * http://www.hindleys.com/index.php/materials/timber/mdf-1/medite-laser-mdf-sheet/medite-mdf-1220mm-x-610mm-x-12mm.html
  * http://hpclaser.co.uk/index.php?main_page=product_info&cPath=3&products_id=110 - Ply

For manually cutting:

  * I need a "Mortice Chisel Set 4Pc"
  http://www.screwfix.com/p/mortice-chisel-set-4pc/15113?kpid=15113&cm_mmc=Google-_-Product%20Listing%20Ads-_-Sales%20Tracking-_-sales%20tracking%20url&kpid=15113&cm_mmc=Google-_-Shopping%20-%20Power%20Tool%20Accessories-_-Shopping%20-%20Power%20Tool%20Accessories&gclid=CJX-l-TK5MUCFSEYwwod13sADg
  * And some sort of attachment for the drill
  * https://www.youtube.com/watch?v=hxyWfze3qzQ
  * https://www.machinemart.co.uk/shop/product/details/cma1b-mortising-attachment
  * http://www.clarketooling.co.uk/tools/Drill_Presses___Mortisers.html
  * drill diameter size is 66mm for the larger one, and I think 47mm for the smaller one


## TODO Design

  * Assembly B
    Reduce the part that holds the dremmel to the minimum width
    add bolt holes
    add an inner part, and anti backlash nut




  * Base Plate E:
  * Sidepanels / Y Axis plates next

  * Do the Y Axis Holes first for the rods, copy the hole spacing / sizes from the X Axis
  * Top features should be locked distance wise to the top of the part and centered

  * Do the Y Axis Support afterwards with tabs etc and adjustable height
  * Finaly do the outer support beams for the electronics etc



  * For 3D printing double the thickness of the side panels, and raise the Y Axis assembly
    look into having an interchangeable Dremmel / 3D printer Head







### 3D Printering

Threaded Rod has the advantage of being possibly more accurate and having more force than a belt, so is better suited for a CNC.
But belts are a lot faster and are better for 3D Printing.

For the belt
http://reprap.org/wiki/Step_rates
http://www.adafruit.com/products/1252 - 20 tooth / 8mm bore
With 200 steps and 1/8 stepping I should be able to manage 0.025mm

For the rotary encoder this is 14bit
one full revolution on the pulley should equal 40mm
this should allow for a resolution of around 2.4 microns



Idea, for the X and Y Axis why not have both!!

To switch from threaded rod to belts:

  * First we have a series of holes so that we can rotate the steppers on both the X and y axis
    When the stepper is directly facing the axis we can attach it to a threaded rod
    When the stepper is at a 90 degree angle we can attach a small piece of rod, with a pulley

  * When in threaded rod cnc mode, both the rod and pulley are in place, but the pulley isn't used
    the stepper is attached to the threaded rod and the pulley is just ignored
    the pulley should stay in place via a rotary bearing and a couple of nuts.

  * When in pulley 3d printer mode, the threaded rod is unscrewed from the X and Y Housing (we just detach the stepper coupler and undo a couple of nuts)
    We rotate the motor, then just attach the motor to the pulley rod

This way we can get the best of both worlds, with minimal effort in changeover.
The Z axis we can keep on threaded rod ether way


### FSR

As a future upgrade think about positioning Force Sensor resistors between the supports
to detect force between the work piece and the dremmel
