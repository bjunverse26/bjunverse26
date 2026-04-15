# Profile README

## 👋 About Me
- 디지털 회로 설계 / 검증 엔지니어를 목표로 공부하고 있습니다.

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
    - 하드웨어 소자의 Noise, Retention, ADC 오차 등 아날로그 특성 시뮬레이션
    - 하드웨어 제약 조건에 따른 모델의 Perplexity(PPL) 성능 분석
- [프로젝트 링크](https://github.com/bjunverse26/PIM_Framework)

### 3. Watch
- SystemVerilog 기반 FPGA 디지털 시계 RTL 설계
- 주요 성과:
    - `one_sec_gen`으로 입력 클럭 기반 1초 tick 생성
    - `tick_gen`을 재사용해 초/분/시 카운터를 모듈식으로 구성
    - `top_watch_v1`에서 직접 구현한 구조를 `top_watch_v2`에서 재사용 가능한 구조로 개선
    - `tb_one_sec_gen`, `tb_top_watch`로 분주기와 전체 시계 동작 검증
- [프로젝트 링크](https://github.com/bjunverse26/Watch)

## 🟦 기술 스택
### HDL / Verification
![Verilog](https://img.shields.io/badge/Verilog-808080?style=for-the-badge)
![SystemVerilog](https://img.shields.io/badge/SystemVerilog-1E90FF?style=for-the-badge)

### Software & AI Framework
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white)

### Tools
![Vivado](https://img.shields.io/badge/Vivado-BB2200?style=for-the-badge)
![VS Code](https://img.shields.io/badge/VS_Code-007ACC?style=for-the-badge&logo=visualstudiocode&logoColor=white)
![Virtuoso](https://img.shields.io/badge/Virtuoso-CC0000?style=for-the-badge&logo=cadence&logoColor=white)

## 📫 연락처 / Links
- GitHub: https://github.com/bjunverse26
- Velog: https://velog.io/@bjunverse_/posts
- Email: bjunverse26@gmail.com
