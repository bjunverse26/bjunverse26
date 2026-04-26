# Profile README

## 👋 About Me
- 디지털 회로부터 mixed-signal/analog 회로까지 확장 가능한 하드웨어 설계 역량을 쌓고 있습니다.

## 🚀 핵심 프로젝트
### 1. AXI4-Lite / AXI4-UART
- AXI4-Lite 기본 slave 구조를 먼저 구현하고, 이를 기반으로 UART Core를 제어하는 AXI4-UART peripheral까지 확장
- 주요 성과:
    - AXI4-Lite `AW->W`, `W->AW`, same-cycle write transaction 처리
    - Testbench와 SVA를 분리한 구조로 protocol assertion 및 coverage 검증
    - AXI4-UART에서 `CTRL`, `STATUS`, `TXDATA`, `RXDATA` 기반 register map 구현
    - UART loopback, invalid access, zero strobe, backpressure scenario 검증
- [AXI4-Lite 프로젝트 링크](https://github.com/bjunverse26/AXI4_Lite)
- [AXI4-UART 프로젝트 링크](https://github.com/bjunverse26/AXI4_UART)

### 2. PIM-Quant-Sim (PIM_Framework)
- Llama 모델 대상 SmoothQuant 및 Bit-slicing 연산 모델링
- 주요 성과:
    - 하드웨어 비이상성 Noise, Retention, ADC 오차 등 아날로그 특성 시뮬레이션
    - 하드웨어 제약 조건에 따른 모델의 Perplexity(PPL) 성능 분석
- [프로젝트 링크](https://github.com/bjunverse26/PIM_Framework)

### 3. Mechatronics
- 학부 Mechatronics 과정에서 센서, 구동기, 제어 로직을 단계적으로 실습 중
- 현재 진행 내용:
    - DC 모터 구동 및 기본 제어 실습
    - 마이크로컨트롤러 기반 입출력 제어 흐름 학습
    - 하드웨어 동작을 고려한 제어 구조 이해
- 향후 학습 예정:
    - Stepping motor 및 BLDC motor 제어 실습
    - 센서 피드백을 활용한 제어 시스템 구현
    - 최종 자율 프로젝트를 통한 메카트로닉스 통합 설계
- [프로젝트 링크](https://github.com/bjunverse26/Mechatronics)

### 4. Digital System Design
- 디지털시스템설계 수업을 통해 FPGA 기반 RTL 설계와 가속기 구조를 단계적으로 학습
- 주요 성과:
    - Vivado 기반 프로젝트 생성, RTL 작성, Testbench Simulation 흐름 정리
    - MAC, adder tree, pipelined adder tree 등 기본 연산 블록 설계
    - BRAM, LUTRAM, URAM, DSP macro 등 FPGA 자원 활용 실습
    - Processing Element(PE), 1D/2D convolution, multi-channel 데이터 처리 구조 구현
    - 최종 Super Resolution 가속기 설계를 위한 사전 구조 학습
- [프로젝트 링크](https://github.com/bjunverse26/Digital_System_Design)

## 🧰 기술 스택
### HDL / Verification
![Verilog](https://img.shields.io/badge/Verilog-808080?style=for-the-badge)
![SystemVerilog](https://img.shields.io/badge/SystemVerilog-1E90FF?style=for-the-badge)

### Software & AI Framework
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white)

### Circuit / EDA Tools
![Virtuoso](https://img.shields.io/badge/Cadence_Virtuoso-CC0000?style=for-the-badge&logo=cadence&logoColor=white)
![LTspice](https://img.shields.io/badge/LTspice-900028?style=for-the-badge)
![HSPICE](https://img.shields.io/badge/HSPICE-4B4B4B?style=for-the-badge)
![Spectre](https://img.shields.io/badge/Spectre-8B0000?style=for-the-badge)
![KiCad](https://img.shields.io/badge/KiCad-314CB0?style=for-the-badge&logo=kicad&logoColor=white)

### FPGA / Development Tools
![Vivado](https://img.shields.io/badge/Vivado-BB2200?style=for-the-badge)
![MATLAB](https://img.shields.io/badge/MATLAB-0076A8?style=for-the-badge)
![Simulink](https://img.shields.io/badge/Simulink-F2A900?style=for-the-badge)
![VS Code](https://img.shields.io/badge/VS_Code-007ACC?style=for-the-badge&logo=visualstudiocode&logoColor=white)

## 🔗 연락처 / Links
- GitHub: https://github.com/bjunverse26
- Velog: https://velog.io/@bjunverse_/posts
- Email: bjunverse26@gmail.com
