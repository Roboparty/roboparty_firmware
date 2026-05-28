# roboparty_firmware

面向 Roboparty 机器人（包括 RPO/Roboto 平台）的固件及板卡镜像构建系统仓库。

## 仓库结构

| 子模块 | 说明 |
|:--|:--|
| [orangepi-build](./orangepi-build) | RK 系列板卡镜像编译系统 |
| [x5-rdk-gen](./x5-rdk-gen) | RP0 X5 镜像编译系统 |
| [roboto_usb2can](./roboto_usb2can) | USB 转 CAN 适配器固件 |

## 快速开始

```bash
# 克隆仓库（含子模块）
git clone --recursive https://github.com/Roboparty/roboparty_firmware.git

# 或克隆后再初始化子模块
git submodule update --init --recursive
```

镜像文件都在每个子模块的release里面

## 说明

部分第三方或上游构建系统、固件组件会保留原始名称、许可证和目录结构。
除非同步更新并验证对应构建脚本，否则不建议直接重命名这些兼容路径。
