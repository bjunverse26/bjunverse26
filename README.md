# Beomjun Kim | Hardware Design Portfolio

**RTL Design · Verification · FPGA · Memory/Custom IC · Embedded Control**

회로와 시스템의 동작 원리를 이해하고, 요구 조건에 맞는 구조를 선택한 뒤 시뮬레이션·구현·측정으로 검증하는 하드웨어 엔지니어를 지향합니다.

## Focus

| 분야 | 경험 |
| --- | --- |
| RTL Design & Verification | Verilog/SystemVerilog, SVA, self-checking testbench, regression |
| FPGA & Digital System | 연산 가속기 데이터패스·제어·메모리 설계, Vivado implementation·timing 검증 |
| Memory & Custom IC | SRAM cell·macro, Virtuoso simulation·layout, DRC/LVS, MPW |
| SoC Interface & CDC | AXI4-Lite, UART, memory-mapped peripheral, asynchronous FIFO |
| Embedded Control | Register-level C, timer ISR, sensor·PWM interface, 실시간 폐루프 제어 |
| Modeling & Analysis | Python, C++, PyTorch, MATLAB/Simulink 기반 분석·검증 자동화 |

## Featured Projects

### 1. 9T Dual-Mode SRAM PUF and 256-bit SRAM Macro

졸업작품 팀 프로젝트에서 SRAM cell 구조와 특성 분석, cell·array layout, FPGA 기반 측정 환경을 담당했습니다.

- 6T·8T cell의 RSNM과 SNM mismatch를 비교하고, PUF mode와 Normal mode를 선택하는 9T cell 설계
- PUF mode의 SNM mismatch를 6T 대비 91.8% 높이면서 Normal mode의 RSNM 감소폭을 1.38%로 제한
- 16×16 macro DRC/LVS 통과 및 0.5 μm CMOS 2P3M MPW 제작 완료
- FPGA–UART–Python 기반 power cycling·순차 read·frame 검사 환경 구축

### 2. [1→8→8→1 Recursive SRCNN FPGA Accelerator](https://github.com/bjunverse26/Digital_System_Design)

4인 팀의 팀장으로 세 가지 SRCNN 가속기 중 1→8→8→1 Recursive 구조를 담당해 데이터패스·제어·메모리 RTL 7개 모듈을 설계하고 FPGA로 구현했습니다.

- 전체 MAC 연산의 80%가 집중된 Layer 2를 64개의 3×3 convolution PE에 병렬 매핑
- Sliding-window line buffer로 선택 논리를 단순화해 초기 대비 전체 설계 LUT 약 15% 감소
- Feature-map lifetime에 따른 buffer reuse로 중간 저장 요구량 5.76 Mbit에서 2.88 Mbit로 축소
- 제공된 모든 테스트 케이스에서 C++ golden reference와 비트 단위 일치 확인 및 100 MHz FPGA 시연 완료

### 3. [AXI4-Lite Slave](https://github.com/bjunverse26/AXI4_Lite) / [AXI4-UART](https://github.com/bjunverse26/AXI4_UART)

AXI4-Lite protocol과 memory-mapped peripheral을 RTL로 구현하고 directed testbench와 SVA로 검증했습니다.

- AW/W channel의 도착 순서와 read/write backpressure를 처리하는 32-bit AXI4-Lite slave 설계
- Register map, byte strobe, response channel과 invalid-address 동작 검증
- AXI register access로 제어하는 UART TX/RX, FIFO, 16× oversampling loopback 구현
- 기능 testbench와 protocol assertion을 분리한 self-checking 검증 환경 구성

### 4. [Asynchronous FIFO and CDC](https://github.com/bjunverse26/Async_FIFO)

서로 다른 clock domain 사이에서 데이터 순서와 무결성을 유지하는 CDC 구조를 설계했습니다.

- Gray-code pointer와 2-FF synchronizer 기반 dual-clock FIFO 구현
- Full/empty flag와 request/acknowledge handshake CDC 설계
- 비동기 write/read clock에서 queue scoreboard로 누락·중복·순서 오류 자동 검사

### 5. [1 kHz Mechatronics Motor Control](https://github.com/bjunverse26/Mechatronics)

TI C6701 DSP에서 센서 입력, 상태 판단, 제어 연산과 PWM 출력을 1 kHz timer ISR로 연결했습니다.

- DC motor PID·trajectory tracking, STEP motor velocity profile, BLDC 6-step commutation 구현
- Inverted pendulum의 PUMP·COAST·Balancing 상태 전이와 각도 PD·cart 위치 P 제어 통합
- 반복 실물 시험에서 약 1~2초 직립을 확인하고, 이후 cart drift를 자세 안정화와 중심 복귀가 결합된 문제로 분석

### 6. [Llama 2 7B Analog PIM Evaluation Framework](https://github.com/bjunverse26/PIM_Framework)

연구실 공동 개발에서 Llama 추론에 Analog PIM의 기능 모델을 연결하고, 하드웨어 조건에 따른 모델 품질을 PPL로 평가했습니다.

- SmoothQuant W8A8 Linear projection과 KV-cache 연동 Attention의 PIM 연산 경로 분리
- `QKᵀ`와 `P·V`에 SubArray 부분합, conductance, retention, noise와 ADC 모델 연결
- WikiText-2 PPL 평가 흐름과 반복 실험을 위한 Python 기반 시뮬레이션 구성

## Tools

| 구분 | 기술 |
| --- | --- |
| HDL & Verification | Verilog, SystemVerilog, SVA |
| FPGA & EDA | Vivado |
| Circuit & Layout | Cadence Virtuoso, KiCad |
| Embedded & Software | C, C++, Python |
| Board & Interface | Arty S7-25T, UART |
| Modeling | PyTorch, MATLAB, Simulink |
| Development | Linux, Git, GitHub |

## Direction

셀과 RTL 설계를 chip 제작, FPGA 구현, board-level 측정 환경으로 연결하고, 반복 검증은 코드로 자동화하는 역량을 쌓고 있습니다.
