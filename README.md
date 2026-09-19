# IT Audit & Controls Frameworks

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![License: CC0-1.0](https://img.shields.io/badge/license-CC0--1.0-lightgrey.svg)](LICENSE)

A curated list of standards, implementation guidance, and tooling for **COBIT**, **COSO Internal Control** and **COSO Enterprise Risk Management (ERM)**, and **IT General Controls / IT Application Controls (ITGC/ITAC)** — the frameworks that underpin most SOX 404 and financial-statement IT audit work.

**Scope:** Anything that materially helps a practitioner scope, design, test, or remediate controls against these frameworks — official standards, control matrices, testing methodologies, GRC platforms, and certification paths. Not generic accounting or audit content unrelated to IT controls.

**Why now:** PCAOB's amendment to AS 2201 (the standard governing audits of internal control over financial reporting) takes effect for fiscal years beginning after 15 December 2026, sharpening requirements around how auditors evaluate technology-related risks. COBIT 2019 remains ISACA's current governance framework, with the NIST CSF crosswalk guide keeping it relevant to security-driven audits. COSO's 2013 Internal Control and 2017 ERM frameworks remain the de facto global baseline nearly two decades after COSO began the modernisation.

Contributions welcome.

---

## Contents

- [Why These Frameworks Matter](#why-these-frameworks-matter)
- [How to Approach Implementation](#how-to-approach-implementation)
- [COBIT](#cobit)
- [COSO Internal Control and Enterprise Risk Management](#coso-internal-control-and-enterprise-risk-management)
- [ITGC and ITAC](#itgc-and-itac)
- [Cross-Framework Mapping and GRC Platforms](#cross-framework-mapping-and-grc-platforms)
- [Open-Source Audit and Controls Tooling](#open-source-audit-and-controls-tooling)
- [Assessment, Testing, and Control Matrix Resources](#assessment-testing-and-control-matrix-resources)
- [Certifications and Training](#certifications-and-training)
- [Government and Standards Bodies](#government-and-standards-bodies)
- [Learning Resources](#learning-resources)
- [Related Lists](#related-lists)

---

## Why These Frameworks Matter

These four pieces fit together as layers, not alternatives. COSO's Internal Control – Integrated Framework is the conceptual backbone almost every SOX 404 programme is built on: its five components (Control Environment, Risk Assessment, Control Activities, Information and Communication, Monitoring Activities) and seventeen principles are what management and auditors assess against when they conclude internal control is effective. COSO ERM sits alongside it as the enterprise risk lens, connecting control design to strategy and risk appetite rather than treating controls as a checklist. COBIT is the IT governance and management framework that translates those control objectives into IT-specific governance and management objectives, so a CIO or IT audit team has a structured way to organise IT policy, process, and accountability. ITGC and ITAC are where all of this becomes testable: ITGCs (access, change management, IT operations, sometimes program development) provide the control environment a financial application relies on, while ITACs (input completeness, accuracy, validity, and processing/output integrity) are the automated controls embedded inside a specific application or workflow.

A financial-statement or IT audit typically works top-down through this stack: COSO sets the control objectives, COBIT structures the IT governance and management response, and ITGC/ITAC testing is where an auditor gathers evidence that the controls actually operate.

---

## How to Approach Implementation

1. **Scope the audit.** Identify in-scope entities, business processes, and financial statement line items (a SOX scoping exercise), then trace those processes to the IT systems and applications that support them.
2. **Map the control environment to COSO.** Assess entity-level controls against the five COSO components and seventeen principles. This is the foundation an auditor or management team references when concluding on control effectiveness.
3. **Assess risk using COSO ERM.** Identify and prioritise the risks that threaten the in-scope objectives, connecting risk appetite and strategy to the specific controls chosen. This step determines how much testing depth each area warrants.
4. **Structure the IT governance response with COBIT.** Use COBIT's governance and management objectives (across the Evaluate-Direct-Monitor, Align-Plan-Organize, Build-Acquire-Implement, Deliver-Service-Support, and Monitor-Evaluate-Assess domains) to organise policies, processes, and accountability for the in-scope IT environment.
5. **Identify ITGCs for each in-scope system.** Document controls across the standard ITGC categories: logical access, change management, IT operations (backup, job scheduling, incident management), and, where relevant, program development / system implementation.
6. **Identify ITACs for each in-scope application.** Document the automated controls embedded in the application itself: input validation, calculation logic, interface controls, and exception/error handling.
7. **Build a Risk and Control Matrix (RCM).** Document each risk, the control that mitigates it, the control owner, frequency, and the type of evidence that will demonstrate operating effectiveness.
8. **Test design and operating effectiveness.** Perform walkthroughs to confirm design, then sample-test operating effectiveness over the audit period.
9. **Report, remediate, and retest.** Document deficiencies (control, significant, or material weakness under PCAOB definitions), track remediation, and retest before the reporting deadline.
10. **Monitor continuously.** COSO's Monitoring Activities component and COBIT's Monitor-Evaluate-Assess domain both expect this to be an ongoing management responsibility, not an annual event.

---

## COBIT

**Path to adoption:** free framework downloads from ISACA (registration required), not itself certifiable, though ISACA offers individual certificates (Foundations, Design & Implementation).

- [COBIT | ISACA](https://www.isaca.org/resources/cobit) - The official COBIT resource hub: framework downloads, focus areas, and the certification path.
- [COBIT 2019 Framework: Introduction and Methodology](https://www.isaca.org/store2/product/CB19FIMP-C) - The foundational publication explaining COBIT's principles and how the framework is structured.
- [COBIT 2019 Framework: Governance and Management Objectives](https://www.isaca.org/resources/cobit) - The 40 governance and management objectives across five domains (EDM, APO, BAI, DSS, MEA) that make up the core of the framework.
- [COBIT Design Guide](https://www.isaca.org/resources/cobit) - Guidance for tailoring COBIT's generic objectives to an organisation's specific context and risk profile.
- [COBIT Implementation Guide](https://www.isaca.org/resources/cobit) - A phased approach (based on ISACA's continual improvement life cycle) for rolling out COBIT in an enterprise.
- [Implementing the NIST Cybersecurity Framework Using COBIT 2019](https://www.isaca.org/resources/cobit) - ISACA's official crosswalk between COBIT and NIST CSF, useful where security and IT governance audits overlap (see the companion [Security Frameworks](https://github.com/garynair/security-frameworks) list).

## COSO Internal Control and Enterprise Risk Management

**Path to adoption:** not certifiable; adopted by reference as the control framework management and auditors assess against. The full framework documents are paywalled (sold via AICPA/CPA2BIZ as COSO's licensing agent); COSO's own site provides free guidance pages and executive summaries.

- [Internal Control - Integrated Framework | COSO](https://www.coso.org/guidance-on-ic) - COSO's official guidance page for the 2013 Internal Control framework: overview, FAQs, and links to purchase the full framework and supplemental guidance. The full document is paywalled and not freely redistributable.
- [COSO ERM Framework | COSO](https://www.coso.org/erm-framework) - COSO's official guidance page for the 2017 Enterprise Risk Management framework: overview and purchase links. Also paywalled in full.
- [COSO](https://www.coso.org/) - The Committee of Sponsoring Organizations of the Treadway Commission's home page: news, guidance thought papers, and the full publication catalogue.
- [AICPA & CIMA: COSO Internal Control - Integrated Framework](https://www.aicpa-cima.com/resources/landing/coso-internal-control-integrated-framework) - AICPA's resource landing page (COSO's licensing and distribution partner), including free implementation guidance alongside paid framework purchases.

## ITGC and ITAC

**Path to adoption:** not a single named standard; ITGC/ITAC is the audit-execution vocabulary that PCAOB, AICPA, and ISACA guidance converge on. Scope and test as part of a SOX 404 or financial-statement IT audit, using COBIT and COSO as the conceptual scaffolding above.

- [AS 2201: An Audit of Internal Control Over Financial Reporting](https://pcaobus.org/oversight/standards/auditing-standards/details/AS2201) - The PCAOB standard governing how an auditor evaluates internal control over financial reporting, including the IT-controls evaluation that drives ITGC/ITAC scoping. Amendment effective for fiscal years beginning after 15 December 2026.
- [PCAOB Auditing Standards](https://pcaobus.org/oversight/standards/auditing-standards) - The full current PCAOB standards library, the authoritative source for any ICFR audit requirement referenced above.
- [AICPA SOC 2 Trust Services Criteria](https://www.aicpa-cima.com/resources/download/get-description-criteria-for-your-organizations-soc-2-r-report) - The criteria (Security, Availability, Processing Integrity, Confidentiality, Privacy) used in SOC 2 engagements; heavily overlapping with ITGC categories and frequently tested using the same evidence.
- [ISACA IT Control Objectives for Sarbanes-Oxley](https://www.isaca.org/resources/cobit) - ISACA's guide mapping COBIT control objectives directly to SOX 404 IT control requirements, historically the standard reference for scoping ITGCs against COBIT.

---

## Cross-Framework Mapping and GRC Platforms

- [Secure Controls Framework (SCF)](https://securecontrolsframework.com/) - Free, open (Creative Commons) meta-framework mapping outward to 250+ laws, regulations, and frameworks, including COBIT-adjacent and SOX-relevant control sets alongside NIST, ISO, and PCI-DSS. Shared with the companion [Security Frameworks](https://github.com/garynair/security-frameworks) list.
- [AuditBoard](https://www.auditboard.com/) - Commercial GRC and SOX-management platform purpose-built for control matrices, walkthroughs, testing workflows, and issue tracking across ITGC/ITAC engagements.
- [Workiva](https://www.workiva.com/) - Commercial platform for SOX compliance, internal controls management, and financial reporting workflows, with control-testing and certification modules.
- [OneTrust](https://www.onetrust.com/) - Enterprise GRC platform covering IT and financial controls alongside broader privacy and third-party risk management.
- [Hyperproof](https://hyperproof.io/) - Commercial GRC platform focused on control-to-evidence traceability, usable across COSO/COBIT-driven programmes as well as security frameworks.

---

## Open-Source Audit and Controls Tooling

- [NIST OSCAL](https://github.com/usnistgov/OSCAL) - NIST's open, machine-readable format for control catalogues and assessment results. Not COBIT/COSO-native, but increasingly used as the underlying data model for control-mapping tooling that spans IT audit and security frameworks.
- [InSpec](https://github.com/inspec/inspec) - Chef's open-source compliance-as-code framework. Useful for automating the technical evidence-gathering half of ITGC testing (configuration and access control checks) that feeds a manual control matrix.

---

## Assessment, Testing, and Control Matrix Resources

- [PCAOB Staff Audit Practice Alerts](https://pcaobus.org/oversight/standards/auditing-standards) - Ongoing PCAOB guidance clarifying how AS 2201 and related standards should be applied in practice, including IT-controls-specific alerts.
- [ISACA Audit and Assurance Resources](https://www.isaca.org/resources/audit-and-assurance) - ISACA's library of audit programmes, control matrices, and assurance guidance, several of which are COBIT-aligned ITGC test plans.
- [AICPA Audit and Attest Standards](https://www.aicpa-cima.com/resources) - AICPA's standards and guidance library, the reference point for SOC 1/SOC 2 engagements that share testing methodology with SOX ITGC work.

---

## Certifications and Training

- [ISACA CISA](https://www.isaca.org/credentialing/cisa) - Certified Information Systems Auditor. The standard credential for IT audit professionals testing ITGC/ITAC and COBIT-aligned controls.
- [ISACA CGEIT](https://www.isaca.org/credentialing/cgeit) - Certified in the Governance of Enterprise IT, ISACA's credential most directly aligned with COBIT's governance objectives.
- [ISACA CRISC](https://www.isaca.org/credentialing/crisc) - Certified in Risk and Information Systems Control, aligned with the COSO ERM risk-assessment step in the roadmap above.
- [ISACA COBIT Certificates](https://www.isaca.org/credentialing/cobit) - COBIT Foundations and COBIT Design & Implementation certificates for practitioners implementing the framework directly.
- [IIA Certified Internal Auditor (CIA)](https://www.theiia.org/en/certifications/cia/) - The Institute of Internal Auditors' flagship certification, broader than IT but foundational for anyone running a COSO-based internal audit function.

---

## Government and Standards Bodies

- [ISACA](https://www.isaca.org/) - The professional association that owns and maintains COBIT, and publishes CISA, CGEIT, and CRISC certifications.
- [COSO](https://www.coso.org/) - The Committee of Sponsoring Organizations of the Treadway Commission, publisher of the Internal Control and ERM frameworks.
- [Public Company Accounting Oversight Board (PCAOB)](https://pcaobus.org/) - The US body that sets and enforces auditing standards, including AS 2201, for audits of public companies.
- [AICPA & CIMA](https://www.aicpa-cima.com/) - The American Institute of CPAs, COSO's licensing and distribution partner, and publisher of SOC 1/SOC 2 attestation standards.
- [The Institute of Internal Auditors (IIA)](https://www.theiia.org/) - The global professional association for internal auditors, publisher of the International Professional Practices Framework (IPPF).

---

## Learning Resources

- [ISACA Journal](https://www.isaca.org/resources/isaca-journal) - ISACA's practitioner journal, regularly covering COBIT implementation case studies and ITGC testing practice.
- [COSO Guidance Thought Papers](https://www.coso.org/guidance) - Free supplemental thought papers from COSO on applying the Internal Control and ERM frameworks in specific contexts (fraud risk, cyber risk, and more).
- [PCAOB Inspections Reports](https://pcaobus.org/oversight/inspections) - Public PCAOB inspection findings, a practical view into where auditors most often find ITGC and ICFR testing deficient.

---

## Related Lists

- [AI Governance](https://github.com/garynair/ai-governance) - A companion curated list covering AI-specific governance: regulation, standards, and runtime controls for autonomous agents.
- [Security Frameworks](https://github.com/garynair/security-frameworks) - A companion curated list covering NIST CSF, ISO/IEC 27001, and PCI-DSS, with a shared control-mapping tooling section.

---

## Contributing

PRs welcome. See [CONTRIBUTING.md](CONTRIBUTING.md) for the criteria a new entry must meet.

## Licence

This list is published under [CC0 1.0 Universal](LICENSE). The linked resources retain their own licences; the COSO Internal Control and ERM frameworks in particular are paywalled and not freely redistributable.
