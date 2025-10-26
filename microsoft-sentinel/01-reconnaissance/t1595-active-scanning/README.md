# T1595 – Active Scanning

**MITRE ATT&CK Mapping:**

* **Tactic:** Reconnaissance
* **Technique:** T1595 – Active Scanning
* **Link:** [MITRE ATT&CK T1595 ↗️](https://attack.mitre.org/techniques/T1595/)

---

## 🧪 Atomic Red Team Simulation

This scenario simulates **Active Scanning** (e.g., Nmap) targeting a lab VM. Detection logic is created and tested in **Microsoft Sentinel** using custom KQL.

> **Safety Notice:**
> All simulations are performed in an isolated lab. **Never run active scanning on production systems.**

---

## 📂 Folder Contents

| File / Folder        | Description                                    |
| -------------------- | ---------------------------------------------- |
| `detection-rule.kql` | Main KQL detection query for T1595.            |
| `test-case.md`       | Step-by-step test case and simulation details. |
| `playbook.md`        | SOC playbook for incident response & triage.   |
| `README.md`          | This documentation file.                       |

---

## 🎯 Objective

* Simulate and detect **active network scanning** by an external actor.
* Document detection logic, test steps, and response workflow.

---

## ✅ Quick Start

1. **Review the KQL Detection Rule:**
   See [`detection-rule.kql`](./detection-rule.kql) for the core query logic.

2. **Run the Test Case:**
   Follow steps in [`test-case.md`](./test-case.md) to simulate scanning and validate alert firing.

3. **SOC Playbook:**
   Use [`playbook.md`](./playbook.md) for structured incident triage and response.

---

## 🧠 Detection Engineering Notes

* All content is MITRE-mapped and manually tested.
* Artifacts (screenshots/logs) should be stored in a separate `/artifacts/` folder if generated.

---

***For educational and portfolio use only. All scenarios are run in an isolated lab environment.***

---

