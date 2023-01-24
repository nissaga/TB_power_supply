# TB_power_supply
How to create the definitive test bench power supply from an ATX-power supply

#Motivations
I made one power supply from an atx of an old computed. It had different fixed voltages (12, 5, 3.3V) and a variable output (12-0 V) made with the typical LM317. It does the work, but there are some things to improve:
- The form factor. All the cables and circuits are in the typical transparent plastic candy box. Therefore, it's awful
- There isn't any current limitation. I couldn't understand how to make it, therefore it only has a fuse
- Not shortcircuit protected. If in the adjustable voltage line, a short circuit is generated, the LM317 gets burned and you have to replace it. In the line there is a fuse, but does not protect anything
- It is possible to get more voltage than 12V?

#Planification
The best thing to do now is to think about the next steps
- [x] Why the fuse doesn't do anything?
- [X] Why the LM317 get burned
- [ ] Review bibliography
- [x] There is a more updated option than the LM317?
- [x] How to create the current limitation circuit
- [ ] Will fit?
