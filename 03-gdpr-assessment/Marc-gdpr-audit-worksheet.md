# GDPR Audit Worksheet

**Prepared by:** Marc Tanguy  
**Scenario:** HR Resume Screening AI  
**Based on:** Nina-fact-pattern.md

---

# Section A — Data Map

| Field | Assessment |
|-------|------------|
| **Categories of personal data** | Name, email address, phone number, postal address (if included), education history, employment history, qualifications, skills, certifications, references, and any additional information voluntarily included in resumes or cover letters. Some resumes may also reveal special-category data, such as health information, trade union membership, religious beliefs, ethnicity, or disability status. |
| **Sources** | Information provided directly by job applicants through the company's careers page, resumes, cover letters, and applicant-tracking system (ATS). |
| **Purpose(s)** | (1) Evaluate candidates for open positions. (2) Rank applicants according to role requirements. (3) Store candidate profiles for future recruitment opportunities. |
| **Lawful basis per purpose** | Recruitment for current vacancies: **Performance of steps prior to entering into a contract (Art. 6(1)(b))**. Candidate database for future opportunities: **Consent (Art. 6(1)(a))** or **Legitimate Interests (Art. 6(1)(f))** depending on local employment law and retention practices. Legal review recommended. |
| **Retention period per purpose** | Recruitment records should be retained only for a defined period (e.g., 6–24 months depending on jurisdiction and litigation requirements). Indefinite retention is not recommended and should be replaced with a documented retention schedule. |
| **Recipients and sub-processors** | Internal HR and recruitment teams, Applicant Tracking System (ATS), AI screening provider, US-based cloud hosting provider. |
| **International transfers and transfer mechanism** | Yes. Applicant data is transferred to a US-based cloud processor. Appropriate safeguards such as the EU-US Data Privacy Framework (where applicable) or Standard Contractual Clauses (SCCs), together with a Transfer Impact Assessment (TIA), should be implemented. |

---

# Section B — Risk and Rights

## Are any special-category data present or inferable (Article 9)?

Yes. Although applicants are not explicitly asked to provide special-category data, resumes and cover letters may reveal health conditions, disabilities, trade union membership, religious affiliations, ethnicity, or other Article 9 data. The organization should avoid collecting or using this information unless a valid legal basis and Article 9 condition apply.

---

## Is there automated decision-making with legal or similarly significant effects (Article 22)?

Potentially. The AI ranks candidates and only the highest-ranked applicants are shown to recruiters by default, while lower-ranked candidates are unlikely to receive meaningful human review. Although a human remains involved, the practical effect of the ranking could significantly influence employment opportunities. This should be reviewed carefully to ensure meaningful human oversight is maintained.

---

## Is a DPIA required?

Yes.

Several EDPB criteria are present, including:

- Evaluation or scoring of individuals.
- Automated processing supporting employment decisions.
- Large-scale processing of applicant data.
- Processing of potentially sensitive personal information.
- Use of innovative AI technologies.

A Data Protection Impact Assessment should therefore be completed before deployment.

---

## What data subject friction points are most likely?

Applicants are likely to exercise:

- Right of access.
- Right to rectification.
- Right to erasure.
- Right to object to profiling.
- Requests for information about how the AI ranking was produced.

Clear privacy notices and documented response procedures should be established.

---

## Controller / Processor split

**Controller:** Employer operating the recruitment process.

**Processors:** Applicant Tracking System provider, AI screening platform provider, and US-based cloud hosting provider.

---

## Is a DPA required?

Yes.

A Data Processing Agreement should be in place with every processor involved in handling applicant data, including the AI vendor, ATS provider, and cloud infrastructure provider.

---

# Section C — Law Stacking

| Area | Assessment |
|------|------------|
| **AI Act cross-check** | The system is likely **High-Risk** under Annex III (Employment). The AI Act adds governance obligations such as risk management, technical documentation, logging, human oversight, and post-market monitoring beyond GDPR requirements. |
| **ePrivacy check** | No evidence of cookies, tracking pixels, or device-level tracking in the fact pattern. ePrivacy is therefore unlikely to introduce additional obligations beyond standard website operation. |
| **Data Act check** | Not applicable. The scenario does not involve connected devices, IoT products, or cloud switching obligations. |

---

# Overall Assessment

The proposed recruitment system may be deployed from a GDPR perspective, provided significant safeguards are implemented before production. The most important issues are ensuring meaningful human oversight over AI-assisted recruitment decisions, defining appropriate data retention periods, completing a DPIA, and establishing compliant international data transfer mechanisms for the US-based cloud provider.
