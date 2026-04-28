**Validation and Equivalence**
- Does layout match schematic?
- Does schematic match RTL
- Does RTL match behavioral model 
- Does Behavior Model match intended design

![[ECE 571 - Lecture 27.png]]


**Layout Validation**
- Need to demonstrate that
	- design meets specification
	- protocol between units is correct and robust
	- Specification is correct
- Typically this is accomplished with hardware description languages and simulation software
	- HDL is typically Verilog or VHDL 

- Usually "divide and conquer"
	- Validate each unit separately 
	- Validate all units in a module
	- Validate all modules within a chip
	- Validate all chips within a system


**Test Vectors**
- Describes "proper" behavior of the DUT (Device under test)
	- Typically capture both functional behavior as well as electrical behavior 

- Stimulus 
	- Specifies a set of inputs to the DUT
	- Varies over time

- Response 
	- Describes the expected outputs from the DUT given the stimulus 
	- Varies over time


**Logical Validation methodology**
![[ECE 571 - Lecture 27-1.png]]

![[ECE 571 - Lecture 27-2.png]]
![[ECE 571 - Lecture 27-3.png]]


**Test Vectors II**
- Set of patterns applied to inputs and a set of expected outputs
- May be coded explicitly - All ones, All zeros, Walking ones, etc.
- May be coded implicitly
	- Emulators - "issue memory read to address 0xab01"
	- Checkers - "is proper bus protocol being adhered to?"

**Logic Validation Approaches**
- Exhaustive testing
- Directed testing
- Random testing


**Testbenches**
- testbench - also called a Harness - is a piece of HDL code that is places as wrapper around a piece of HDL, that models the design under test to apply and check test vectors.
![[ECE 571 - Lecture 27-4.png]]

**Regression Testing**
- A suit of tests generally run automatically from scripts
- Multiple levels of regression suits are usually defined 
	- Shorter suits to demonstrate that a logic change doesn't break existing functionality 
	- Longer suits to demonstrate that a logic change is correct
	- Full suits to demonstrate that a design meets specifications 

**Version Control**
- Medium complexity designs and higher require a versioning system to allow orderly changes into the design
- Regression testing is an important component of accepting a design change into the main trunk
- Applies to both logic and validation collateral (checkers, emulator, test vectors)
- Can use CVS, Subversion, Git, or other versioning software

**Bug Tracking and Management**
- Medium complexity designs and higher require an organized approach to logging, approving and fixing bugs
- A robust bug tracking system allows the collection of all the data needed to reproduce, diagnose, and fix a bug as well as assessing the costs of a fix
- Ideally the bug tracking system can apply to both presilicon and postsilicon phases of a design
- Can also used by a person or committee that determines which needs to be addressed, how they are fixed and the timeline for doing so

**Performance Validation**
- A design may be functionally correct but not meet the minimum performance requirements
- Logic validation methodologies tend to focus on "corner" or "edge cases" while performance validation requires large number of cycles of typical operations 
- Can use logic validation testbenches if performance "kernels" can be identified and written along with checking or self checking
- Usually very high-level models are developed specifically for performance testing
- Equivalence between HDL models and these very high level models can be difficult to prove 

*Silicon Test*
**Testers**
- Manufacturing test occurs at several levels and points within the fabrication process
	- Wafer level
	- Packaged part
	- Custom PCB
	- In system
- The cost of finding a defective part goes up as we move down the list
	- Visibility into the failure goes down

**Test flow**
- Apply voltages
- Apply clocks and signals
- Record Signals 
- Check Responses 
- Log errors


*Post-Si Debugging*
**Debugging Overview**
- Challenge: determine cause of failure of a VLSI circuit
- PCB debug techniques dont apply
- Three strategies 
	- Manufacturing test vectors
	- Contact and con-contact probing
	- Voltage, Timing and temperature sensitivities


**Failures**
- Debugging needs to identify the type of failure
	- Manufacturing defects
	- Electrical bug (speed path, race, leakage, etc.)
	- Functional Bug
- Then it needs to get to the root cause

**Physical probing**
- Can probe pads/pins with standard tester
- If probe points were added to layout can use a picoprobe

**E-Beam Probing**
- A special version of a scanning electron microscope 
- It can measure voltages on metal lines, poly and diffusions vs. time similar to an oscilloscope
- The high energy electrons form the beam generate low energy secondary electrons - The number of secondary electrons correspond to voltage
-  A repeating pattern must be used at the target


**Laser Voltage Probing**
- For flip-chip ICs
- Laser scanning microscope using infrared lasers
- Measures voltage of diffusion regions - the amount of reflected light from a P-N junction is affected by the electromagnetic field there 
- Like E-Beam probing, requires a looping test pattern at the target to reconstruct a signal waveform 
- Can disturb sensitive dynamic nodes 

**Other techniques**
- Picosecond imaging circuit analysis
	- PICA is passive and thus non-invasive 
	- Captures light generated when a FET switches 
- Infrared imaging
	- Used to identify hot spots 

**Focused Ion Beam**
- A FIB can cut wires or create new ones
- It can be used to repair defects or test bug fixes
- It can't add new FETs and requires sufficiently large metal areas to connect 
- These areas can be added to designs to provide for this possibility
- For flip-chip designs, this must be accomplished from the back side

**Shmoo Plots**
- Usually a plot of voltage vs speed for a given test vector
- Typically used to diagnose electrical failures
- Shape of plot can give clues to root cause 