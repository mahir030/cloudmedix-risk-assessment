# CloudMedix Threat Analysis

## Threat-Vulnerability Pairs

### T-01: SQL Injection on Patient Portal
- **Threat:** Attacker executes SQL injection against the patient portal search or input fields
- **Vulnerability:** Unsanitized user input in database queries
- **Potential Impact:** Unauthorized access to PHI, HIPAA breach notification required, regulatory fines
- **NIST CSF 2.0 Function:** Protect (PR)

### T-02: Credential Stuffing Against User Accounts
- **Threat:** Attacker uses leaked credential lists to gain unauthorized access to patient accounts
- **Vulnerability:** No multi-factor authentication (MFA), no account lockout policy
- **Potential Impact:** Unauthorized PHI access, account takeover, HIPAA violation
- **NIST CSF 2.0 Function:** Protect (PR)

### T-03: Phishing Attack Targeting Employees
- **Threat:** Employee clicks malicious link or attachment, leading to credential theft or malware installation
- **Vulnerability:** No security awareness training, no email filtering controls
- **Potential Impact:** Compromised employee credentials, lateral movement to production systems, PHI exposure
- **NIST CSF 2.0 Function:** Protect (PR)

### T-04: Unencrypted PHI in Transit
- **Threat:** Network attacker intercepts patient data transmitted between client and server
- **Vulnerability:** Inconsistent or missing TLS enforcement on API endpoints
- **Potential Impact:** PHI exposure, HIPAA violation, patient harm
- **NIST CSF 2.0 Function:** Protect (PR)

### T-05: Misconfigured Cloud Storage Exposing PHI
- **Threat:** Cloud storage bucket or database is accidentally made publicly accessible
- **Vulnerability:** No cloud configuration review process, no automated misconfiguration detection
- **Potential Impact:** Mass PHI exposure, regulatory fines, reputational damage
- **NIST CSF 2.0 Function:** Identity (ID)

### T-06: Insider Threat - Unauthorized PHI Access
- **Threat:** Employee accesses patient records beyond their job function
- **Vulnerability:** No role-based access control (RBAC), no access review process
- **Potential Impact:** HIPAA violation, patient privacy breach, legal liability
- **NIST CSF 2.0 Function:** Protect (PR)

### T-07: Undetected Security Breach
- **Threat:** Attacker maintains persistent access to systems without detection
- **Vulnerability:** No logging, monitoring, or alerting in place
- **Potential Impact:** Prolonged PHI exposure, delayed breach response, increased regulatory penalties
- **NIST CSF 2.0 Function:** Detect (DE)

### T-08: No Incident Response Capability
- **Threat:** A security incident occurs with no documented process to contain or recover from it
- **Vulnerability:** No incident response plan exists
- **Potential Impact:** Extended downtime, uncontrolled breach spread, failure to meet HIPAA breach notification timelines
- **NIST CSF 2.0 Function:** Respond (RS)

### T-09: Data Loss Due to Missing Backups
- **Threat:** Ransomware or accidental deletion destroys patient data with no recovery path
- **Vulnerability:** No documented backup or disaster recovery process
- **Potential Impact:** Permanent PHI loss, inability to restore services, HIPAA violation
- **NIST CSF 2.0 Function:** Recover (RC)

### T-10: No Formal Security Governance
- **Threat:** Security decisions are made ad hoc with no policy framework, leading to inconsistent controls
- **Vulnerability:** No security policies, no risk management program, no defined security roles
- **Potential Impact:** Systemic control failures across all risk areas, inability to demonstrate HIPAA compliance
- **NIST CSF 2.0 Function:** Govern (GV)