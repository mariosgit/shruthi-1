# How to convert a pcb

1. Start KICAD with no project opened
2. File / Import NOnKiCad.. / Eagle...
3. Select the board or schematics file you want to import.. (it will import both, no matter which you choose)
4. It will ask for a project dir, I would use ../pcb-kicad for all converted pcbs. If you choos existing proj dir, it will complain, ignore it say "no".
5. A Layer mapping dialog will open
   * Click the auto match button below
   * Now select "Milling" from the left list and double click "Edge.Cuts" under KiCAD Layers this will add this mapping to the list on the right.
   * Click OK
6. Save PCB and Schematic !
7. Try to F8 in the PCB, look if that removes things or not !?
8. Run a DRC check. Most of the "fails" are related to silkscreen, text, artwork and can be ignored, watch out for real problems on the copper layers.
9. Save again, Done.

# PS

If you convert all PCBs into one directory like I did, you need to **open the xy.pro file before** you can usefully edit the xy sch/brd.
