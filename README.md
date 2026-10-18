# ExByE Professional Pathways v5.7

Start with **START_HERE_V57.md** for logins, modules and care-plan links.

# ExByE Clinical Records v5.6

## Open the current edition

Extract the full ZIP and open `index.html` or `ExByE.html` in Chrome, Edge or Safari. The `ExByE-One-File.html` fallback runs without linked folders. No Python, account subscription or local database installation is required.

## Starting accounts (offline edition)

- Staff identifiers `EXB-001` to `EXB-030`. Access codes run from `4001` to `4030`, using the matching numeric suffix.
- Lead consultant `EXB-CONSULT`, local access code `9090`. The consultant can open all records and withdraw journal entries or archive patient records. Other users cannot withdraw entries.
- Five multidisciplinary groups (A to E). Each group sees its allocated records, with some records accessible to multiple groups.

These codes are only **local demonstration controls**, not secure passwords. HTML source can be read by anyone with the files. Browser data is not synchronised between devices. Do not enter actual patient information. The Firebase edition provisions separate secure passwords and enforces permissions in Firestore rules.

## Seven starting records

1. **Zoe Carter, 32**: mild learning disability, alcohol dependence, incomplete SADQ, elevated liver blood results and weight loss, mother at home, daughter living with father, family service questions and protective factors.
2. **Freddy Mason, 56**: young-onset Alzheimer's disease, type 1 diabetes, ward admission following hypoglycaemia, possible insulin dose errors, insulin review and discharge planning.
3. **Tommy Reed, 27**: mild learning disability, autism, chronic constipation, recent sepsis and rectal trauma from attempts to remove impacted stool, supported-living care plan.
4. **Robby Ellis, 40**: non-speaking, new incontinence, episodes staff believe may be seizures. Record intentionally sparse; meaningful history and infection findings can be introduced subsequently.
5. **Gwen Harris, 36**: Down syndrome, learning disability, epilepsy review and relationships. Comprehensive assessment deliberately incomplete with named follow-up actions.
6. **Isla Bennett, 9**: asthma control, school attendance and inhaler technique, no learning disability recorded.
7. **Ethan Okafor, 15**: recurrent abdominal pain, incomplete investigation history, school absence and young person confidentiality, no learning disability recorded.

All people, organisations and identifiers are invented. Clinical details are intended for educational use only, not validated clinical decision support.

## Workflow changes

- Every clinical journal entry can be marked **For review**, with a named receiving professional, due date and review notes.
- The receiving review creates a task and a linked journal review entry; completion closes related open tasks.
- Staff tasks can be allocated to an `EXB-###` identifier. Other roles cannot withdraw journal entries.
- Updates to tasks, medicines, care plans, investigations and other structured records are reflected in the living clinical journal, with source IDs where available.
- Existing NEWS2, 4AT, full risk assessment, capacity assessment, blood panels, medication-warning examples, discipline templates, care planning and recalls are retained.
- The lead consultant can withdraw an entry, preserving the audit record, or archive a patient; the local controls do not constitute a secure authorization boundary.

## Cloud-ready package

The `firebase` directory includes a Firebase-hosted sign-in page, Firestore rules, account/patient provisioning, and a cloud synchronisation adapter. **No live Firebase project has been configured or tested with these files.** You must follow `firebase/SETUP_STEP_BY_STEP.md` and verify the security and multi-user tests before deployment. The standalone `index.html` and the Firebase `firebase/site/index.html` are different launchers: the latter is prepared with `npm run prepare` and contains no preloaded patient histories.
