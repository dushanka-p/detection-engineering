# 🎯 Detection Engineering Portfolio

**Welcome!**  
This section showcases my production-ready detection rules, each mapped to [MITRE ATT&CK®](https://attack.mitre.org/) techniques for maximum clarity and real-world relevance.

---

## 🚦 Why MITRE ATT&CK Structure?

- **Industry Standard:**  
  All detection rules and analytic queries are organized by MITRE ATT&CK Tactic and Technique (e.g., `03-initial-access/t1078.001-default-accounts.kql`), mirroring how leading SOCs and detection engineering teams operate in production.

- **Clarity & Scalability:**  
  This approach makes it easy to find, review, and expand coverage for any stage of the attack lifecycle—whether it’s initial access, persistence, lateral movement, or exfiltration.

- **Red Team Alignment:**  
  Structuring detections this way ensures I’m always thinking like both an attacker and a defender, ready to simulate, detect, and respond to threats mapped to real adversary behaviors.

---

## 📚 What You'll Find Here

- **KQL, Sigma, and other production-ready detection queries** for Microsoft Sentinel, Defender, and other modern SIEM/EDR platforms
- **MITRE ATT&CK IDs and context** in every file and folder
- **Short descriptions, validation notes, and tuning tips** at the top of each query
- **Completely decoupled from lab/test tools:**  
  While all rules are validated using attack simulations (e.g., Atomic Red Team), the queries themselves are designed for real SOC/production use.

---

## 📁 Folder Structure Example


```markdown
detection-engineering/
├── 03-initial-access/
│   ├── t1078.001-default-accounts.kql
│   ├── t1566.001-phishing-excelmacro.kql
│   └── ...
├── 09-collection/
│   └── t1005-data-from-local-system.kql
├── README.md
```

- Each subfolder matches a **MITRE tactic** (“03-initial-access”), and each detection file matches a **MITRE technique**.
- This layout ensures instant traceability for blue teamers, threat hunters, and hiring managers.

---

## 🛡️ About Me

I’m passionate about building and testing real-world detections, mapping everything to MITRE ATT&CK, and delivering security engineering work that’s easy to scale and operationalize in any SOC.

---

> *Feel free to explore, borrow, or reach out for collaboration!*


---

