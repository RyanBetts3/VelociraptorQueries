# Velociraptor DFIR Artifacts

This repository contains custom Velociraptor artifacts developed for Digital Forensics and Incident Response (DFIR) operations. These artifacts are designed to assist with common triage, hunting, and threat detection tasks in Windows environments.

## 🔍 About

Velociraptor is a DFIR tool that enables scalable endpoint querying and response. Custom artifacts extend its functionality for your specific investigation needs. This collection focuses on:

- Early-stage ransomware detection
- Suspicious file and process behavior
- Lateral movement and credential theft detection
- Artifact extraction for triage

## 📁 Artifact List

| Artifact Name | Purpose |
|---------------|---------|
| `Custom.Windows.DetectRansomNoteFiles` | Scan for known ransomware note files across user directories |
| `Custom.Windows.MonitorLSASSAccess` | Detect suspicious access to LSASS memory |
| `Custom.Windows.FindEncodedPowerShell` | Identify PowerShell processes using base64-encoded commands |
| `Custom.Windows.SuspiciousCertutilUsage` | Locate misuse of certutil for downloading/decoding payloads |

## 🛠 Usage

1. Clone this repo or download individual `.yaml` files.
2. Import artifacts into Velociraptor via the GUI or CLI.
3. Run as part of a hunt, triage, or scheduled collection.
4. Review output in the Velociraptor interface or export as needed.