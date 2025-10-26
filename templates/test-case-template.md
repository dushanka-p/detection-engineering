# Test Case – <MITRE Technique ID> <Technique Name>

**MITRE ATT&CK Mapping:**

* **Tactic:** <Tactic Name>
* **Technique:** <MITRE Technique ID> – <Technique Name>
* **Link:** [MITRE ATT&CK <ID> ↗️](MITRE ATT&CK Link)

---

## 🎯 Test Objective

* Simulate <short summary of technique/action> using **Atomic Red Team** in a controlled lab.
* Confirm detection logic in [`detection-rule.kql`](./detection-rule.kql) triggers as expected in Microsoft Sentinel.

---

## 📝 Test Steps

1. **Lab Prep**

   * [ ] Confirm lab VM(s) and Microsoft Sentinel workspace are online.
   * [ ] (Optional) Take snapshot/backup of VMs before testing.

2. **Run Atomic Red Team Test**

   * [ ] Identify relevant ART test:
     `<Atomic Test ID/Name – e.g., T1595.001 – Nmap Network Scanning>`
   * [ ] Execute ART test on target VM:

     ```
     Invoke-AtomicTest <TechniqueID> -TestNumbers <TestNumber> -GetPrereqs -ShowDetails
     Invoke-AtomicTest <TechniqueID> -TestNumbers <TestNumber> -Confirm
     ```

     *(Replace with the exact ART command you use)*
   * [ ] Record execution date/time.

3. **Detection Validation**

   * [ ] In Microsoft Sentinel, open Logs and run the [`detection-rule.kql`](./detection-rule.kql) query.
   * [ ] Confirm alert/flag for the ART activity.
   * [ ] If needed, tune detection logic and retest.

4. **Documentation**

   * [ ] Screenshot ART test execution and Sentinel alerts.
   * [ ] Export relevant logs (if needed).
   * [ ] Note issues, false positives, or recommendations.

---

## 🧩 Artifacts

| Type         | Filename/Path                | Description                 |
| ------------ | ---------------------------- | --------------------------- |
| Screenshot   | `artifacts/scan-result.png`  | ART test & alert screenshot |
| Log Export   | `artifacts/logs.csv`         | Sentinel logs (if exported) |
| Query Output | `artifacts/query-result.txt` | Output from KQL query       |

---

## 🧠 Notes & Observations

* <Add lessons learned, detection tuning, or real-world considerations here.>

---

***All ART simulations performed in a fully isolated lab environment. Never execute on production systems.***

---
