# Atom01 固件

Atom01 系列固件及构建系统仓库。

## 仓库结构

| 子模块 | 说明 |
|:--|:--|
| [orangepi-build](./orangepi-build) | RK 系列板卡镜像编译系统 |
| [x5-rdk-gen](./x5-rdk-gen) | RP0 X5 镜像编译系统 |
| [roboto_usb2can](./roboto_usb2can) | USB 转 CAN 适配器固件 |

## 快速开始

```bash
# 克隆仓库（含子模块）
git clone --recursive https://github.com/wentywenty/atom01_firmware.git

# 或克隆后再初始化子模块
git submodule update --init --recursive
```

镜像文件都在每个子模块的release里面
