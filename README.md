<h1 align="center">Anton Vynohradov</h1>

<p align="center">
  <b>Embedded Systems Engineer · Founder of <a href="https://systemfromscratch.github.io/">SystemFromScratch®</a></b><br/>
  Reliable, secure, high-performance embedded systems built from scratch:<br/>
  from bare metal to Linux, from first schematic to certification.
</p>

<p align="center">
  <a href="https://systemfromscratch.github.io/"><img src="https://img.shields.io/badge/SystemFromScratch-Website-050b16?style=for-the-badge&logo=googlechrome&logoColor=2f8cff" alt="Website"/></a>
  <a href="mailto:avynohradov@systemfromscratch.com?subject=Project%20inquiry"><img src="https://img.shields.io/badge/Email-Get_in_touch-1d5fbf?style=for-the-badge&logo=maildotru&logoColor=white" alt="Email"/></a>
  <a href="https://www.linkedin.com/in/vynohradov"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
  <a href="https://github.com/SystemFromScratch"><img src="https://img.shields.io/badge/SystemFromScratch-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub organization"/></a>
  <a href="https://orcid.org/0009-0005-6965-0911"><img src="https://img.shields.io/badge/ORCID-A6CE39?style=for-the-badge&logo=orcid&logoColor=white" alt="ORCID"/></a>
</p>

---

## About

I help industrial IoT, automotive, robotics, medical and consumer electronics teams turn hardware into secure, maintainable products. One partner for firmware, platform software and compliance, from the first board on the bench to the product in the field.

📍 Based in **Poland**, working remotely worldwide.

## Services

| | Service | What you get |
| --- | --- | --- |
| 🔧 | **Embedded Software Development** | Bare-metal, RTOS and Linux application firmware in C/C++, including OTA, built for performance, reliability and long-term maintainability. |
| 🧩 | **BSP & Device Drivers** | Board support packages, bootloaders and low-level drivers for MCUs, SoCs, FPGAs and custom hardware, including Zephyr drivers and Linux kernel work. |
| 🐧 | **RTOS & Embedded Linux** | Porting, configuration, integration and reproducible builds for Zephyr, FreeRTOS and Embedded Linux (Yocto, Buildroot). |
| 🔌 | **Hardware Bring-up & Integration** | From schematic review through first boot, validation and production, including SoC FPGA and motor-control platforms (CAN, SPI, I²C). |
| 🔐 | **Cybersecurity & CRA Readiness** | Secure boot, firmware integrity, threat modelling and a secure development lifecycle that prepares connected products for the EU Cyber Resilience Act. |
| 📋 | **Compliance & Consulting** | MISRA C/C++, static analysis, code and architecture reviews, compliance roadmaps and ongoing technical advisory. |

## Why work with me

- **Hardware and software in one person.** I read schematics as fluently as source code.
- **Security and certification from day one.** MISRA and CRA requirements are designed in, not added at the end.
- **Code built to last.** Modular and documented, so it can be maintained for years.
- **Reproducible engineering.** Containerised builds and CI/CD on every project.
- **Transparent communication.** Startup agility with enterprise standards.

## Open-source libraries

My libraries show the standard I deliver to clients: code you can put in a safety- or security-relevant product and defend in an audit.

<p>
  <img src="https://img.shields.io/badge/MISRA_C:2012-0_violations-2ea44f?style=flat-square" alt="0 MISRA C:2012 violations"/>
  <img src="https://img.shields.io/badge/coverage-100%25_line_%26_branch-2ea44f?style=flat-square" alt="100% line and branch coverage"/>
  <img src="https://img.shields.io/badge/cross--checked-Python_twin-3776AB?style=flat-square&logo=python&logoColor=white" alt="Cross-checked against an independent Python implementation"/>
  <img src="https://img.shields.io/badge/C11-no_heap,_no_RTOS-1b3358?style=flat-square" alt="C11, no heap, no RTOS"/>
  <img src="https://img.shields.io/badge/static_analysis-Cppcheck_%C2%B7_CodeQL-1b3358?style=flat-square" alt="Cppcheck and CodeQL"/>
</p>

### Engineering standard

- ✅ **MISRA C:2012, zero violations.** Checked in CI on every pull request, with a documented deviation register instead of silent exceptions.
- ✅ **100 % line and branch coverage.** Enforced as a CI gate for every library (GoogleTest, pytest), so no untested code reaches a release.
- ✅ **Cross-checked against an independent Python twin.** A separate Python implementation verifies the C code end to end, catching errors that tests written from the same assumptions would miss.
- ✅ **Embedded-first design.** C11, no heap, no RTOS, no globals, no OS calls. Static memory only, with RAM and worst-case stack measured and published.
- ✅ **Static analysis on every change.** Cppcheck, CodeQL and format checks run in CI next to the tests and examples.
- ✅ **Portable by design.** The same code runs bare metal, under Zephyr or another RTOS, and on a PC, with a thin, hardware-agnostic integration layer.
- ✅ **Release-ready deliverables.** Every release ships as a versioned package with a static library, a MISRA report and a printable PDF user manual.

### Libraries

| Library | What it does | RAM | Stack (Cortex-M4) | Links |
| --- | --- | --- | --- | --- |
| [**Baton-C**](https://github.com/AntonVynohradov/Baton-C) `1.0.0` | Deterministic master/slave bus over a single-wire UART or RS-485. CRC-16, acknowledgements, retries and duplicate filtering give exactly-once, in-order delivery. | 1696 B / node | 280 B | [Docs](https://antonvynohradov.github.io/Baton-C/) · [Article](https://systemfromscratch-articles.github.io/Baton-C-One-wire-many-MCUs-no-lost-messages/) |
| [**ISOTP-C**](https://github.com/AntonVynohradov/isotp-c) | ISO-TP (ISO 15765-2) over CAN: segmentation, flow control and timeout detection, messages up to 4095 B. Bare metal, Zephyr, Linux SocketCAN. | 104 B / link + buffers | ≤ 120 B | [Docs](https://antonvynohradov.github.io/isotp-c/) |
| [**DXL2-C**](https://github.com/AntonVynohradov/DXL2-C) | ROBOTIS DYNAMIXEL Protocol 2.0 over UART, RS-485, USB or TCP. 10 public functions, reviewable in an afternoon. | ≈ 550 B / bus | ≤ 600 B | [Docs](https://antonvynohradov.github.io/DXL2-C/) |
| [**Stepper-C**](https://github.com/AntonVynohradov/Stepper-C) | Stepper motor control at 20 kHz PWM with PI current control, trapezoidal moves, up to 256 microsteps and same-period overcurrent/voltage protection. 6.8 KiB flash. | 336 B / motor | 184 B (PWM ISR) | [Docs](https://antonvynohradov.github.io/Stepper-C/) · [Article](https://systemfromscratch-articles.github.io/Stepper-C-Motor-Control-Library/) |

More on the [projects page](https://systemfromscratch.github.io/projects.html). Engineering write-ups, each with a repository that reproduces the numbers it quotes, are on the [articles page](https://systemfromscratch.github.io/articles.html).

## Tech stack

**Software & OS**

![C](https://img.shields.io/badge/C-A8B9CC?style=flat-square&logo=c&logoColor=black)
![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Zephyr](https://img.shields.io/badge/Zephyr_RTOS-AF52DE?style=flat-square&logo=zephyrproject&logoColor=white)
![FreeRTOS](https://img.shields.io/badge/FreeRTOS-5B9A30?style=flat-square)
![Embedded Linux](https://img.shields.io/badge/Embedded_Linux-FCC624?style=flat-square&logo=linux&logoColor=black)
![Yocto](https://img.shields.io/badge/Yocto-1E73BE?style=flat-square)
![Buildroot](https://img.shields.io/badge/Buildroot-333333?style=flat-square)

**Hardware & protocols**

![ARM Cortex-M](https://img.shields.io/badge/ARM_Cortex--M-0091BD?style=flat-square&logo=arm&logoColor=white)
![STM32](https://img.shields.io/badge/STM32-03234B?style=flat-square&logo=stmicroelectronics&logoColor=white)
![Microchip](https://img.shields.io/badge/Microchip-EE2223?style=flat-square&logo=microchiptechnology&logoColor=white)
![FPGA](https://img.shields.io/badge/SoC_FPGA-6d2c91?style=flat-square)
![RISC-V](https://img.shields.io/badge/RISC--V-283272?style=flat-square&logo=riscv&logoColor=white)
![CAN](https://img.shields.io/badge/CAN_/_ISO--TP-2a4a7a?style=flat-square)
![RS-485](https://img.shields.io/badge/RS--485-2a4a7a?style=flat-square)
![ROS 2](https://img.shields.io/badge/ROS_2-22314E?style=flat-square&logo=ros&logoColor=white)

**Tooling & quality**

![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/CI/CD-2088FF?style=flat-square&logo=githubactions&logoColor=white)
![MISRA](https://img.shields.io/badge/MISRA_C/C++-1b3358?style=flat-square)
![CRA](https://img.shields.io/badge/EU_CRA_readiness-003399?style=flat-square)

## Work with me

Building a connected product, bringing up new hardware, or preparing for the Cyber Resilience Act?
I can take it from the first board on the bench to a secure, maintainable product in the field.

📩 **[avynohradov@systemfromscratch.com](mailto:avynohradov@systemfromscratch.com?subject=Project%20inquiry)** · 🌐 **[systemfromscratch.github.io](https://systemfromscratch.github.io/)** · 💼 **[LinkedIn](https://www.linkedin.com/in/vynohradov)**

---

<p align="center"><sub><b>SystemFromScratch®</b> · Embedded systems built from scratch, from concept to certification.</sub></p>
