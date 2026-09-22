EGA New Client Intake MVP
A standalone browser prototype for new-client intake only. It deliberately stops at Ready for Needs Analysis.
Run it
No Python, virtual environment, or package installation is required.
Unzip the folder.
Double-click `index.html`.
Use the intake wizard in your browser.
The prototype does not transmit data anywhere and does not persist data after you close/reload the page. At completion you can download the structured intake as JSON or use Print / Save PDF.
Intake scope
Advisor creates intake
Advisor disclosure acknowledgement
Privacy consent / optional CASL consent
Minimum reusable client record
Investment profile questionnaire + automatic score/allocation
Individual Wealth Protection Health Check
Completeness validation
Client confirmation/signature
Advisor review/signature
Structured client record → Ready for Needs Analysis
Based on the uploaded EGA materials
2026 EGA investment profile / “KYC” questionnaire
Pilot Individual Wealth Protection Health Check
EGA Advisor Disclosure, Privacy Statement and CASL consent
Important implementation notes
The file called “KYC questionnaire” is an investment-risk profile. It does not contain a full identity-verification / AML / source-of-funds workflow. This prototype does not claim FINTRAC KYC completion.
The wealth-health-check form has a `Score` field but the supplied document does not define a scoring algorithm. The MVP therefore shows `checked items / 10` rather than inventing a score.
The investment-profile allocation table uses overlapping labels at exact boundary values (e.g. `12–24` and `24–32`). The MVP uses half-open bands internally. Confirm exact boundary behavior with EGA before production.
Client record fields such as DOB, phone, address and province are proposed minimum reusable fields for a digital intake and are not all present in the supplied forms.
Electronic signature, retention, authentication, audit logging, encryption, consent wording, and compliance sufficiency need production legal/compliance review.
What a production version should add
Secure one-time client links and authentication
Encryption at rest and in transit
Database / CRM integration
Audit trail and document versioning
Proper e-signature provider
Identity-verification / FINTRAC workflow if required
AI prefill from discovery notes/transcript, with field-level confidence and advisor review
Rule engine by province / advisor / product line
Final generated versions of the original EGA documents
