# DFIR QuickTriage

DFIR QuickTriage is a lightweight Windows **Digital Forensics & Incident Response (DFIR) triage utility**
designed for fast, objective collection and prioritization of forensic artefacts.

The tool focuses on **technical signal extraction**, not attribution or malware classification.

---

## Features

- Automatic elevation to administrator
- Runtime process enumeration
- Process image path extraction
- SHA256 hashing of executable images
- Heuristic scoring of processes
- Flag-based prioritization
- CSV and TXT report generation
- Minimal runtime footprint
- Single portable executable

---

## Output Files

The tool generates the following files in the execution directory:

- `timeline_scored.csv` — full process timeline with heuristic scores
- `timeline_high.csv` — high-priority flagged entries only
- `timeline.txt` — plain-text timeline
- `report.html` — human-readable forensic summary

---

## Usage

Run the executable with administrative privileges:

```text
DFIR_QuickTriage.exe

If not launched as administrator, the tool will automatically relaunch itself with elevated privileges.

No installation is required.

Digital Signature

The release executable is digitally signed using a self-signed code signing certificate.

Because the certificate is not issued by a public Certificate Authority (CA),
Windows SmartScreen may display a warning on first execution.

This does not affect the integrity or functionality of the executable.

Intended Use

This tool is intended for defensive DFIR and triage purposes only.

It does not:

exploit systems

modify protected artefacts

bypass security mechanisms

perform attribution or malware verdicts

All output is neutral, technical data.

Limitations

Designed for rapid triage, not full forensic acquisition

Requires local administrative access

Self-signed certificate is not trusted by default Windows installations

License

MIT License




