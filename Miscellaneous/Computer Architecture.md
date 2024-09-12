# [Computer Architecture By Dr. Onur Mutlu ETH Zurich](https://www.youtube.com/playlist?list=PL5Q2soXY2Zi-EImKxYYY1SZuGiOAOBKaf)

- **[CPU Power Consumption (roughly)](https://electronics.stackexchange.com/questions/33318/power-consumed-by-a-cpu)**:
    - **Dynamic Power Consumption** = `1/2 * C * V^2 * f`
    - **Static Power Consumption** = `V * I_leakage`

- **[FinFET](https://en.wikipedia.org/wiki/FinFET)**: A type of non-planar transistor, or "3D" transistor, used in modern processors. 
- **[EUV (Extreme Ultraviolet Lithography)](https://en.wikipedia.org/wiki/Extreme_ultraviolet_lithography)**: A technology used in semiconductor fabrication to produce microchips.
- **[FPGA (Field-Programmable Gate Array)](https://en.wikipedia.org/wiki/Field-programmable_gate_array)**: An integrated circuit designed to be configured by a customer or a designer after manufacturing. (Multiplexers are critical components)
- **[Tri-State Buffer](https://en.wikipedia.org/wiki/Three-state_logic)**: Allows an output to assume a high, low, or high-impedance state, useful in bus-oriented systems.
- **[SoftMC](https://github.com/CMU-SAFARI/SoftMC)**: A software-based memory controller for experimental DRAM testing.
- **[DRAM-Bender](https://github.com/CMU-SAFARI/DRAM-Bender)**: A tool for testing and understanding DRAM vulnerabilities, like Row-Hammer.
- **[Row-Hammer](https://en.wikipedia.org/wiki/Row_hammer)**: Accesing a row of memory cells repeatedly can cause bit flips in adjacent rows.
- **Timing Parameters**:
    - **t_setup (Setup Time)**: The minimum time before the clock edge that the input signal to a flip-flop must be held constant.
    - **t_hold (Hold Time)**: The minimum time after the clock edge that the input signal to a flip-flop must remain constant.
    - **t_skew (Clock Skew)**: The variation in timing of the clock signal as it is distributed across different parts of a circuit.
- **[Memory Wall](https://en.wikipedia.org/wiki/Memory_wall)**: A performance bottleneck in computing where the time taken to access memory is significantly longer than the time taken to perform operations on the data.
- **Opcode**: The portion of a machine language instruction that specifies the operation to be performed.
- **Operands**: The subjects of the operation (e.g., constants, memory addresses).
