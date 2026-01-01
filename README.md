
# Fire-Gecko UWB Antenna (火壁虎-超宽带穿墙雷达天线)

[![Status](https://img.shields.io/badge/Status-Fabrication-blue)](https://github.com/YourUsername/Fire-Gecko-Antenna)
[![Frequency](https://img.shields.io/badge/Frequency-1.2GHz-green)]()
[![Bandwidth](https://img.shields.io/badge/Bandwidth-0.9~1.8GHz-orange)]()

[English Version](#english-introduction) | [中文介绍](#chinese-introduction)

---

<a name="english-introduction"></a>

## 🦎 English Introduction

### 🎯 Project Context

This project is the RF front-end subsystem for the **Fire-Gecko Through-Wall Radar**.
It is designed for post-disaster rescue and aims to detect vital signs (heartbeat/respiration) of stationary targets behind walls using SFCW radar technology.

### 🧬 Design Highlights

* **Architecture**: Teardrop Dipole with Resistive Loading.
* **Core Frequency**: 1.2 GHz (optimized for wall penetration).
* **Innovation**: Uses a **12Ω resistor** to dampen the high-Q resonance, achieving a flat UWB response (0.9-1.8 GHz) suitable for SFCW transmission.
* **Performance**: **S11 < -15 dB** @ 1.2 GHz, **Gain 3.62 dBi**.

### 📂 Repository Structure

* `models/`: HFSS simulation files (`.aedt`) and DXF fabrication files.
* `docs/`: **[Engineering Log](docs/Engineering_Log.md)** (Detailed design history & failure analysis).
* `hardware/`: Gerber files for PCB manufacturing.

*(See detailed design process and simulation plots in the Engineering Log)*

---

<a name="chinese-introduction"></a>

## 🦎 中文介绍 (Chinese Introduction)

### 🎯 项目背景

本项目是 **Fire-Gecko (火壁虎) 穿墙生命探测雷达** 的天线子系统。
针对废墟搜救场景，我们需要一只“穿墙的眼睛”。本设计旨在提供一个高穿透力 (1.2 GHz) 且具有高距离分辨率 (UWB) 的定向天线方案。

### 🧬 技术亮点

* **架构**: 电阻加载式水滴形偶极子 (Resistively Loaded Teardrop Dipole)。
* **核心指标**: 中心频率 **1.2 GHz**，带宽覆盖 **0.9 - 1.8 GHz**。
* **设计突破**: 针对早期版本“高Q值窄带谐振”的问题，创新性地引入 **12Ω 并联电阻**，成功将尖锐的谐振峰压平，实现了良好的超宽带匹配。
* **最终性能**: 反射系数 S11 低至 **-15 dB**，增益 **3.62 dBi**，具有优异的单向辐射特性。

### 📂 目录说明

* `models/`: HFSS 仿真源文件及 DXF 结构图。
* `docs/`: **[工程设计日志](docs/Engineering_Log.md)** (包含从 V1 失败到 V3 成功的完整复盘记录与波形图)。
* `hardware/`: PCB 打样制造文件 (Gerber)。

---

**Maintainer**: Chief Architect, Fire-Gecko Team
