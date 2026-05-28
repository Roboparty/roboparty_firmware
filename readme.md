# roboparty_firmware

Firmware and board image build systems for Roboparty robots, including RPO/Roboto platforms.

## Overview

This module contains firmware components and board image build systems required for the robot's embedded systems.

## Submodules

| Module | Description |
|--------|-------------|
| [roboto_usb2can](./roboto_usb2can) | USB to CAN adapter firmware - provides communication interface between host computer and robot's CAN bus |
| [orangepi-build](./orangepi-build) | OrangePi board image build system - compiles custom Linux images for RK series boards |
| [x5-rdk-gen](./x5-rdk-gen) | RP0 X5 image build system - generates firmware images for X5 platforms |

## Quick Start

```bash
# Clone repository with submodules
git clone --recursive https://github.com/Roboparty/roboparty_firmware.git

# Or initialize submodules after cloning
git submodule update --init --recursive
```

## Directory Structure

```
roboparty_firmware/
├── roboto_usb2can/      # USB2CAN firmware source
├── orangepi-build/      # OrangePi build system
│   └── external/cache/sources/bms_daemon/  # BMS daemon (nested)
├── x5-rdk-gen/          # X5 RDK generator
├── readme.md            # This file
└── readme_cn.md         # Chinese documentation
```

## Related Repositories

- **[rpo_hardware](https://github.com/Roboparty/rpo_hardware)** - Hardware design files
- **[roboparty_deploy](https://github.com/Roboparty/roboparty_deploy)** - ROS2 deployment framework
- **[roboparty_train](https://github.com/Roboparty/roboparty_train)** - RL training environment
- **[rpo_description](https://github.com/Roboparty/rpo_description)** - URDF model files

## License

This project is licensed under the GNU General Public License Version 3 (GPLv3).

## Contributing

See the main [roboto_origin](https://github.com/Roboparty/roboto_origin) repository for contribution guidelines.

## Notes

Some vendored build systems and firmware components may keep their upstream names,
licenses, and directory layout. Those compatibility paths should not be renamed
unless the corresponding build scripts are updated and validated.
