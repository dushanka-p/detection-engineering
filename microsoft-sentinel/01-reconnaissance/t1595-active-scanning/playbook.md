# Detection Playbook – <MITRE Technique ID> <Technique Name>

**MITRE ATT&CK Mapping:**

* **Tactic:** <Tactic Name>
* **Technique:** <MITRE Technique ID> – <Technique Name>
* **Link:** [MITRE ATT&CK <ID> ↗️](MITRE ATT&CK Link)

---

## 🎯 Playbook Goal

* Guide detection engineering tasks for <Technique Name>:

  * Building, validating, tuning, and documenting detection logic (KQL/Sentinel).

---

Requirement:
* Requires DeviceNetworkEvents enabled on endpoints.

---

## 🛠️ Detection Engineering Workflow

1. **Understand the Technique**

   * [ ] Review MITRE ATT&CK documentation and Atomic Red Team test(s).
   * [ ] Summarize what “good” and “malicious” looks like for this behavior.
   * [ ] Note typical log sources (e.g., SecurityEvent, DeviceNetworkEvents).

2. **Build Detection Logic**

   * [ ] Draft KQL query targeting the technique’s indicators.
   * [ ] Map query fields to Sentinel entity mappings (e.g., Account, Host, IP).
   * [ ] Save query as [`detection-rule.kql`](./detection-rule.kql).

3. **Simulate & Validate**

   * [ ] Use Atomic Red Team to simulate the technique in lab.
   * [ ] Confirm detection rule triggers as expected.
   * [ ] Investigate any false positives/negatives.

4. **Tune Detection**

   * [ ] Adjust query for accuracy and minimize noise.
   * [ ] Add exclusions (known-good behavior, service accounts, IT ranges).
   * [ ] Document all changes and rationale.

5. **Document Test Evidence**

   * [ ] Save screenshots of the simulation and detection in `artifacts/` (if collected).
   * [ ] Export example logs (if needed) for future reference.

6. **Review & Iterate**

   * [ ] Peer review detection logic (if possible).
   * [ ] Schedule periodic retest as technique or environment changes.

---

## 📋 Detection Quality Checklist

* [ ] MITRE technique reviewed and understood
* [ ] Detection logic mapped to correct log source
* [ ] Detection tested with ART
* [ ] False positives/negatives addressed
* [ ] Query fields mapped to Sentinel entities
* [ ] Documentation and artifacts updated

---

## 🧠 Notes & Future Improvements

* <Add detection gaps, improvement ideas, or threat landscape changes to monitor.>
* <Example: “Need to add coverage for new PowerShell obfuscation variants in future.”>

---

***This playbook is for detection engineering use only. All simulations and logic development are performed in an isolated lab environment.***

---
