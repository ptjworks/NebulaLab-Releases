<div align="center">

<img src="./assets/logo.png" alt="Nebula Lab logo" width="92" />

# Nebula Lab

**A Windows desktop workstation for scientific data preparation, batch execution, and Origin-ready export**

From raw experimental files to plot-ready datasets, Nebula Lab keeps import, grouping, processing, batch reuse, and export in one workflow, alongside sample and recipe records and a data center that connects to your lab's own server.

[🇨🇳 简体中文](./README.md) · [🇺🇸 English](./README_EN.md)

[![Latest Release](https://img.shields.io/github/v/release/ptjworks/NebulaLab-Releases?display_name=tag&sort=semver&style=for-the-badge&color=2e4c70)](https://github.com/ptjworks/NebulaLab-Releases/releases/latest)
[![Platform](https://img.shields.io/badge/Platform-Windows%2010%20%7C%2011%20x64-0A66C2?style=for-the-badge&logo=windows)](https://github.com/ptjworks/NebulaLab-Releases/releases/latest)
[![Channels](https://img.shields.io/badge/Channels-Stable%20%7C%20Beta-C97A1A?style=for-the-badge)](https://github.com/ptjworks/NebulaLab-Releases/releases)

[**📥 Download Stable Release**](https://github.com/ptjworks/NebulaLab-Releases/releases/latest) &nbsp;&nbsp;•&nbsp;&nbsp; [**📄 View Release History**](https://github.com/ptjworks/NebulaLab-Releases/releases) &nbsp;&nbsp;•&nbsp;&nbsp; [**📖 Documentation**](https://nebulalab.app/)

</div>

> **What Nebula Lab is for:** a stable, repeatable workflow for group-level data and multi-plot experimental series, reducing repetitive manual cleanup before handoff to Origin or other plotting tools.

## Workflow Overview

| Import | Group | Process | Batch Reuse | Preview | Export |
| :--- | :--- | :--- | :--- | :--- | :--- |
| `.csv` `.txt` `.xlsx` `.xls` `.dat` `.xy` `.asc` | Merge files into one group or split them into several | Crop, smooth, baseline correction, normalize | Tune the workflow on one sample, then replay it from raw data across the group | Preview each step on real samples | Origin workbook and graph, CSV, PNG / JPG / SVG, Nebula project files |

## Core Capabilities

| Capability | Description |
| :--- | :--- |
| Preprocessing First | Standardize data quality and structure before formal plotting to reduce downstream rework. |
| Group-Level Reuse | Apply a workflow validated on one sample to its whole group; save the steps, parameters, axis mapping, and plot defaults to reuse on similar data. |
| Independent Branch Control | Split an anomalous sample into its own workflow and adjust its steps without affecting the rest of the group. |
| Handoff to Origin | Send selected sample groups to Origin with Origin graph templates and themes (requires Origin installed on the same computer). |
| Plugins and Community | Install official or community plugins from the plugin store; browse and publish shared workflows, Origin templates, themes, and research scripts. |
| Samples and Recipes | Sample management brings together overview, appearance, tests and characterization, attachments, and history, with report generation; the recipe library keeps versions with diffs, and the materials library supports PubChem lookup. |
| Lab Data Center | Once connected to your lab's server, upload sample records, search across samples, tests, and metrics, and share per sample; administrators manage members, devices, and the audit log in lab management. Some data center features are still being validated; see each release's notes. |
| Local First | Runs as a standalone Windows application with experimental data stored on your computer; the data center uses your lab's own server. |

## Getting Started

1. Download `NebulaLab-<version>-windows-x64-setup.exe` from the [Releases page](https://github.com/ptjworks/NebulaLab-Releases/releases/latest) and run the installer.
2. Import instrument files and check the encoding, skipped lines, header row, and sheets in the import settings, then organize them into sample groups.
3. Add processing steps such as crop, smoothing, baseline correction, and normalization on one sample, previewing the result at each step.
4. Apply the same steps to the whole group, and save them as a workflow to reuse on similar data.
5. Export the prepared groups to Origin, or export CSV, images, and Nebula project files.

> For accounts, sign-in, and licensing, follow the in-app prompts and the [documentation site](https://nebulalab.app/).

## Download and Installation

> Supported systems: Windows 10 / Windows 11 (x64)

| Channel | Package | Description |
| :--- | :--- | :--- |
| Stable | `NebulaLab-<version>-windows-x64-setup.exe` | Releases marked Latest; recommended for everyday work. |
| Beta | `NebulaLabBeta-<version>-windows-x64-setup.exe` | Releases marked Pre-release, for testers who want to try new features early; keep using the stable release for important work. Beta and stable are isolated from each other and can be installed side by side on the same computer. |

- Since 0.8.8, only the `setup.exe` installer is published; there is no `.msi` package.
- `.sig` and `latest.json` are the signature and manifest files used by in-app updates and can be ignored for manual installation. The release named `beta-channel` only holds the Beta update manifest and contains no installer.
- The installer is not code-signed yet, so your browser or Windows SmartScreen may show a warning; the [user manual](https://nebulalab.app/manual/) (in Chinese) explains how to proceed.

## Updates

- Stable and Beta each receive updates from their own channel. When a new version is found, the app asks for confirmation first and then shows download and installation progress.
- Each release's notes list what changed, data compatibility notes, and known limitations; read them before upgrading.

## Documentation and Feedback

- Documentation: [nebulalab.app](https://nebulalab.app/) (user manual and tutorials)
- Bug reports and feature requests: [Issues](https://github.com/ptjworks/NebulaLab-Releases/issues); choose the Bug Report or Feature Request template.
- Before attaching sample data, logs, or screenshots, remove unpublished research data and personal information.
