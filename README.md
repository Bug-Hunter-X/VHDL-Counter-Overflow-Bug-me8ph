# VHDL Counter Overflow Bug
This repository demonstrates a common bug in VHDL code: improper handling of counter overflow.  The `buggy_counter` entity attempts to implement a simple 4-bit counter, but the `else` case within the `rising_edge(clk)` process does not reset the counter correctly. This can lead to unexpected outputs, simulation failures, or synthesis issues, depending on how the simulator or synthesizer handles the integer overflow.

The solution demonstrates how to correctly handle the counter overflow and reset the counter to 0 when it reaches its maximum value.