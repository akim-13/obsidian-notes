# Address bus
**Address bus** — a [[Buses|bus]] that is used to send an address of a
particular main memory location requested by the [[CPU]].

Memory is divided up internally into units called **words**.

**Word** — a fixed size group of digits, typically 16, 32 or 64 bits, which is
handled as a unit by the processor, and different types of processor have
different word sizes.

The address bus transmits the memory addresses of words that are used as
operands in program instructions, so that the data can be retrieved and sent
back to the processor. 

When an instruction has been performed and the result is to be stored at a
particular memory location, it is transmitted via the [[Data bus|data bus]].
