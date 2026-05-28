# roboparty_firmware

面向 Roboparty 机器人（包括 RPO/Roboto 平台）的固件及板卡镜像构建系统仓库。

## 概述

本模块包含机器人嵌入式系统所需的固件组件和板卡镜像构建系统。

## 子模块

| 模块 | 说明 |
|------|------|
| [roboto_usb2can](./roboto_usb2can) | USB 转 CAN 适配器固件 - 提供主机与机器人 CAN 总线之间的通信接口 |
| [orangepi-build](./orangepi-build) | OrangePi 板卡镜像构建系统 - 为 RK 系列板卡编译定制 Linux 镜像 |
| [x5-rdk-gen](./x5-rdk-gen) | RP0 X5 镜像构建系统 - 为 X5 平台生成固件镜像 |

## 快速开始

```bash
# 克隆仓库（含子模块）
git clone --recursive https://github.com/Roboparty/roboparty_firmware.git

# 或克隆后初始化子模块
git submodule update --init --recursive
```

镜像文件都在每个子模块的 release 里面。

## 目录结构

```
roboparty_firmware/
├── roboto_usb2can/      # USB2CAN 固件源码
├── orangepi-build/      # OrangePi 构建系统
│   └── external/cache/sources/bms_daemon/  # BMS 守护进程（嵌套）
├── x5-rdk-gen/          # X5 RDK 生成器
├── readme.md            # 英文文档
└── readme_cn.md         # 中文文档
```

## 关联仓库

- **[rpo_hardware](https://github.com/Roboparty/rpo_hardware)** - 硬件设计文件
- **[roboparty_deploy](https://github.com/Roboparty/roboparty_deploy)** - ROS2 部署框架
- **[roboparty_train](https://github.com/Roboparty/roboparty_train)** - RL 训练环境
- **[rpo_description](https://github.com/Roboparty/rpo_description)** - URDF 模型文件

## 许可证

本项目采用 GNU 通用公共许可证第三版 (GPLv3) 授权。

## 贡献指南

请参阅主仓库 [roboto_origin](https://github.com/Roboparty/roboto_origin) 了解贡献指南。

## 说明

部分第三方或上游构建系统、固件组件会保留原始名称、许可证和目录结构。
除非同步更新并验证对应构建脚本，否则不建议直接重命名这些兼容路径。
