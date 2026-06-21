# bjunverse26

## 소개

RTL 설계와 검증, FPGA 기반 디지털 시스템, 임베디드 펌웨어를 중심으로 학습하고 구현하고 있습니다. 하드웨어 인터페이스와 실시간 제어 시스템을 직접 설계하며, 설계 의도를 테스트벤치와 검증 환경으로 확인하는 과정을 중요하게 생각합니다.

현재는 디지털 회로 설계, SoC 인터페이스, FPGA 가속기, 메모리 회로, 임베디드 제어 펌웨어를 중심으로 포트폴리오를 정리하고 있습니다.

## 관심 분야

| 분야 | 내용 |
| --- | --- |
| RTL Design & Verification | Verilog/SystemVerilog 기반 RTL 설계, SVA, self-checking testbench |
| FPGA / Digital System | Vivado 기반 FPGA 설계, 연산 가속기, timing closure |
| Memory / Custom IC | SRAM, PUF, custom layout, MPW, chip measurement |
| SoC Interface | AXI4-Lite, UART, CDC, memory-mapped peripheral |
| Embedded Firmware | C 기반 하드웨어 제어, timer interrupt, sensor/PWM interface |
| Control System | DSP 기반 모터 제어, 실시간 제어 루프, MATLAB/Simulink 연계 |

## 대표 프로젝트

### Capstone Design

**9T Dual-Mode SRAM PUF 설계 및 MPW 제출**

- PUF reliability와 SRAM read latency/power trade-off를 함께 고려한 9T dual-mode SRAM PUF architecture를 설계했습니다.
- PUF mode에서는 mismatch를 증가시켜 reliability를 높이고, normal mode에서는 6T SRAM에 가까운 latency/power 특성을 확보하도록 구성했습니다.
- 16x16 SRAM array, precharge circuit, sense amplifier, write driver, column mux, row decoder를 통합했습니다.
- ETRI My Chip MPW service를 통해 GDS를 제출하고, fabricated die 측정을 위한 KiCad PCB와 Arty S7-25T FPGA 기반 제어 환경을 준비하고 있습니다.

### Digital System Design

**FPGA 기반 SRCNN 이미지 업스케일링 가속기 설계**

- Q8.8 fixed-point 기반 3-layer SRCNN 연산 구조를 RTL로 구현했습니다.
- Recursive 및 Streamline 구조를 포함한 3가지 아키텍처를 설계했습니다.
- Line Buffer, PE Array, Controller FSM, Packed Activation Memory를 구성했습니다.
- C++ reference와 RTL 결과를 bit-level로 비교하고 100 MHz timing을 검증했습니다.

[Digital_System_Design](https://github.com/bjunverse26/Digital_System_Design)

### AXI4-Lite / AXI4-UART

**Memory-mapped peripheral RTL 설계 및 검증**

- 32-bit AXI4-Lite slave와 UART peripheral을 구현했습니다.
- AW/W channel 도착 순서, read/write backpressure, invalid address response를 검증했습니다.
- Directed testbench와 SVA를 분리하여 protocol 동작을 확인했습니다.

[AXI4_Lite](https://github.com/bjunverse26/AXI4_Lite) / [AXI4_UART](https://github.com/bjunverse26/AXI4_UART)

### Async FIFO & CDC

**Clock Domain Crossing 설계 및 self-checking 검증**

- Gray-code pointer와 2-FF synchronizer 기반 dual-clock FIFO를 구현했습니다.
- Full/empty flag, request/acknowledge handshake CDC 구조를 설계했습니다.
- Queue scoreboard 기반으로 데이터 순서와 무결성을 검증했습니다.

[Async_FIFO](https://github.com/bjunverse26/Async_FIFO)

### Mechatronics Motor Control

**DSP 기반 실시간 모터 제어 펌웨어**

- TI C6701 DSP의 timer interrupt 기반 실시간 제어 루프를 구현했습니다.
- Encoder, Hall sensor, PWM 출력을 이용해 DC/STEP/BLDC motor 제어를 수행했습니다.
- Inverted pendulum의 swing-up 및 balancing 제어를 구현했습니다.
- MATLAB/Simulink 모델과 Embedded C 기반 DSP 제어 실습을 연계했습니다.

[Mechatronics](https://github.com/bjunverse26/Mechatronics)

### PIM Framework

**PIM hardware effect 및 quantization simulation**

- Llama 추론 경로에서 quantization과 PIM hardware effect를 모델링했습니다.
- 하드웨어 제약이 추론 결과에 미치는 영향을 simulation 관점에서 분석했습니다.

[PIM_Framework](https://github.com/bjunverse26/PIM_Framework)

## 기술 스택

| 구분 | 기술 |
| --- | --- |
| HDL / Verification | Verilog, SystemVerilog, SVA |
| FPGA / EDA | Vivado |
| Circuit / Layout | Cadence Virtuoso, KiCad |
| Embedded / Software | C, C++, Python |
| Modeling / Analysis | MATLAB, Simulink |
| Development Tools | Git, GitHub |

## 지향점

하드웨어 구조를 이해하고 RTL로 구현하는 능력, 검증 환경을 통해 설계 신뢰도를 높이는 능력, 그리고 실제 보드에서 동작하는 펌웨어를 작성하는 능력을 함께 키우고 있습니다. 장기적으로는 디지털 시스템과 임베디드 하드웨어가 맞물리는 영역에서 실무 역량을 쌓고자 합니다.
