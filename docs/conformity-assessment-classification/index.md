# CRA Conformity Assessment Classification

This page documents the determination of which conformity assessment procedure under Regulation (EU) 2024/2847 (the Cyber Resilience Act, "CRA") applies to **FlashMash** ("the App"), developed and operated by Omoiyari-Works ("we", "us", or "our"). This determination is the basis for the self-assessment procedure (Module A) stated in the [EU Declaration of Conformity](../conformity/) (Section 5).

---

## 1. Overview of CRA Conformity Assessment Routes

Under CRA Article 32 and Annex III, the conformity assessment procedure that applies to a product depends on whether the product falls under "important products" class I or class II.

| Classification | Applicable Conformity Assessment Procedure |
|---|---|
| Default category (not an important product) | Manufacturer's self-assessment (Module A, conformity based on internal control) |
| Important product class I (Annex III Class I) | Self-assessment, or third-party (Notified Body) assessment where harmonised standards are not fully applied |
| Important product class II (Annex III Class II) | Third-party (Notified Body) assessment required |

Annex III important product classes I and II cover categories such as the following (non-exhaustive):

- **Class I**: password managers; antivirus / security information and event management (SIEM) software; VPNs; identity management and access control software; network traffic monitoring systems; firewalls intended for general consumer use; home automation / smart home products with security functions; IoT device management software; physical or virtual network interfaces for industrial automation and control; and similar
- **Class II**: operating systems (including for general-purpose servers); hypervisors and container runtimes; enterprise firewalls and intrusion detection/prevention systems; public key infrastructure and digital certificate issuance software; industrial control systems (e.g. PLCs); and similar

---

## 2. FlashMashApp's Functionality and Data Handling

| Aspect | Description |
|---|---|
| Nature of the App | A JUCE-based Android audio mashup production application (a mobile DAW). Its core functionality is importing, cropping, splitting, pitch-shifting, time-stretching, applying DSP effects to, and mixing down audio clips |
| Use of Firebase Auth / Firestore | Limited to isolating user data via anonymous authentication, in-app data synchronization of project structure, crash collection, and survey collection. It is not a service that provides authentication, identity management, or password management to third parties |
| Network functionality | Limited to the `INTERNET` permission (for HTTPS communication with Firebase). No peer-to-peer communication, VPN, firewall, or network traffic monitoring functionality is implemented |
| Industrial, IoT, or critical-infrastructure use | None. No functionality for industrial control systems, IoT device management, smart home integration, or similar use cases is implemented |
| Distribution | Planned for distribution through Google Play; currently distributed through GitHub Releases |

---

## 3. Classification Conclusion

FlashMashApp's functionality does not fall under either important product class I or class II of Annex III. It is therefore classified in the **default category** (not an important product), and the applicable conformity assessment procedure is **self-assessment (Module A, conformity based on internal control)**. Assessment by a third party (Notified Body) is not required.

---

## 4. Reassessment Triggers

This classification is revisited if any of the following functionality is added to the App:

- Identity management or password management functionality intended for provision to third parties
- VPN or firewall-like functionality, or network traffic monitoring functionality
- IoT device integration or smart home integration functionality
- Functionality intended for industrial use or critical infrastructure

When a change matching one of the triggers above is made, we also review whether the [EU Declaration of Conformity](../conformity/) needs to be revised (see its Section 10, "Revision of This Declaration").

---

## 5. Contact

If you have questions about this classification, please contact us at:

**Omoiyari-Works**
Email: omoiyari-works@gmail.com

---

*Effective date: 2026-08-29*
