# 👋 Hi, I'm bjunverse

<div align="center">

### Digital Logic · RTL Design · Verification · Mixed-Signal Hardware

Digital 회로 설계부터 Mixed-signal 회로까지 확장 가능한 하드웨어 설계 역량을 쌓고 있습니다.

<br/>

[![GitHub](https://img.shields.io/badge/GitHub-bjunverse26-181717?style=for-the-badge\&logo=github\&logoColor=white)](https://github.com/bjunverse26)
[![Velog](https://img.shields.io/badge/Velog-bjunverse_-20C997?style=for-the-badge\&logo=velog\&logoColor=white)](https://velog.io/@bjunverse_/posts)
[![Email](https://img.shields.io/badge/Email-bjunverse26%40gmail.com-D14836?style=for-the-badge\&logo=gmail\&logoColor=white)](mailto:bjunverse26@gmail.com)

</div>

---

## 🚀 Featured Projects

### 1. AXI4-Lite / AXI4-UART

> AXI4-Lite 기본 slave 구조를 구현하고, 이를 기반으로 UART Core를 제어하는 AXI4-UART peripheral까지 확장한 프로젝트입니다.

**Key Highlights**

* AXI4-Lite `AW -> W`, `W -> AW`, same-cycle write transaction 처리
* Testbench와 SVA를 분리한 구조로 protocol assertion 및 coverage 검증
* AXI4-UART에서 `CTRL`, `STATUS`, `TXDATA`, `RXDATA` 기반 register map 구현
* UART loopback, invalid access, zero strobe, backpressure scenario 검증

**Links**

[![AXI4-Lite](https://img.shields.io/badge/Repo-AXI4__Lite-181717?style=flat-square\&logo=github)](https://github.com/bjunverse26/AXI4_Lite)
[![AXI4-UART](https://img.shields.io/badge/Repo-AXI4__UART-181717?style=flat-square\&logo=github)](https://github.com/bjunverse26/AXI4_UART)

---

### 2. PIM-Quant-Sim / PIM Framework

> Llama 모델을 대상으로 SmoothQuant 및 Bit-slicing 연산을 모델링하고, PIM 하드웨어 비이상성이 모델 성능에 미치는 영향을 분석한 프로젝트입니다.

**Key Highlights**

* SmoothQuant 기반 quantization flow 모델링
* Bit-slicing 연산 구조 시뮬레이션
* Noise, Retention, ADC error 등 아날로그 하드웨어 비이상성 반영
* 하드웨어 제약 조건에 따른 Perplexity(PPL) 성능 분석

**Link**

[![PIM Framework](https://img.shields.io/badge/Repo-PIM__Framework-181717?style=flat-square\&logo=github)](https://github.com/bjunverse26/PIM_Framework)

---

### 3. Mechatronics

> 센서, 구동기, 제어 로직을 단계적으로 실습하며 하드웨어 동작을 고려한 제어 구조를 학습하는 프로젝트입니다.

**Current Progress**

* DC motor 구동 및 기본 제어 실습
* Microcontroller 기반 입출력 제어 흐름 학습
* 실제 하드웨어 동작을 고려한 제어 구조 이해

**Next Steps**

* Stepping motor 및 BLDC motor 제어 실습
* Sensor feedback 기반 제어 시스템 구현
* 최종 자율 프로젝트를 통한 Mechatronics 통합 설계

**Link**

[![Mechatronics](https://img.shields.io/badge/Repo-Mechatronics-181717?style=flat-square\&logo=github)](https://github.com/bjunverse26/Mechatronics)

---

### 4. Digital System Design

> FPGA 기반 RTL 설계와 하드웨어 가속기 구조를 단계적으로 학습하며, 최종적으로 Super Resolution 가속기 설계를 목표로 진행한 프로젝트입니다.

**Key Highlights**

* Vivado 기반 프로젝트 생성, RTL 작성, Testbench simulation 흐름 정리
* MAC, adder tree, pipelined adder tree 등 기본 연산 블록 설계
* BRAM, LUTRAM, URAM, DSP macro 등 FPGA 자원 활용 실습
* Processing Element(PE), 1D/2D convolution, multi-channel 데이터 처리 구조 구현
* Super Resolution accelerator 설계를 위한 사전 구조 학습

**Link**

[![Digital System Design](https://img.shields.io/badge/Repo-Digital__System__Design-181717?style=flat-square\&logo=github)](https://github.com/bjunverse26/Digital_System_Design)

---

## 🧰 Tech Stack

### HDL / Verification

![Verilog](https://img.shields.io/badge/Verilog-808080?style=for-the-badge)
![SystemVerilog](https://img.shields.io/badge/SystemVerilog-1E90FF?style=for-the-badge)

### Software / AI Framework

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge\&logo=python\&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge\&logo=pytorch\&logoColor=white)

### Circuit / EDA Tools

![Cadence Virtuoso](https://img.shields.io/badge/Cadence_Virtuoso-CC0000?style=for-the-badge)
![LTspice](https://img.shields.io/badge/LTspice-900028?style=for-the-badge)
![HSPICE](https://img.shields.io/badge/HSPICE-4B4B4B?style=for-the-badge)
![Spectre](https://img.shields.io/badge/Spectre-8B0000?style=for-the-badge)
![KiCad](https://img.shields.io/badge/KiCad-314CB0?style=for-the-badge\&logo=kicad\&logoColor=white)

### FPGA / Development Tools

![Vivado](https://img.shields.io/badge/Vivado-BB2200?style=for-the-badge)
![MATLAB](https://img.shields.io/badge/MATLAB-0076A8?style=for-the-badge)
![Simulink](https://img.shields.io/badge/Simulink-F2A900?style=for-the-badge)
![VS Code](https://img.shields.io/badge/VS_Code-007ACC?style=for-the-badge\&logo=visualstudiocode\&logoColor=white)

---

## 📌 Interests

* RTL Design & Verification
* AXI-based Peripheral Design
* FPGA-based Accelerator Architecture
* Processing-In-Memory Simulation
* Mixed-Signal Circuit Design
* Hardware-aware AI Model Optimization

---

## 🔗 Contact

<div align="center">

[![GitHub](https://img.shields.io/badge/GitHub-bjunverse26-181717?style=for-the-badge\&logo=github\&logoColor=white)](https://github.com/bjunverse26)
[![Velog](https://img.shields.io/badge/Velog-bjunverse_-20C997?style=for-the-badge\&logo=velog\&logoColor=white)](https://velog.io/@bjunverse_/posts)
[![Email](https://img.shields.io/badge/Email-bjunverse26%40gmail.com-D14836?style=for-the-badge\&logo=gmail\&logoColor=white)](mailto:bjunverse26@gmail.com)

</div>
