# Windows Memory Forensics — Volatility & Volatility 3

**Author:** Pedro Gonçalves  
**Domain:** Digital Forensics & Incident Response (DFIR) | Windows Security | Malware Triage

## Overview

This project documents a hands-on Windows 11 memory-forensics laboratory using Volatility Workbench, classic Volatility and Volatility 3. It explores how volatile-memory evidence can help investigators examine process execution, potentially injected code, virtual memory, kernel artifacts, network connections and Windows Registry activity.

> **Evidence note:** The laboratory demonstrates investigative tooling and workflows. The supplied evidence does **not** establish a confirmed malware infection or rootkit. Findings are therefore presented as training observations rather than proven compromise.

## Objectives

- Understand forensic value and limitations of RAM images.
- Examine active and potentially hidden processes using PsList, PsScan, PsXView and Malfind.
- Inspect VAD regions and process memory mappings.
- Review drivers, modules, SSDT entries, callbacks, timers and thread artifacts.
- Investigate network socket artifacts with NetScan.
- Explore Windows Registry, file-system and user-activity artifacts.
- Practice defensible evidence handling and technical reporting.

## Technologies

| Area | Tools / artifacts |
| --- | --- |
| Memory forensics | Volatility Workbench, Volatility, Volatility 3 |
| Target | Windows 11 memory sample |
| Processes | PsList, PsScan, PsXView, Malfind, command lines |
| Virtual memory | Memmap, VadInfo, VadWalk, VadTree |
| Kernel | Modules, DriverScan, SSDT, timers, callbacks |
| Network | NetScan |
| Registry and files | HiveList, PrintKey, FileScan, DumpRegistry, MFT |

## Investigation workflow

1. Identify and preserve the memory-image evidence.
2. Load the sample into Volatility Workbench.
3. Enumerate processes and cross-check suspicious results.
4. Inspect VADs and memory regions for anomalies.
5. Review kernel structures and network artifacts.
6. Correlate Registry, file and activity evidence.
7. Record observations, limitations and conclusions.

## Technical report

[**Read the full illustrated technical report (PDF)**](./Windows_Memory_Forensics_Volatility3_Pedro_Goncalves.pdf)

The PDF includes an original conceptual diagram, explanations and selected original laboratory screenshots. It has been reformatted for portfolio presentation without institutional branding.

## Scope and ethics

This is a controlled cybersecurity training exercise. Screenshots and interpretations should not be used as proof of compromise without independent corroboration. Memory images can contain sensitive information; use only authorized evidence and review it before public release.

## Skills demonstrated

Digital forensics, incident-response methodology, Windows internals, process analysis, malware triage, kernel inspection, network artifact analysis, evidence documentation and security reporting.

---

**Pedro Gonçalves** | Cybersecurity & Digital Forensics Portfolio
