# bsp-rk3588

Boardcon RK3588 Board Support Package — 面向基于 Rockchip RK3588 芯片的嵌入式开发板和模块化计算机的 BSP 维护仓库。

[![Platform](https://img.shields.io/badge/platform-RK3588-orange)](https://www.rock-chips.com/a/en/products/RK35_Series/2024/0110/RK3588.html)
[![License](https://img.shields.io/badge/license-GPL--2.0-blue)](LICENSE)

---

## 简介

本仓库维护 Boardcon Embedded Design Limited 所有基于 RK3588 平台产品的板级支持包（BSP），涵盖以下核心组件：

- **U-Boot** — 引导加载程序（含 DDR 初始化、ATF 集成）
- **Linux Kernel** — Vendor 内核及 Mainline 主线跟踪
- **Yocto / Buildroot** — 构建系统配方和配置
- **Device Tree** — 板级设备树文件
- **固件 / 分区** — 分区布局、固件打包脚本

### 目标产品

| 产品 | 类型 | 关键规格 |
|------|------|----------|
| （待补充） | SBC / COM / DevKit | RK3588 + LPDDR4x/5 + eMMC |

---

## 仓库结构（规划中）



---

## 快速开始

> **仓库初始化中，以下为预期构建流程。**

### 环境需求

| 工具 | 版本 | 说明 |
|------|------|------|
| Ubuntu / Debian | 20.04 / 22.04 (x86_64) | 推荐构建系统 |
| Rockchip Linux SDK | 基于 linux-5.10-gen-rkr4 或更高 | Vendor 内核 |
| GCC Toolchain | aarch64-none-linux-gnu- (9.x / 10.x) | 交叉编译 |
| Python | 3.8+ | 固件打包脚本依赖 |

### 构建步骤（草案）



---

## 分支策略

| 分支 | 用途 |
|------|------|
|  | 主分支，稳定版本 |
|  | 开发分支，待验证 |
|  | 发布版本标签 |

---

## 贡献指南

欢迎社区贡献！请遵循以下流程：

1. **Fork** 本项目
2. 创建特性分支 ()
3. 提交更改并推送
4. 提交 **Pull Request**，附上清晰的修改说明

### 提交规范



### Issue 提交

提交 Issue 时请附上：
- 产品型号和硬件版本
- 内核版本 / 构建日期
- 复现步骤和日志（ / 串口输出）

---

## 关键依赖 & 上游

| 项目 | 仓库 | 说明 |
|------|------|------|
| Rockchip Linux Kernel | [rockchip-linux/kernel](https://github.com/rockchip-linux/kernel) | 官方 Vendor 内核 |
| U-Boot | [u-boot/u-boot](https://github.com/u-boot/u-boot) | 主线 U-Boot |
| Arm Trusted Firmware | [ARM-software/arm-trusted-firmware](https://github.com/ARM-software/arm-trusted-firmware) | ATF (BL31) |
| Armbian | [armbian/build](https://github.com/armbian/build) | 社区 Armbian 构建 |
| rkbin | [rockchip-linux/rkbin](https://github.com/rockchip-linux/rkbin) | Rockchip 闭源固件 |
| RKNN Toolkit | [airockchip/rknn-toolkit2](https://github.com/airockchip/rknn-toolkit2) | RK3588 NPU 工具链 |

---

## RK3588 技术要点

| 特性 | 说明 |
|------|------|
| **CPU** | 4xCortex-A76 @ 2.4GHz + 4xCortex-A55 @ 1.8GHz |
| **GPU** | Mali-G610 MP4, OpenGL ES 3.2 / Vulkan 1.2 |
| **NPU** | 6 TOPS (INT8), 支持 TensorFlow / PyTorch / ONNX |
| **显示** | 4xHDMI 2.1 / 2xDP 1.4 / 2xMIPI DSI, 8K@60fps |
| **视频** | 8K@60fps 解码 / 8K@30fps 编码 (H.265/H.264/VP9/AV1) |
| **存储** | eMMC 5.1 / SATA 3.0 / PCIe 3.0x4 / USB 3.1 |
| **网络** | 双千兆以太网 (GMAC) |
| **工艺** | 8nm LP (Samsung) |

---

## 社区资源

- [Rockchip Wiki](http://opensource.rock-chips.com/) — 官方开源文档
- [Rockchip Linux 开发者指南](https://rockchip-linux.github.io/)
- [Armbian RK3588 论坛](https://forum.armbian.com/forum/203-rockchip-35xx3288/)
- [RK3588 NPU 开发指南](https://github.com/airockchip/rknn-toolkit2)

---

## License

本仓库中的代码遵循其上游项目的原始许可证。Boardcon 贡献部分采用 [GPL-2.0](LICENSE)。

---

_维护方：Boardcon Embedded Design Limited | 最后更新：2026-06-10_
