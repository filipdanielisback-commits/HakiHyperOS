# HakiHyperOS

**An experimental genuine Xiaomi HyperOS porting research project for the Motorola Moto G60 (XT2135-2 / hanoip).**

> **Status: Research only.** There is currently no verified bootable HakiHyperOS build. This repository does not contain a ROM, installer, or claim of successful HyperOS 4 compatibility.

## Project goal

Investigate whether genuine Xiaomi HyperOS components and framework can be adapted to the Moto G60, while preserving the device-specific support required for its hardware. The goal is not to create an Android theme or a HyperOS look-alike.

A genuine port would require substantial compatibility work across the Android framework, proprietary Xiaomi components, device configuration, kernel, vendor interface, and hardware-specific services. Feasibility has not yet been established.

## Target device

| Field | Current information |
|---|---|
| Device | Motorola Moto G60 |
| Model | XT2135-2 |
| Device codename | hanoip (to be confirmed against source/device data) |
| RAM | 6 GB (owner-reported) |
| Current firmware | S2RIS32.32-20-9-9-2-3 (owner-reported) |
| SoC | Qualcomm Snapdragon 732G (reference specification) |
| GPU | Qualcomm Adreno 618 (reference specification) |

See [docs/DEVICE_INFO.md](docs/DEVICE_INFO.md) for confidence levels and sources.

## Repository contents

- `.gitignore` — excludes generated build output, local configuration, and private/proprietary downloads.
- `docs/DEVICE_INFO.md` — target-device facts and items that still need verification.
- `docs/PROJECT_STATUS.md` — honest status and milestones.
- `docs/RESEARCH_PLAN.md` — staged feasibility and compatibility research.

## Principles

1. **Authenticity:** do not label a themed or AOSP-based build as genuine HyperOS.
2. **Evidence first:** record sources, versions, and test results; distinguish verified facts from assumptions.
3. **Respect licensing:** preserve upstream licenses and notices. Do not publish proprietary firmware, vendor blobs, or Xiaomi components unless redistribution is explicitly permitted.
4. **Device safety:** do not treat experimental images as safe for daily use. Any future testing must use verified device-specific instructions and appropriate recovery options.
5. **No unsupported claims:** boot status, working hardware, and compatibility are only reported after reproducible tests.

## Current status

The repository is at the documentation and feasibility-research stage. No source port, build system, or flashable image has been produced here.

See [docs/PROJECT_STATUS.md](docs/PROJECT_STATUS.md) and [docs/RESEARCH_PLAN.md](docs/RESEARCH_PLAN.md).

## Disclaimer

HakiHyperOS is an independent community research project and is not affiliated with, endorsed by, or sponsored by Xiaomi, Motorola, Lenovo, or Qualcomm. Product names and trademarks belong to their respective owners.
