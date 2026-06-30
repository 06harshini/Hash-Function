# SimpleHash – 8-bit Keyed Hash Function

## Overview

SimpleHash is a lightweight 8-bit keyed hash function implemented in Verilog. It demonstrates basic hashing concepts using XOR operations, bit rotations, shifts, and a custom 4-bit S-Box.

## Features

- 16-bit message input
- 8-bit secret key
- 8-bit hash output
- Two rounds of mixing
- Custom 4-bit S-Box
- Avalanche effect demonstration
- Exhaustive testing of all 65,536 input values
- VCD waveform generation

## Files

- `SimpleHash.v` – Hash function and testbench

## Running the Simulation

Using Icarus Verilog:

```bash
iverilog -o SimpleHash SimpleHash.v
vvp SimpleHash
```

To view waveforms:

```bash
gtkwave SimpleHash.vcd
```

## Testbench

The testbench:
- Tests sample input messages
- Demonstrates the avalanche effect
- Performs an exhaustive distribution test over all 16-bit inputs
- Reports the number of distinct hash values and bucket statistics
