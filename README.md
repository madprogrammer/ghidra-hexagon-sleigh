### Ghidra Hexagon SLEIGH

This is a WIP implmementation of the Hexagon architecture in pure SLEIGH


Supports:
- Dissassembly up to v73, (except extended instructions)
- No broken java plugins needed
- Initial support for hardware loops
- Pcode implemented for most common ops (Missing < 1% for most binaries)

Currently broken / unimplemented:
- No support for GPR.new (Pred.new is supported)
- No suport for hw loops with terminating packets of size > 2
- No FP or COMPLEX ops
- No vector ops
- Some immediate extentions are ignored or affect multiple instructions in a packet


(See notes at top of `Hexagon/data/languages/skel.slaspec`) for up to date details:


### How to install
Copy `Hexagon` into `./<ghidra_root>/Ghidra/Processors/` (Confirmed to work on 11.2.1)
