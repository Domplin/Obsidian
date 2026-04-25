Self boosting is a technique used in NAND flash memory to prevent program disturb on unselected cells sharing the same bit line or word line during a program operation 

During programming, a high voltage (15-20V) is applied to the selected wordline. All cells in the same NAND string ([[NAND Array Structure]]) share this bitline. Unselected cells on inhabited bitlines (those not being programmed) are at risk of being unintentionally programmed by this high field 


**How self Boosting Works**
The core Idea is to float the channel of unselected 