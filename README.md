# TB_power_supply
How to create the definitive test bench power supply from an ATX-power supply

# Motivations
I made one power supply from an atx of an old computed. It had different fixed voltages (12, 5, 3.3V) and a variable output (12-0 V) made with the typical LM317 circuit. It does the work, but there are some things to improve:
- The form factor. All the cables and circuits are in the typical transparent plastic candy box. Therefore, it's awful
- Not shortcircuit protected. If in the adjustable voltage line, a short circuit is generated, the LM317 gets burned and you have to replace it. In the line there is a fuse, but does not protect anything. Why??
- I would love to have some current limitation to protect the tested equipment
- It is possible to get more voltage than 12V?

![My image](/images/old_BS1.jpg "The old one")

# Preamble
## Checklist
The best thing to do now is to think about the next steps
- [x] Why the fuse doesn't do anything?
- [X] Why the LM317 get burned
- [X] Review bibliography
- [x] There is a more updated option than the LM317?
- [x] How to create the current limitation circuit

## Why the fuse didn't work and the LM317 get burned
In a nutshell, the fuse was 1,6 A, while the LM317 has a protection against higher currents (1.5A). Therefore the fuse did nothing. So, the protection of the LM317 kind of turned off the circuit. I could not recall if the LM317 get burnt or only was out for some days. 

## Review the bibliography
I have check the different power supplys that I think I could construct with my tools and knowledge. This is further explained in the Bibliography.md document.

## How to create the current limitation circuit and higher voltages
I have tried to understand some current limitation circuits. I do not understand how they work and felt like if I was stucked there I will drop the project. Therefore I moved to a much simple solution, use a buck-boost converter. 
In this way, I could have a higher range of voltage and some nice features like current regulation

# Design
