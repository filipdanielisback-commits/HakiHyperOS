# HyperOS port feasibility research plan

The first objective is to determine whether a genuine port is technically and legally feasible. Do not begin by copying a random ROM or mixing files from unrelated devices.

## Phase 1 — Establish the target baseline

- Confirm the exact XT2135-2 variant and codename.
- Record Android version, build fingerprint, security patch, kernel version, and vendor interface from trusted device information.
- Identify the partition and boot-image layout from authoritative device-specific sources.
- Keep owner-provided values clearly labelled until independently checked.

**Deliverable:** a sourced device profile in [DEVICE_INFO.md](DEVICE_INFO.md).

## Phase 2 — Audit existing device support

- Review relevant device tree, common tree, and kernel repositories.
- Check whether sources match the target model and firmware generation.
- Record repository URLs, branches, licenses, last meaningful activity, and known limitations.
- Do not assume a repository is compatible merely because its name contains the codename.

**Deliverable:** a source audit with evidence and unresolved questions.

## Phase 3 — Identify a legitimate HyperOS base

- Establish which HyperOS release and Android base are actually available.
- Determine whether required framework and system components can be obtained and used lawfully.
- Record architecture, API level, framework dependencies, proprietary service dependencies, and vendor expectations.
- Do not upload proprietary firmware, vendor blobs, APKs, or extracted system components unless redistribution is explicitly permitted.

**Deliverable:** a donor-base compatibility report. If no suitable, lawful base exists, document that blocker rather than claiming a port is underway.

## Phase 4 — Compatibility assessment

Compare the donor requirements with the Moto G60 baseline:

- Android framework and API compatibility.
- Vendor interface and proprietary service dependencies.
- Kernel and device-specific hardware support.
- Graphics, display, audio, camera, sensors, radio, fingerprint, and power-management dependencies.
- Boot image and partition-layout requirements.

**Deliverable:** a compatibility matrix marking each item as verified, unknown, incompatible, or blocked.

## Phase 5 — Build planning

Only after the earlier phases show a plausible path:

- Define a reproducible build environment.
- Pin source revisions and document licenses.
- Keep generated output and private material out of Git.
- Add build scripts only when their inputs and outputs are understood.
- Document testing criteria before producing any experimental image.

## Safety and release policy

This repository is not a flashing guide. Do not test experimental images on a primary-use device. Any future device testing requires verified model-specific documentation, suitable recovery options, and an understanding of the risk of data loss or device failure.

Never describe a build as bootable, stable, or fully functional without reproducible test evidence.
