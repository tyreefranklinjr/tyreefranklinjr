<h1 align="center">Tyree Franklin Jr.</h1>
<h3 align="center">RF Software • Embedded Systems • Real-Time C++ / Rust / Linux</h3>

<p align="center">
  <a href="https://www.linkedin.com/in/tyree-franklin-jr/">
    <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" />
  </a>
  <a href="mailto:tyree.franklinjr@gmail.com">
    <img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" />
  </a>
  <a href="https://github.com/tyreefranklinjr">
    <img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" />
  </a>
</p>

<p align="center">
  I build performance-critical software at the <b>RF / systems boundary</b>:
  SDR/DSP pipelines, resilient communications, embedded autonomy, and hardware/software integration.
</p>

<p align="center">
  <b>U.S. Citizen</b> • Fort Worth, TX • B.S. Computer Science @ WGU
</p>

---

## RF / Systems Snapshot

|                                                          |                                                |
| -------------------------------------------------------- | ---------------------------------------------- |
| **1.024 MS/s** IQ throughput                             | **< 4 ms p99** DSP latency                     |
| **< 1% BER @ 8 dB Eb/N0** across 1M+ bits                | **99.99%** block delivery over 60 min          |
| **0 steady-state heap allocations** in DSP critical path | **4096-point FFT** deterministic RF validation |
| **< 250 ms** communications failover                     | **500+** automated SIL/HIL fault scenarios     |

<p align="center">
  <img
    src="./rocket.gif"
    width="400"
    alt="Rocket flight test"
  />
</p>

---

## Algorithms & Systems I Implement

```text
IQ samples
   ↓
DC correction → DDC → FIR / decimation → preamble correlation
   ↓
carrier + timing synchronization
   ↓
soft decisions → Viterbi decode → CRC validation
```

**DSP / Communications**
`BPSK` · `QPSK` · `FFT` · `FIR` · `CRC-32` · `Convolutional FEC` · `Soft-Decision Viterbi` · `BER/PER Analysis`

**Real-Time Systems**
`Bounded SPSC Queues` · `Backpressure` · `Zero-Allocation Critical Paths` · `IQ Record/Replay` · `Deterministic Testing`

**Embedded / Autonomy**
`FreeRTOS` · `CAN/TWAI` · `EKF Sensor Fusion` · `PID Control` · `A* Planning` · `Watchdogs`

**Resilient Communications**
`ACK/Retry` · `Sequence Tracking` · `Duplicate Suppression` · `Link Scoring` · `Hysteresis Failover`

---

## RF Validation

<p align="center">
  <a href="https://github.com/tyreefranklinjr/TeleComms--Software-Defined-Comms">
    <img
      src="https://raw.githubusercontent.com/tyreefranklinjr/TeleComms--Software-Defined-Comms/main/figures/ber_vs_ebn0_awgn.png"
      width="49%"
      alt="Empirical BER versus theoretical BER over AWGN"
    />
  </a>
  <a href="https://github.com/tyreefranklinjr/TeleComms--Software-Defined-Comms">
    <img
      src="https://raw.githubusercontent.com/tyreefranklinjr/TeleComms--Software-Defined-Comms/main/figures/frame_error_rate.png"
      width="49%"
      alt="Frame error rate under channel noise"
    />
  </a>
</p>

<p align="center">
  <sub>
    Monte Carlo link validation — empirical BER vs. closed-form
    Q(√(2·Eb/N0)) theory and frame-level degradation under channel noise.
  </sub>
</p>

<p align="center">
  <a href="https://github.com/tyreefranklinjr/TeleComms--Software-Defined-Comms">
    <b>View RF simulation + statistical analysis →</b>
  </a>
</p>

---

## Selected Engineering Work

### Real-Time Software-Defined Communications + RF Processing

`C++20` `C` `Rust` `Python` `Linux` `RTL-SDR` `FFTW` `CMake/Ninja` `Nix`

* Sustained **1.024 MS/s IQ processing** with **<4 ms p99 DSP latency**, bounded queues, explicit backpressure, and zero steady-state allocation in the critical path.
* Implemented **BPSK/QPSK**, CRC-32 framing, **rate-1/2 K=7 convolutional FEC**, soft-decision Viterbi decoding, synchronization, and BER/PER validation.
* Achieved **<1% BER at 8 dB Eb/N0 across 1M+ simulated bits**.
* Built **4096-point FFT**, deterministic IQ record/replay, fault injection, and endurance validation with **99.99% block delivery over 60 minutes**.

### Resilient Autonomous Mission Computer

`C++20` `C` `Rust` `FreeRTOS` `ESP32-C3` `CAN/TWAI` `EKF` `PID` `A*`

* Architected a distributed **4-node** embedded system with real-time tasks up to **50 Hz**, CAN/TWAI, IMU/GNSS fusion, watchdogs, and bounded-memory execution.
* Maintained autonomous mission execution through **30 seconds of complete communications loss** with **<250 ms failover**.
* Implemented **EKF state estimation, PID control, A* planning**, degraded-mode recovery, stale-data rejection, and link-health scoring.
* Achieved **100% safe-state transition success across 500+ automated SIL/HIL fault scenarios**.

### Live RF / Fixed-Wireless Operations

* Diagnose physical wireless links using **constellation diagrams, SNR, packet loss, MTR, and radio telemetry**.
* Identify RF interference, intermittent **QAM downshift**, radio-side faults, backhaul failures, and routing issues across roughly **30 cases/day**.
* Work directly with network and tower engineering on RF alignment, backhaul, and field infrastructure.

---

## Core Stack

`C++20` · `Rust` · `C` · `Python` · `Linux` · `SDR` · `DSP` · `FreeRTOS` · `Sockets` · `TCP/UDP` · `CAN/TWAI` · `CMake` · `Nix` · `Docker` · `pytest` · `GoogleTest`

---

<p align="center">
  <b>Interested in building RF communications, autonomous systems, and software that has to work outside the lab.</b>
</p>

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/tyreefranklinjr/tyreefranklinjr/output/github-contribution-grid-snake-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/tyreefranklinjr/tyreefranklinjr/output/github-contribution-grid-snake.svg">
  <img alt="contribution snake" src="https://raw.githubusercontent.com/tyreefranklinjr/tyreefranklinjr/output/github-contribution-grid-snake.svg">
</picture>
