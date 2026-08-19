# Healthcare Cybersecurity Risk Assessment

## Cybersecurity Assessment of a Simulated Hospital Radiology Environment

### Overview

This project presents a simulated cybersecurity risk assessment of a hospital radiology environment.

The assessment focuses on critical healthcare assets including PACS, RIS, CT, MRI, X-ray systems, radiologist workstations, the hospital network, and patient information.

### Objectives

- Identify critical healthcare assets
- Identify cybersecurity threats
- Identify potential vulnerabilities
- Assess cybersecurity risks
- Recommend security controls
- Map security recommendations to the NIST Cybersecurity Framework

### Environment

The project uses a simulated hospital named Al Noor General Hospital.

The environment includes:

- CT
- MRI
- X-ray
- PACS
- RIS
- EHR
- Radiologist workstations
- Hospital network
- Patient information

### Risk Assessment

The assessment uses a simple risk scoring methodology:

**Risk Score = Likelihood × Impact**

Likelihood and impact are scored from 1 to 5.

### Key Risks

The assessment identified several high and critical risks, including:

- PACS ransomware
- Hospital network intrusion
- Workstation malware
- Credential theft
- Patient data exfiltration

### Recommended Controls

Recommended controls include:

- Multi-Factor Authentication (MFA)
- Network segmentation
- Endpoint Detection and Response (EDR)
- Role-Based Access Control (RBAC)
- Patch management
- Security monitoring
- Offline / immutable backups
- Incident response

### Framework

Security recommendations were mapped to the NIST Cybersecurity Framework (CSF).

### Medical Device Security

The project considers cybersecurity challenges associated with medical devices and legacy systems, including controlled patching, network segmentation, vendor coordination, and compensating controls.

### Disclaimer

This is a simulated educational project. No real hospital systems, medical devices, production networks, or patient data were accessed or tested.

### Hospital Network Architecture

```
┌──────────────┐
                 │     EHR      │
                 └──────▲───────┘
                        │
                    Hospital
                     Network
                        │
        ┌───────────────┼───────────────┐
        │               │               │
      PACS             RIS          Workstation
        ▲               ▲               │
        │               │               │
   ┌────┼────┐          │          Radiologist
   │    │    │
  CT   MRI  X-Ray 
  """
```

### Attack Path (Simulated)
```
 Phishing
   ↓
Compromised Workstation
   ↓
Credential Theft
   ↓
Lateral Movement
   ↓
PACS
   ↓
Ransomware
   ↓
Radiology Disruption

```

  
