# roboparty_firmware

Firmware and board image build systems for Roboparty robots, including RPO/Roboto platforms.

## Repository Structure

| Submodule | Description |
|:--|:--|
| [orangepi-build](./orangepi-build) | RK series board image build system |
| [x5-rdk-gen](./x5-rdk-gen) | RP0 X5 image build system |
| [roboto_usb2can](./roboto_usb2can) | USB to CAN adapter firmware |

## Quick Start

```bash
# Clone with submodules
git clone --recursive https://github.com/Roboparty/roboparty_firmware.git

# Or init submodules after clone
git submodule update --init --recursive
```

## Notes

Some vendored build systems and firmware components may keep their upstream names,
licenses, and directory layout. Those compatibility paths should not be renamed
unless the corresponding build scripts are updated and validated.
