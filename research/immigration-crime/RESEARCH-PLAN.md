# Research plan — comprehensive national case discovery

## Two clocks
- **Incident cohort:** initially 2026-08-15 through 2026-11-15; only qualifying incident dates count toward pilot incident totals.
- **Reporting cohort:** any DOJ/news release published during the pilot may identify older incidents. Keep these in the historical backlog, not the pilot incident numerator.
- Record offense, arrest, charging, conviction, sentencing, publication, and status-verification dates separately.

## Source tiers and discovery coverage
1. **Official case documents:** federal PACER docket identifiers, accessible state court dockets, sentencing memoranda, plea agreements, court judgments, charging documents. Verify identity and outcomes.
2. **Official announcements:** DOJ USAO press releases across all 94 federal judicial districts; ICE/HSI/ERO; state/local police; prosecutors; state corrections; crash-investigation agencies.
3. **Independent reporting:** local newsrooms, investigative reporting, original victim interviews where consent and privacy permit. Use to find cases; never infer immigration status from name or nationality.
4. **Audit context:** GAO, DHS OIG, state auditor reports, data dictionaries, jurisdiction-level reporting completeness and detention/release policies.

## Coverage ledger (required for every sweep)
Record date of search, agency/jurisdiction, query or feed, accessible results, examined results, candidates, exclusions, broken links, source restrictions and reviewer. Maintain a list of unsearched jurisdictions; never imply full national coverage based on a partial sweep.

## Search terms
Use neutral case-finding queries across categories:
- homicide/murder/manslaughter + DHS-confirmed unlawful presence
- fatal DUI/DWI/OWI/vehicular homicide + immigration status confirmed
- sexual assault/rape + DHS status or immigration court record
- fentanyl/meth trafficking + illegal reentry/removal + conviction
- detainer, prior deportation, removal, release, reentry, criminal history
Include counterexamples, acquittals, mistaken identifications, corrections and overturned convictions.

## Extraction and reconciliation
- Case-level unique key: jurisdiction + incident date + docket/incident ID; provisional composite only when docket unavailable.
- Multiple defendants in one incident: separate person records linked to one incident. Multiple victims: record separately without inflating incident counts.
- Charge vs conviction vs sentencing outcomes: separate, dated fields.
- Distinguish fatal impaired driving from prior DUI convictions without fatalities.
- Status must be established *at the incident date*, not merely at sentencing.
- Preserve exact evidence citations, conflicting reports, missing details and corrections.
- Independently check official source claims against accessible court records before verified status.
- Avoid names of victims and unnecessary personally identifying data in public release.

## Verification statuses
discovered → source_checked → immigration_status_confirmed → legal_outcome_checked → deduplicated → reviewer_1_approved → reviewer_2_approved → published. Any conflict → disputed/hold. No automatic public release.

## Dashboard publication rules
- Headline: 'Verified documented cases in this tracker', only after approvals.
- Coverage date, jurisdiction count, number of sources searched, and last reviewed displayed.
- No inferred national totals, incidence rates, immigrant/citizen comparisons, or conclusions about preventability from a convenience sample.
- Explicitly identify selection and news coverage bias.
- Show incident-date versus sentencing-date views only when adequately populated.
- Keep Texas DPS aggregate separate from individually verified case records; do not sum.
