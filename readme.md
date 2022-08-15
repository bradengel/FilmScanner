# Film Scanner
This film scanner is based off of the very good work of Seckin Sinan Isik's LIDAR driven motorized film carrier here: https://www.duckafterduck.com/blog/how-to-make-a-lidar-driven-motorized-film-carrier

## Changes
- Moved CAD from FreeCAD to Fusion360
- Converted the main bodies (front and back) from surfaces to solid bodies (better for 3D printing)
- Removed the LIDAR mount (using modified software from https://github.com/bezineb5/RoboScan)
    - My fork here: https://github.com/bradengel/RoboScan?organization=bradengel&organization=bradengel
- Created 135 version
- Added Motor mount for 28BYJ-48 Stepper Motor
- Changed orientation to make extended film collectors the legs for horrizontal scanning
- Created a slot for plate glass to support film (WIP)
- Configured for bearings, rather than parts rubbing together

## Non-3D printed parts
- O-Rings
    - Nitrile Rubber O-Rings 16mm OD 11mm ID 2.5mm Width
    - https://www.amazon.com/dp/B07W61VVFV?psc=1&ref=ppx_yo2ov_dt_b_product_details
- Timing Belts
    - 110mm and 300mm GT2 6mm timing belt
    - https://www.amazon.com/dp/B07KK86NYX?psc=1&ref=ppx_yo2ov_dt_b_product_details
- Timing Belt Pulleys
    - 20 Tooth GT2x6mm 5mm bore
    - https://www.amazon.com/dp/B077GNZK3J?psc=1&ref=ppx_yo2ov_dt_b_product_details
- Stepper Motor and Driver
    - 28BYJ-48 Stepper Motor
    - ULN2003 Motor Driver
    - https://www.amazon.com/dp/B01CP18J4A?psc=1&ref=ppx_yo2ov_dt_b_product_details
- Ball Bearings
    - 625 Ball bearings 5mm x 16mm x 5mm
    - https://www.amazon.com/dp/B07TML6YP4?psc=1&ref=ppx_yo2ov_dt_b_product_details
- M4 bolts and nuts
    - 2x 10mm for stepper motor
    - 4x 15mm for spacers
- M4 Heat-set inserts
    - https://www.cnckitchen.com/shop#!/Gewindeeinsatz-threaded-insert-M4-Standard-50-Stk-pcs/p/431147582/category=0

## 3D Printed Parts
### Shared Components
- Drive Side Body (with stepper motor mount)
- Idle Side Body
- Film Collector (x2 for using as legs)

## non-shared components
- Drive and Idler axles
- Spacers

## A note about bearings, housings, shafts, and fits
Generally, you need to change the dimensions so that the fits on the bearings are what you want.  My dimensions may not work for you.  In a perfect world, I'd print the precision components on a resin printer (or even a metal 3d printer, then machine them to the proper tolerances), but I don't have one, nor do I want one.  So there.
### Bearing Housing Fit
My goals is to have the bearing housings (the holes that the bearings fit into on the drive and idle bodies) be interference fit (https://en.wikipedia.org/wiki/Interference_fit).  I've adjusted the dimensions so that _my_ 3D printer creates a housing that just barely fits the bearings.  I put the bearings in the freezer to shrink them, press them in their housing, and as they warm up, they expand into the housing.  This means that to remove the bearings, the body they are in will likely need to be destroyed, or you may try softening the plastic, but that could also melt the grease out of the bearings.
### Shaft Fit
Since the drive and idle bodies are shared, but the spacers and shafts are not, the bearing fit to the shafts should be a sliding clearance fit (https://en.wikipedia.org/wiki/Engineering_fit#Clearance_fits).  Again, I've adjusted the dimensions so that _my_ 3D outputs that result.