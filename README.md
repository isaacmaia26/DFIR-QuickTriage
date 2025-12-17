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
