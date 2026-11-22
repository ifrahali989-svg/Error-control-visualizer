# Error-control-visualizer
Interactive AlgoVision-style web visualizer demonstrating error control mechanisms, noisy communication channels, bit-flip fault injection, and real-time Python calculation tracing.

# Error Control & Noisy Communication Channel Visualizer

An interactive, dark-themed educational web application designed to simulate data transmission over a noisy communication channel and visualize real-time error detection logic alongside synchronized Python code execution.

## Overview

This tool allows users to input custom binary sequences or decimal numbers and observe how redundant check bits are generated, transmitted across an unreliable medium, and verified at the receiver end. Every mathematical step and variable state updates dynamically as inputs or channel faults are modified.

## Key Features

- **Custom Live Inputs:** Accepts arbitrary binary bitstreams or decimal integers with instant conversion and codeword generation.
- **Noisy Channel Simulation:** Interactive transmission pipeline (`Sender TX` -> `Noisy Channel` -> `Receiver RX`) supporting single-bit errors, burst errors with live burst-length measurement, double-bit errors, and manual bit-flipping on click.
- **Real-Time Error Detection Algorithms:**
  - **Simple Parity (Even / Odd):** Demonstrates single-bit detection and even-number bit-flip blind spots.
  - **Cyclic Redundancy Check (CRC-3):** Live modulo-2 binary polynomial division (`1101` generator) showing step-by-step XOR operations.
  - **Internet Checksum:** 1's complement binary addition and wrap-around carry calculation.
- **Synchronized Python Execution Trace:** Displays step-by-step Python implementation logic with live variable inspection and playback controls (`Auto Play`, `Next Step`, `Reset`).
- **Networking Terminology Explorer:** Built-in reference covering redundancy, Hamming distance, burst length, syndrome, and modulo-2 arithmetic.

## Usage

1. Clone or download the repository.
2. Open `index.html` directly in any modern web browser (no backend server or external dependencies required).
3. Enter a binary or decimal value, select an error-detection scheme, and inject channel noise to observe the detection outcome.
