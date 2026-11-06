# 04 | Qubit Measurements with FPGA and QICK

Our lab uses an FPGA-based QICK setup to control and measure superconducting qubits. QICK stands for Quantum Instrumentation Control Kit. It provides open-source firmware and software for RFSoC boards. An FPGA is a programmable hardware device. In this setup, it runs pulse sequences and synchronizes readout acquisition with the pulses. The board's DACs convert digital waveforms into analog signals, and its ADCs digitize the returning readout signal. [Official QICK repository](https://github.com/openquantumhardware/qick)

## Where to Learn

1. Start with the official Quick Start to learn how to set up the board and run a first pulse experiment. [QICK documentation](https://docs.qick.dev/latest/)
2. For single-qubit measurements, open **demo 06** in the official `qick_demos` folder. Follow how the notebook defines pulse parameters, sweeps a variable, and acquires readout data. [06_qubit_demos.ipynb](https://github.com/openquantumhardware/qick/blob/main/qick_demos/06_qubit_demos.ipynb)
3. For the scripts used in our lab, see our internal measurement repository. [tprocv2_guidemo](https://github.com/JayChien04717/tprocv2_guidemo)
