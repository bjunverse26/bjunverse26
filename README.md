# bjunverse26

**RTL Design · Verification · FPGA · Embedded Firmware · Memory/Custom IC**

디지털 시스템을 RTL로 구현하고, 검증 환경과 실제 하드웨어 동작 확인까지 연결하는 엔지니어링 역량을 쌓고 있습니다.

관심 분야는 **디지털 회로 설계**, **SoC 인터페이스**, **FPGA 가속기**, **메모리 회로**, **임베디드 제어 펌웨어**입니다.

## 🎯 핵심 역량

| 분야 | 역량 |
| --- | --- |
| RTL Design & Verification | Verilog/SystemVerilog 기반 RTL 설계, SVA, self-checking testbench |
| FPGA / Digital System | Vivado 기반 FPGA 구현, 연산 가속기 구조 설계, timing 검증 |
| Memory / Custom IC | SRAM PUF architecture, custom layout, MPW 제출, chip measurement 준비 |
| SoC Interface | AXI4-Lite, UART, CDC, memory-mapped peripheral 설계 |
| Embedded Firmware | C 기반 register-level 제어, timer interrupt, sensor/PWM interface |
| Control System | DSP 기반 모터 제어, 실시간 feedback loop, MATLAB/Simulink 연계 |

## 📌 대표 프로젝트

### 1. Capstone Design

**9T Dual-Mode SRAM PUF 설계 및 MPW 제출**

핵심 성과: **PUF 신뢰성과 SRAM normal-mode 성능을 함께 고려한 dual-mode memory architecture 설계**

- PUF mode: cascode PMOS mismatch를 활용한 reliability 향상 구조
- Normal mode: 6T SRAM에 가까운 read latency/power 특성 확보를 목표로 한 dual-mode 동작
- 16x16 SRAM array, precharge circuit, sense amplifier, write driver, column mux, row decoder 통합
- ETRI My Chip MPW service를 통한 GDS 제출
- Fabricated die 측정을 위한 KiCad PCB 및 Arty S7-25T FPGA 기반 제어 환경 준비

### 2. Digital System Design

**FPGA 기반 SRCNN 이미지 업스케일링 가속기 설계**

핵심 성과: **Q8.8 fixed-point 기반 3-layer SRCNN 연산을 FPGA용 RTL architecture로 구현**

- Recursive 및 Streamline 구조를 포함한 3가지 SRCNN accelerator architecture 설계
- Line Buffer, PE Array, Controller FSM, Packed Activation Memory 구성
- C++ reference와 RTL 결과의 bit-level 비교 검증
- 100 MHz timing 기준의 FPGA 구현 가능성 확인

[Digital_System_Design](https://github.com/bjunverse26/Digital_System_Design)

### 3. AXI4-Lite / AXI4-UART

**Memory-mapped peripheral RTL 설계 및 검증**

핵심 성과: **AXI4-Lite slave와 UART peripheral을 직접 설계하고 protocol edge case 검증**

- 32-bit AXI4-Lite slave interface 및 UART peripheral RTL 설계
- AW/W channel 도착 순서, read/write backpressure, invalid address response 처리
- Directed testbench와 SVA를 분리한 protocol 검증 환경 구성
- Register map 기반 memory-mapped peripheral 동작 확인

[AXI4_Lite](https://github.com/bjunverse26/AXI4_Lite) / [AXI4_UART](https://github.com/bjunverse26/AXI4_UART)

### 4. Async FIFO & CDC

**Clock Domain Crossing 설계 및 self-checking 검증**

핵심 성과: **dual-clock 환경에서 데이터 무결성을 보장하는 CDC 구조 설계 및 검증**

- Gray-code pointer와 2-FF synchronizer 기반 dual-clock FIFO 설계
- Full/empty flag 및 request/acknowledge handshake CDC 구조 구현
- Queue scoreboard 기반 데이터 순서 및 무결성 검증
- 비동기 클럭 조건에서 overflow/underflow 방지 시나리오 확인

[Async_FIFO](https://github.com/bjunverse26/Async_FIFO)

### 5. Mechatronics Motor Control

**DSP 기반 실시간 모터 제어 펌웨어**

핵심 성과: **TI C6701 DSP 기반 register-level 제어와 실시간 feedback loop 구현**

- Timer interrupt 기반 1 kHz 실시간 제어 루프 구성
- Encoder, Hall sensor, PWM 출력을 이용한 DC/STEP/BLDC motor 제어
- Inverted pendulum의 swing-up 및 balancing 제어 구조 구현
- MATLAB/Simulink 모델과 Embedded C 기반 DSP 제어 실습 연계

[Mechatronics](https://github.com/bjunverse26/Mechatronics)

### 6. PIM Framework

**PIM hardware effect 및 quantization simulation**

핵심 성과: **LLM inference 경로에서 hardware non-ideality가 결과 품질에 미치는 영향 분석**

- Llama 추론 경로의 quantization 및 PIM hardware effect 모델링
- Retention, noise, ADC error 등 hardware constraint 반영
- PPL 기반 inference 품질 변화 분석

[PIM_Framework](https://github.com/bjunverse26/PIM_Framework)

## 🛠 기술 스택

| 구분 | 기술 |
| --- | --- |
| HDL / Verification | Verilog, SystemVerilog, SVA |
| FPGA / EDA | Vivado |
| Circuit / Layout | Cadence Virtuoso, KiCad |
| Embedded / Software | C, C++, Python |
| Modeling / Analysis | MATLAB, Simulink |
| Development Tools | Git, GitHub |

## 🚀 지향점

하드웨어 구조를 이해하고 RTL로 구현하는 능력, 검증 환경으로 설계 신뢰도를 높이는 능력, 실제 보드와 칩에서 동작을 확인하는 능력의 균형 있는 성장.

장기적으로는 디지털 시스템과 임베디드 하드웨어가 맞물리는 영역에서 실무 역량 축적.
