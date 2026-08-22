# Identity and Access Management (IAM) Lab Portfolio

Welcome to my IAM engineering and administration portfolio. This repository documents a series of hands-on homelabs designed to build, secure, and troubleshoot enterprise identity architectures using industry-leading cloud platforms like Okta and Microsoft Entra ID. I am a recent graduate of DeVry University's undergraduate cybersecurity program. My passion for technology and security comes from life lessons from being hacked and watching family losing credentials and become victims of ransomware. I love information security and the professionals who keep data protected.

The goal of this portfolio is to bridge theoretical security concepts with practical implementation, focusing on Zero Trust principles, automated identity lifecycles, and secure federation.

---

## 🛠️ Skills & Technologies Demonstrated
* **Identity Providers (IdP):** Okta Identity Engine (OIE), Microsoft Entra ID
* **Access Control:** Role-Based Access Control (RBAC), Attribute-Based Access Control (ABAC), Adaptive Multi-Factor Authentication (MFA)
* **Lifecycle Management (LCM):** Automated User Provisioning/Deprovisioning, Custom Group Rules, Expression Languages
* **Federation & Protocols:** SAML 2.0, OpenID Connect (OIDC)
* **Governance & Security:** Network Zones, Risk-Based Policies, Access Reviews

---

## 📁 Lab Directory

| Lab # | Project Title | Core Technologies | Description |
| :---: | :--- | :--- | :--- |
| **01** | [Automated Lifecycle Management](https://github.com/Kendelv5/.-01-Lifecycle-Management-) | Okta, Expression Language | Automated contractor provisioning and group assignment using custom attribute rules. |
| **02** | [Adaptive MFA & Network Zones](https://github.com/Kendelv5/Lab03-Adaptive-MFA-Network-Zones) | Okta OIE, Network Security | Enforced step-up authentication based on corporate network boundaries and device context. |
| **03** | [SAML 2.0 Federation](https://github.com/Kendelv5/Lab03-SAML-2.0-Federation/blob/main/README.md) | Okta IdP, SAML | Configured single sign-on (SSO) and attribute mapping between an identity provider and a service provider. |
| **04A** | [On-Premises JML Automation](https://github.com/Kendelv5/04-JML-Lifecycle-Automation) | Active Directory, OUs, GPOs | Structured an on-premises enterprise JML framework utilizing Organizational Units, security groups, and manual offboarding controls. |
| **04B** | [Cloud JML Lifecycle Automation](https://github.com/Kendelv5/04B-JML-Automation-OKTA) | Okta OIE, Lifecycle Workflows | Designed a complete cloud-native Joiner-Mover-Leaver lifecycle workflow handling automated transitions, department shifts, and secure offboarding. |
---

## 🚀 Lab Architecture & Implementation Highlights

### Lab 1: Lifecycle Management & Group Rules
* **Challenge:** Manually managing temporary or contractor accounts introduces severe security oversight risks and administrative drag.
* **Solution:** Configured custom user attributes and Okta Expression Language rules (`user.department == "Contractor"`) to dynamically route users into specific security groups upon account activation.
* **Key Takeaway:** Mastered evaluating expression syntax and testing automated state transitions.

### Lab 2: Adaptive Multi-Factor Authentication
* **Challenge:** Balancing frictionless user experience with strict organizational security requirements.
* **Solution:** Established IP-based Network Zones to separate trusted corporate environments from external spaces, applying sign-on policies that trigger step-up MFA only for out-of-band access or sensitive resources.

### Lab 3: Adaptive Multi-Factor Authentication
* **Challenge:** Balancing frictionless user experience with strict organizational security requirements.
* **Solution:** Established IP-based Network Zones to separate trusted corporate environments from external spaces, applying sign-on policies that trigger step-up MFA only for out-of-band access or sensitive resources.

### Lab 4: JML Lifecycle Automation (Joiner-Mover-Leaver)
* **Challenge:** Ensuring seamless, secure permission updates when employees join, change roles internally, or leave the company without leaving orphaned accounts.
* **Solution:** Configured attribute-driven group rules to handle the **Joiner** phase (automatic app assignment), **Mover** phase (dynamic department/title updates, revoking old access and granting new apps), and **Leaver** phase (instant deactivation and suspension of active sessions).
* **Key Takeaway:** Built an automated state machine logic via identity attributes to drastically reduce administrative overhead and mitigate insider threat windows.
---

## 📈 Future Roadmap
* [ ] Integrate Microsoft Entra ID Conditional Access policies.
* [ ] Implement Privileged Identity Management (PIM) workflows.
* [ ] Automate infrastructure deployment of these labs using Terraform.

---
*Connect with me on [LinkedIn](https://linkedin.com) or reach out via email for inquiries.*
