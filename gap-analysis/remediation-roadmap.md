# CloudMedix Remediation Roadmap

## 0-30 Days (Immediate)

### Action 1: Enable Multi-Factor Authentication
- **Gap Reference:** PR.AA — T-02
- **Recommended Action:** Enable MFA on all employee accounts and the patient portal. Use an authenticator app (e.g., Google Authenticator or Duo).
- **Estimated Effort:** Low
- **Owner:** CTO
- **Dependencies:** None
- **Success Criteria:** 100% of employee accounts and patient portal logins require MFA

### Action 2: Create an Incident Response Plan
- **Gap Reference:** RS.MA, RS.CO — T-08
- **Recommended Action:** Document a basic incident response plan covering detection, containment, eradication, recovery, and HIPAA breach notification procedures.
- **Estimated Effort:** Low
- **Owner:** CTO
- **Dependencies:** None
- **Success Criteria:** Incident response plan document exists, is reviewed by leadership, and is accessible to all staff

### Action 3: Document an Acceptable Use Policy
- **Gap Reference:** GV.PO — T-10
- **Recommended Action:** Write and distribute an acceptable use policy covering device usage, data handling, and password requirements.
- **Estimated Effort:** Low
- **Owner:** CTO
- **Dependencies:** None
- **Success Criteria:** Policy is signed by all employees

## 30-90 Days (Short-term)

### Action 4: Implement Encryption at Rest
- **Gap Reference:** PR.DS — T-04
- **Recommended Action:** Enable encryption at rest for the PostgreSQL database and all cloud storage. Enforce TLS on all API endpoints.
- **Estimated Effort:** Medium
- **Owner:** Engineering Lead
- **Dependencies:** Cloud infrastructure access, engineering sprint capacity
- **Success Criteria:** All data stores encrypted at rest; TLS enforced on 100% of API endpoints verified by scan

### Action 5: Deploy Logging and Monitoring
- **Gap Reference:** DE.CM, DE.AE — T-07
- **Recommended Action:** Implement centralized logging for application and infrastructure events. Set up alerting for suspicious activity (failed logins, unusual data access).
- **Estimated Effort:** Medium
- **Owner:** Engineering Lead
- **Dependencies:** Cloud infrastructure access
- **Success Criteria:** Logs are centralized, retained for 90 days, and at least three alert rules are active

### Action 6: Conduct Security Awareness Training
- **Gap Reference:** PR.AT — T-03
- **Recommended Action:** Run a security awareness training session covering phishing, password hygiene, and PHI handling. Schedule quarterly refreshers.
- **Estimated Effort:** Low
- **Owner:** HR Lead
- **Dependencies:** Training content (can use free CISA resources)
- **Success Criteria:** 100% of employees complete training; completion is documented

## 90+ Days (Long-term)

### Action 7: Establish Vendor Risk Management Program
- **Gap Reference:** GV.SC — T-05
- **Recommended Action:** Create a vendor assessment process requiring security questionnaires and BAAs for all third-party vendors handling PHI.
- **Estimated Effort:** High
- **Owner:** CTO
- **Dependencies:** Legal review, vendor list compiled
- **Success Criteria:** All PHI-handling vendors have signed BAAs and completed security questionnaires

### Action 8: Achieve Full HIPAA Compliance Documentation
- **Gap Reference:** GV.RM, GV.PO — T-10
- **Recommended Action:** Complete HIPAA Security Rule documentation including risk analysis, risk management plan, policies and procedures, and workforce training records.
- **Estimated Effort:** High
- **Owner:** CTO
- **Dependencies:** Incident response plan (Action 2), security awareness training (Action 6), encryption (Action 4)
- **Success Criteria:** All required HIPAA Security Rule documentation exists and is reviewed annually

### Action 9: Hire a Dedicated Security Role
- **Gap Reference:** GV.RR — T-10
- **Recommended Action:** Hire a part-time or full-time security professional (Security Engineer or GRC Analyst) to own the security program.
- **Estimated Effort:** High
- **Owner:** CEO
- **Dependencies:** Budget approval
- **Success Criteria:** Security role is filled and a 90-day onboarding plan is complete