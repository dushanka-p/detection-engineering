# <MITRE Technique ID> – <Technique Name>

**MITRE ATT&CK Mapping:**

* **Tactic:** <Tactic Name>
* **Technique:** <MITRE Technique ID> – <Technique Name>
* **Link:** [MITRE ATT&CK <ID> ↗️](MITRE ATT&CK Link)

---

## 🧪 Atomic Red Team Simulation

This scenario simulates **<Short scenario description>** (e.g., <tool/method>). Detection logic is created and tested in **Microsoft Sentinel** using custom KQL.

> **Safety Notice:**
> All simulations are performed in an isolated lab. **Never run these techniques on production systems.**

---

## 📂 Folder Contents

| File / Folder        | Description                                    |
| -------------------- | ---------------------------------------------- |
| `detection-rule.kql` | Main KQL detection query for <Technique>.      |
| `test-case.md`       | Step-by-step test case and simulation details. |
| `playbook.md`        | SOC playbook for incident response & triage.   |
| `README.md`          | This documentation file.                       |

---

## 🎯 Objective

* Simulate and detect **<Technique/Action to be Detected>**.
* Document detection logic, test steps, and response workflow.

---

## ✅ Quick Start

1. **Review the KQL Detection Rule:**
   See [`detection-rule.kql`](./detection-rule.kql) for the core query logic.

2. **Run the Test Case:**
   Follow steps in [`test-case.md`](./test-case.md) to simulate and validate detection.

3. **SOC Playbook:**
   Use [`playbook.md`](./playbook.md) for incident triage and response.

---

## 🧠 Detection Engineering Notes

* All content is MITRE-mapped and manually tested.
* Artifacts (screenshots/logs) should be stored in a separate `/artifacts/` folder if generated.

---

***For educational and portfolio use only. All scenarios are run in an isolated lab environment.***

---
