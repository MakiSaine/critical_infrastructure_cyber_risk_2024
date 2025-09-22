# ICS and Cloud Security Reflection 2024

This repository documents a reflection on cybersecurity risks in industrial control systems (ICS) and cloud-connected SCADA solutions, using the SunGrow case as a study.  
The work is based on an exam scenario, but it has been expanded and restructured into a professional write-up to share insights and recommended mitigations for real-world systems.

---

## Problem Statement

Modern energy infrastructure is increasingly dependent on cloud services and IoT-enabled SCADA systems.  
While this improves efficiency and monitoring capabilities, it also increases the attack surface.  
The central question explored in this project is:  

**How can critical solar infrastructure be secured against cyber threats such as espionage, lateral movement, and service disruption while using cloud-connected SCADA systems?**

---

## Risk Analysis and Key Observations

- **SCADA Weaknesses:**  
  SCADA systems often lack strong authentication and encryption, leaving them vulnerable to man-in-the-middle and denial-of-service attacks (Wali & Alshehry, 2024).  

- **Cloud Exposure:**  
  Remote maintenance and iSolarCloud connectivity increase potential entry points.  
  If network segmentation is poor, attackers can move laterally into critical control systems (NIST, 2023).  

- **Supplier Risk:**  
  SunGrow is a Chinese supplier, and Chinese firms may be subject to policies such as military-civil fusion (MCF), increasing the risk of espionage or sabotage (Jüris, 2023).  

- **State-Sponsored Threats:**  
  Volt Typhoon attacks demonstrate how nation-state groups exploit weaknesses in critical infrastructure for disruption (CISA, 2024).  

- **Lack of Oversight:**  
  Many nations lack strict monitoring requirements for foreign suppliers, leaving infrastructure exposed to hidden backdoors and data exfiltration risks.

---

## Recommended Mitigations

- **Secure Configuration and Maintenance:**  
  Update firmware, disable unused ports, and harden SCADA devices to reduce attack surface (NSM, 2024).  

- **Network Segmentation and Data Flow Control:**  
  Separate OT and IT networks and enforce firewall rules to minimize lateral movement (NIST, 2023).  

- **Strong Access Control:**  
  Implement multi-factor authentication, least-privilege principles, and comprehensive logging for accountability (Mortvedt, 2024).  

- **Continuous Monitoring and Anomaly Detection:**  
  Use IDS/IPS and behavioral analytics to quickly detect scanning, brute-force attempts, or abnormal commands.  

- **Supplier Due Diligence:**  
  Require security audits and transparency from technology providers before deploying them in critical systems.

---

## Lessons Learned

The exercise highlighted that cyber risk in energy infrastructure is not just a technical challenge but also a geopolitical one.  
Combining technical hardening, strict access control, and supplier governance is essential to safeguard national security.  
Early threat detection and rapid response, supported by frameworks like NIST CSF, can reduce impact from attacks like the Lviv incident.

---

## References

- Cybersecurity and Infrastructure Security Agency. (2024). *People's Republic of China cyber threat*. U.S. Department of Homeland Security. https://www.cisa.gov/topics/cyber-threats-and-advisories/nation-state-cyber-actors/china  
- Harrou, F., Taghezouit, B., Bouyeddou, B., & Sun, Y. (2023). *Cybersecurity of photovoltaic systems: Challenges, threats, and mitigation strategies: A short survey.* Frontiers in Energy Research, 11. https://doi.org/10.3389/fenrg.2023.1274451  
- Industrial Cyber. (2024). *FBI warns of increased cyber threats to expanding US renewable energy sector.* https://industrialcyber.co/threats-attacks/fbi-warns-of-increased-cyber-threats-to-expanding-us-renewable-energy-sector/  
- Jüris, F. (2023). *Security implications of China-owned critical infrastructure in the European Union.* European Parliament. https://www.europarl.europa.eu/RegData/etudes/IDAN/2023/702592/EXPO_IDA(2023)702592_EN.pdf  
- Mortvedt, S. (2024). *RPAM: Best praksis for sikker fjernaksess til kritisk infrastruktur.* Last Mile AS. https://fagstoff.lastmile.no/rpam-best-praksis-for-sikker-fjernaksess-til-kritisk-infrastruktur  
- National Institute of Standards and Technology. (2023). *Guide to operational technology (OT) security.* https://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-82r3.pdf  
- National Institute of Standards and Technology. (2024). *Cybersecurity for smart inverters: NIST releases draft guidelines.* https://csrc.nist.gov/News/2024/cybersecurity-for-smart-inverters-nist-releases-dr  
- Nasjonal sikkerhetsmyndighet (NSM). (2024). *Grunnprinsipper for IKT-sikkerhet versjon 2.1.* https://nsm.no/getfile.php/1313975-1717589722/NSM/Filer/Dokumenter/Veiledere/NSMs%20Grunnprinsipper%20for%20IKT-sikkerhet%20v2.1.pdf  
- Wali, A., & Alshehry, F. (2024). *A survey of security challenges in cloud-based SCADA systems.* Computers, 13(4), 97. https://doi.org/10.3390/computers13040097  
- Yawar, S. (2024). *Cyberattack in Lviv disrupts heating for 600 buildings.* https://www.pureversity.com/blog/frostygoop-malware-attac  
