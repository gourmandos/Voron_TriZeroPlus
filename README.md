# Voron_TriZeroPlus

### Configs:

Tri-Zero+2xHuvud - [double-dragon_octopus](https://github.com/zruncho3d/double-dragon/tree/main/Config/Octopus/Tri-Zero%2B2xHuvud)

Change hybrid-corexy --> corexy

PRINT_START is inadequate grab that one from here:
 
Klipper_2xSKR_2xEBB - [DuelingZero](https://github.com/zruncho3d/DuelingZero/tree/main/Configs/Klipper_2xSKR_2xEBB)

--------

T0 BoxZero - [Voron BoxZero](https://github.com/rplanier/Voron-BoxZero)

### Bed mesh debug - Zruncho

If you find you're not getting convergence within 2 or 3 retries reliably, here's some debug tips:
(1) double-check the ZeroClick probe offsets (starter values here: https://github.com/zruncho3d/double-dragon/blob/main/Config/Octopus/Tri-Zero%2B2xHuvud/printer.cfg)
(2) bump tolerance to 0.01 or even 0.015 temporarily (I usually run 0.0075 on all printers)
(3) check for no axis binding or looseness near bed joints
(4) ensure your microstepping on Z is maxed out; 64x seems good
(5) bump currents, especially if using NEMA17s, to get the most out of microstepping; you won't need this to hold the bed, but more, to overcome the static friction for small moves
(6) double-check that there's no rocking in your ZeroClick and that the magnet are perfectly parallel.  They should be if you pressed them into place with a clamp.  
 

A little more advanced: run many cycles to get a baseline for how many cycles are expected.  This is why I know some of the items above.  

Code for that here: https://github.com/zruncho3d/printer-experiments


