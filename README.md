# wasm-metal
A bare metal physical implementation of WebAssembly. That's right, a WebAssembly CPU.

## Why is this a good idea?

* The world is moving to WebAssembly
* Some of the biggest and potentially most world-changing projects are implementing their virtual machines as WebAssembly virtual machines (DFINITY, Ethereum)
* The bytecode is being designed as a compilation target for low-level languages first
* The bytecode is meant to execute at near-native speeds on a variety of underlying ISAs
* Java processors already offer potential benefits, even being compilation targets for a high-level language
* Cutting out the translation from WebAssembly to the underlying ISAs could provide efficiency benefits
* We could get rid of WebAssembly virtual machines entirely, and replace them with WebAssembly physical machines

## Roadmap

- [ ] Understand the WebAssembly ISA
- [ ] Implement the mircoarchitecture in HTML/CSS/JavaScript
  * This will be a GUI simulator of the microarchitecture
  * This simulator will become the specification for the microarchitecture
  * It will allow us to quickly experiment with hardware configurations
  * It will allow us to iterate and learn how the microarchitecture should work
- [ ] Implement the microarchitecture as an RTL design in an HDL
- [ ] Simulate the RTL design
- [ ] Test the implementation on an FPGA
- [ ] Design the ASIC