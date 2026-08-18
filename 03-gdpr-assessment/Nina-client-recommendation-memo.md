# GDPR Compliance Memorandum

**To:** NordSecure Health
**Subject:** AI-Assisted Underwriting System — Initial GDPR Review
**Prepared by:** Janaina Hoffmann

---

## Recommendation

> **Proceed, subject to the conditions set out below.**

The system's underlying objective — accelerating and standardizing underwriting decisions while identifying potentially fraudulent applications — constitutes a legitimate business purpose. However, given the sensitivity of the data involved, several matters require remediation prior to deployment against real applicant data.

---

## 1. Primary Finding — Legal Basis for Health Data

This system processes **health data**, which GDPR designates as a special category subject to enhanced protection under **Article 9**. This includes:

- Medical questionnaires and declared conditions
- Body mass index (BMI)
- Lifestyle indicators (smoking, alcohol consumption)

Data of this nature cannot generally be processed on the legal bases applicable to ordinary personal data. An additional Article 9 legal basis — such as **explicit consent** or a basis specific to insurance underwriting recognized under Member State law — must be identified and formally documented before processing continues.

> ⚠️ **This is the priority issue.** Without a valid Article 9 basis, the lawfulness of the entire processing activity is undermined.

---

## 2. Secondary Findings

### 2.1 Human oversight requires reinforcement

Underwriters currently review each AI-generated recommendation, but in practice tend to follow it absent a specific reason to deviate.

**Risk:** If human review becomes largely nominal over time, the system risks constituting an automated decision under **Article 22**, which would trigger additional safeguards.

**Recommended action:**
- Formally document what constitutes "meaningful review" in practice
- Periodically audit a sample of accepted recommendations to verify substantive engagement

### 2.2 International data transfer

The underwriting platform is hosted by a **US-based cloud provider**, resulting in health data being transferred outside the EEA.

**Recommended action:**
- Implement a valid transfer mechanism (e.g., Standard Contractual Clauses)
- Support this with a documented Transfer Impact Assessment

### 2.3 Fraud detection is a separate purpose

Using the system to flag potentially fraudulent applications is **distinct from underwriting** and should be independently identified, justified, and documented — combining purposes without separate justification can create gaps under the purpose limitation principle.

---

## 3. Areas of Existing Compliance

✅ Human underwriter review is built into every decision
✅ The organization already recognizes health data requires enhanced protection

This review does **not** recommend halting the project — only closing a defined set of gaps before deployment.

---

## 4. Residual Risk

Even after the above measures are implemented, the following risks remain:

| Risk | Why it matters |
|---|---|
| **DPIA not yet conducted** | Required given the scale of special-category data and cross-border processing — not optional |
| **Applicant access requests** | Applicants may request an explanation of their risk score; no process currently defined |
| **National variation** | Insurance and health-data rules may differ slightly across the five Member States and should be reviewed individually |

---

## Closing Note

This assessment is a **first-pass review** and does not represent formal legal advice. Given the volume of special-category health data involved, a full DPIA and legal review are strongly recommended before this system processes real applications.

**Kind regards,**
Janaina Hoffmann
