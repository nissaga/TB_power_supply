# Why the fuse doesn't work

In the output line of the LM317 there is a fuse of 1.6A to protect it from shortcircuit. However, I have made some shortcircuits (accidentally) and the LM was left unoperable whereas the fuse was still intact.

It's just a suposition, but in the datasheet of LM317 says:
"The LM317 device is an adjustable three-terminal positive-voltage regulator capable of supplying more than 1.5 A over an output-voltage range of 1.25 V to 37 V."
However, the maximum output current is 1.5A. More in concrete, the section 8.3.2 of the datasheet (Overload block) says:
"Over-current and over-temperature shutdown protects the device against overload or damage from operating in excessive heat."

Therefore, is more than possible that this is the cause of the fuse don't workin.

Just to be shure, the easiest way is to obtain a fuse lower than 1.5A and do a shortcircuit.

But as I don't have any, I will not test it.
