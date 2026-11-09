<h1 align="center">Anton Vynohradov</h1>

<p align="center">
  <b>Embedded Systems Engineer · Founder of <a href="https://SystemFromScratch.com/">SystemFromScratch®</a></b><br/>
  Firmware and embedded Linux for connected products:<br/>
  secure, MISRA-compliant and ready for the EU Cyber Resilience Act.
</p>

<p align="center">
  <a href="https://SystemFromScratch.com/"><img src="https://img.shields.io/badge/SystemFromScratch-Website-050b16?style=for-the-badge&logo=googlechrome&logoColor=2f8cff" alt="Website"/></a>
  <a href="mailto:contact@systemfromscratch.com?subject=Project%20inquiry"><img src="https://img.shields.io/badge/Email-Get_in_touch-1d5fbf?style=for-the-badge" alt="Email"/></a>
  <a href="https://www.linkedin.com/in/vynohradov"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
  <a href="https://github.com/SystemFromScratch"><img src="https://img.shields.io/badge/SystemFromScratch-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub organization"/></a>
</p>

---

## About

I founded **SystemFromScratch®** to help industrial IoT, automotive, robotics, medical and consumer electronics teams turn hardware into secure, maintainable products.

I design and write the software: firmware, drivers, RTOS and embedded Linux, security and compliance. For hardware design I work with experienced partner engineers, so you get one point of contact from the first board on the bench to the product in the field.

📍 Based in **Poland**, working remotely worldwide.

## 🔐 Preparing for the Cyber Resilience Act?

The CRA's vulnerability reporting obligations have applied since **11 September 2026**. The full requirements apply from **11 December 2027**. If you sell connected products in the EU, your firmware has to be ready by then.

I can review your current firmware, show you where the gaps are and help you close them. That covers secure boot, firmware integrity, threat modelling and a secure development lifecycle you can document.

## Services

| | Service | What you get |
| --- | --- | --- |
| 🔧 | **Embedded Software Development** | Bare-metal, RTOS and Linux application firmware in C/C++, including OTA, built for performance, reliability and long-term maintainability. |
| 🧩 | **BSP & Device Drivers** | Board support packages, bootloaders and low-level drivers for MCUs, SoCs, FPGAs and custom hardware, including Zephyr drivers and Linux kernel work. |
| 🐧 | **RTOS & Embedded Linux** | Porting, configuration, integration and reproducible builds for Zephyr, FreeRTOS and Embedded Linux (Yocto, Buildroot). |
| 🔌 | **Hardware Bring-up & Integration** | Firmware side of first boot, validation and production, including SoC FPGA and motor-control platforms (CAN, SPI, I²C). Hardware design and schematic work through trusted partners. |
| 🔐 | **Cybersecurity & CRA Readiness** | Secure boot, firmware integrity, threat modelling and a secure development lifecycle that prepares connected products for the EU Cyber Resilience Act. |
| 📋 | **Compliance & Consulting** | MISRA C/C++, static analysis, code and architecture reviews, compliance roadmaps and ongoing technical advisory. |

## Why work with me

- **One partner, the full product.** I lead the software and coordinate hardware specialists, so you don't have to manage separate vendors.
- **Security and compliance from day one.** MISRA and CRA requirements are designed in, not added at the end.
- **Code built to last.** Modular and documented, so your team can maintain it for years.
- **Reproducible engineering.** Containerised builds and CI/CD on every project.
- **Evidence, not promises.** My open-source libraries below show the standard you get, with public reports and measured numbers.

**How we can start:** a short call about your product, or a fixed-scope code, MISRA or CRA review of your existing firmware.
📩 [contact@systemfromscratch.com](mailto:contact@systemfromscratch.com?subject=Project%20inquiry)

## Open-source libraries

My libraries show the standard I deliver to clients: code you can put in a safety- or security-relevant product and defend in an audit.

<p>
  <img src="https://img.shields.io/badge/MISRA_C:2012-0_violations-2ea44f?style=flat-square" alt="0 MISRA C:2012 violations"/>
  <img src="https://img.shields.io/badge/coverage-100%25_line_%26_branch-2ea44f?style=flat-square" alt="100% line and branch coverage"/>
  <img src="https://img.shields.io/badge/cross--checked-Python_twin-3776AB?style=flat-square&logo=python&logoColor=white" alt="Cross-checked against an independent Python implementation"/>
  <img src="https://img.shields.io/badge/C11-no_heap,_no_RTOS-1b3358?style=flat-square" alt="C11, no heap, no RTOS"/>
  <img src="https://img.shields.io/badge/static_analysis-Cppcheck_%C2%B7_CodeQL-1b3358?style=flat-square" alt="Cppcheck and CodeQL"/>
</p>

What this means for your product:

- ✅ **Audit-ready.** Every release ships with a static library, a MISRA report and a printable PDF user manual.
- ✅ **Verified twice.** 100 % line and branch coverage, plus an independent Python implementation that checks the C code end to end.
- ✅ **Fits small MCUs.** Static memory only, with RAM and worst-case stack measured and published.
- ✅ **Portable.** The same code runs bare metal, under Zephyr or another RTOS, and on a PC.

| Library | What it does | RAM | Stack (Cortex-M4) | Links |
| --- | --- | --- | --- | --- |
| [**Baton-C**](https://github.com/AntonVynohradov/Baton-C) `1.0.0` | Deterministic master/slave bus over a single-wire UART or RS-485. CRC-16, acknowledgements, retries and duplicate filtering give exactly-once, in-order delivery. | 1696 B / node | 280 B | [Docs](https://antonvynohradov.github.io/Baton-C/) · [Article](https://systemfromscratch-articles.github.io/Baton-C-One-wire-many-MCUs-no-lost-messages/) |
| [**ISOTP-C**](https://github.com/AntonVynohradov/isotp-c) `2.0.1` | ISO-TP (ISO 15765-2) over CAN: segmentation, flow control and timeout detection, messages up to 4095 B. Bare metal, Zephyr, Linux SocketCAN. | 104 B / link + buffers | ≤ 120 B | [Docs](https://antonvynohradov.github.io/isotp-c/) |
| [**DXL2-C**](https://github.com/AntonVynohradov/DXL2-C) `1.0.0` | ROBOTIS DYNAMIXEL Protocol 2.0 over UART, RS-485, USB or TCP. 10 public functions, reviewable in an afternoon. | ≈ 550 B / bus | ≤ 600 B | [Docs](https://antonvynohradov.github.io/DXL2-C/) |
| [**Stepper-C**](https://github.com/AntonVynohradov/Stepper-C) `1.2.0` | Stepper motor control at 20 kHz PWM with PI current control, trapezoidal moves, up to 256 microsteps, sensorless stall detection and same-period overcurrent/voltage protection. | 336 B / motor | 184 B (PWM ISR) | [Docs](https://antonvynohradov.github.io/Stepper-C/) · [Article](https://systemfromscratch-articles.github.io/Stepper-C-Motor-Control-Library/) |

**Models and tools behind the libraries**

- [**Stepper-Lab**](https://github.com/AntonVynohradov/Stepper-Lab): Scilab/Xcos model of a hybrid stepper motor. Stepper-C is developed and tested against it before it runs on hardware.
- [**DYNAMIXEL X430 emulator**](https://github.com/AntonVynohradov/DYNAMIXEL-X430-Control-Table-Emulator): your firmware drives any motor, and DynamixelSDK, DYNAMIXEL Wizard and ROS 2 see a genuine X430.

More on the [projects page](https://SystemFromScratch.com/projects.html). Engineering write-ups, each with a repository that reproduces the numbers it quotes, are on the [articles page](https://SystemFromScratch.com/articles.html).

<details>
<summary><b>Tech stack</b></summary>
<br/>

**Software & OS:** C · C++ · Python · Zephyr RTOS · FreeRTOS · Embedded Linux · Yocto · Buildroot

**Platforms & protocols:** ARM Cortex-M · STM32 · Microchip · SoC FPGA · RISC-V · CAN / ISO-TP · RS-485 · ROS 2

**Tooling & quality:** Docker · Git · GitHub Actions CI/CD · MISRA C/C++ · Cppcheck · CodeQL · EU CRA readiness

</details>

## Work with me

Building a connected product, bringing up a new board, or preparing for the Cyber Resilience Act?
Tell me about your product, timeline and constraints, and I will reply with a proposal for the first step.

📩 **[contact@systemfromscratch.com](mailto:contact@systemfromscratch.com?subject=Project%20inquiry)** · 🌐 **[SystemFromScratch.com](https://SystemFromScratch.com/)** · 💼 **[LinkedIn](https://www.linkedin.com/in/vynohradov)**

---

<p align="center"><sub><b>SystemFromScratch®</b> · Embedded systems built from scratch, from concept to certification-ready product. · <a href="https://orcid.org/0009-0005-6965-0911">ORCID</a></sub></p>
