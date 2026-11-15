# National Immigration & Serious Crime Case Tracker — pilot

Status: **research pilot; no verified national case count**. This project catalogs *discoverable, documented cases*, not a census or an estimate of immigrant crime rates.

## Pilot
Initial historical window: 2026-08-15 through 2026-11-15 (incident dates); nationwide. Include homicide, fatal impaired-driving crashes, sexual assault, and major drug-trafficking prosecutions. Record later charges/convictions with separate outcome dates.

## Inclusion
1. An identifiable criminal incident with a dated, attributable police, court, or official investigative record.
2. Specific evidence of **unlawful presence at the time of the incident**, from an immigration court record, DHS/ICE documentation, or an attributed official confirmation corroborated where possible. Nationality, ethnicity, language, name, or lack of a driver's license are never proxies.
3. Original source URL and exact evidence location; record publication and access dates.
4. Status: alleged/charged/convicted/acquitted/dismissed; do not equate arrest with guilt.
5. Two independent reviewers before public release; record disagreements, corrections, and retractions.

## Exclusions and guardrails
- Exclude cases where status is unknown, disputed, or supported only by an unattributed social post; retain these as **candidates** only.
- Never scrape private records, bypass paywalls, CAPTCHA, robots restrictions, or platform access controls.
- Do not expose victim names, minors' identifiers, addresses, or unnecessary personal data.
- Count incidents, accused persons, victims, charges, and convictions **separately**. Never add them together.
- Deduplicate by jurisdiction, incident date, incident/court identifiers, and source cross-checks.
- For drug trafficking, distinguish possession, trafficking, seizures, and overdose deaths; do not infer causal overdose victims from a seizure.
- Prior detainer, removal, or release must be documented and does not automatically mean a later crime was preventable.
- Record jurisdiction coverage and search effort; news discovery bias makes national totals and rate comparisons invalid.
- Preserve source snapshots or bibliographic metadata only where copyright and terms permit.
- Do not publish a case unless reviewed; do not publish aggregate figures from unreviewed candidates.

## Pipeline
Discovery (public news / DOJ / ICE / accessible court feeds) → candidate rows → source verification → status validation → duplicate review → two-person approval → published case records → periodic outcome updates.

## Publication rule
Dashboard should display “Verified documented cases in this tracker,” never “all undocumented immigrant crimes nationwide.” Counts remain blank until reviewed records exist.
