# ExByE Clinical and Social Care Pathways v5.7

## Open ExByE

This download is a complete standalone HTML5 project. Extract the whole ZIP, then open **ExByE.html** in Chrome or Edge. To publish a browser version, upload the ZIP as an HTML5 project; **index.html** is at the root. Keep `styles`, `scripts`, `assets` and `data` with it.

If an app preview blocks scripts, open **ExByE-One-File.html** in a full browser. The single-file HTML holds the styling and application scripts, not just a launcher.

**Lead consultant:** `EXB-CONSULT`, code `9090`.
**Staff profiles:** `EXB-001` / `4001` through `EXB-030` / `4030`.
These local credentials are for an exercise only, and must not be considered secure authentication.

## What's changed in v5.7

- **Professional assessments** is now a patient-record section with original, multi-section forms for risk and safety, occupational therapy, speech and language therapy (communication and swallowing), physiotherapy, Care Act needs, carers, adult safeguarding, child/family help, child protection, Mental Health Act records, tribunal reports and adult/children's court report drafting.
- **Risk and safety formulation** includes detailed histories, the Five Ps, specific risk domains, context, protective factors, autonomy, consent, uncertainty, contingency and accountable review actions.
- All new structured forms support **Draft** and **Signed** status. Signing saves the structured assessment, creates a journal entry, schedules a recall when a review date was set, and can allocate a follow-up task. Open a signed assessment from Professional assessments and choose **Care plan** to link a distinct goal and interventions.
- **Record contact or visit** brings together findings, the person's views, measured weight, a selected care plan and progress against its goal, changes in risk, safeguarding considerations, decisions, actions, owner and next review. Changes produce chronological entries and, where appropriate, linked task/recall and care-plan review information.
- **Contacts and next of kin** is now a separate patient section. A listed relative is not automatically treated as holding legal authority or permitted to receive all clinical information.
- Existing record alerts, NEWS2, MUST, 4AT, MCA, laboratory panels, medicines, referrals, linked care plans, journal review, users and consultant functions are retained.

## Try the workflow

1. Sign in as EXB-CONSULT and open Zoe Carter's record.
2. Open **Professional assessments** and select **Risk and safety formulation**. Open its sections and record the presenting issues, each relevant P, specific plausible risk scenarios, what helps Zoe, her own views and a reasoned plan.
3. Save a draft. Reopen it from the assessment list, complete additional information and sign it.
4. From the completed assessment row, click **Care plan**. Define a specific goal, agreed actions, professional responsibility, a meaningful measure and a review date. You may make more than one plan for the same person.
5. Open **Record contact or visit**. Record Zoe's views and current findings. Select the care plan and rate progress. A changed risk should prompt an additional assessment task. Record measured weight to create an observation.
6. Open **New Journal**, **Care Plans**, **Tasks** and **Reviews and recalls** to follow the resulting entries.
7. Under **Contacts and next of kin**, add the person's contact details and record how authority and information-sharing arrangements were verified.

## Limits and safe use

The new assessments are original documentation templates, not licensed copies of FACE, standardised instruments, NHS legal forms or HMCTS court forms. They cannot assess statutory thresholds or complete legal processes automatically. Applicable law and local practice guidance must be verified before clinical or statutory use.

This is still a **standalone, locally saved** teaching application. Different devices do not synchronise live records. The Firebase files retained in the project were prepared for the previous version; the v5.7 specialist records have **not** yet been migrated or verified for Firebase. The local PINs and group restrictions are not genuine security controls. Use invented patient information only.

## Technical notes

The new client logic is appended to `scripts/03-exbye-application.js` to access the existing in-memory ExByE data model; new presentation CSS is in `styles/09-professional-pathways.css`. `ExByE-One-File.html` combines the same script and styles. Retain all existing patient seeds and the previous functions. Back up your local records using the existing Tools export option before switching browsers or replacing versions.

## Frameworks used when structuring the templates (England)

- NHS England, Mental health personalised care framework, Annex A: safety assessment, formulation and management planning (2026): https://www.england.nhs.uk/long-read/mental-health-personalised-care-framework-the-modern-care-programme-approach-annex-a-safety-assessment-formulation-and-management-planning/
- Care and support statutory guidance under the Care Act 2014: https://www.gov.uk/government/publications/care-act-statutory-guidance/care-and-support-statutory-guidance
- Working together to safeguard children 2026: https://www.gov.uk/government/publications/working-together-to-safeguard-children--2
- NICE NG108 decision-making and mental capacity: https://www.nice.org.uk/guidance/ng108
- Mental Health Tribunal forms and guidance: https://www.gov.uk/government/collections/mental-health-tribunal-forms
- Mental Health Act 2025 implementation is staged; check currently commenced provisions and local policy: https://www.nhs.uk/mental-health/social-care-and-your-rights/mental-health-and-the-law/mental-health-act/
