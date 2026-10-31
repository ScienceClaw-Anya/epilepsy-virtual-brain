# SCOPE.lock — Round 3 (datasets) · signed by Nicole 2026-10-31

## Question
For each candidate epilepsy dataset: what exactly does it contain (data types, formats, cohort/sample details, labels, outcomes, access route), and which step of the virtual-brain agent pipeline can it serve?

## Inclusion test (first failing clause decides)
1. Human epilepsy patients (controls alongside OK). Animal only → FAIL.
2. Has ≥1 pipeline asset, else FAIL:
   A. structural MRI (± diffusion) to build a virtual brain
   B. iEEG/SEEG with seizure or SOZ/EZ annotations
   C. outcome (Engel/ILAE) linked to resected/stimulated tissue
   D. population prior: genetics, lesion maps, normative atlases, large clinical EEG (≥1,000 patients)
3. Documented access route (open / DUA / consortium). "On request from authors" only → FAIL.
4. ≥10 patients, or a collection of single-patient sets counted as one entry (exception: unique stimulation data).

## Grades
- **A build-ready**: open AND serves A/B/C directly
- **B usable with effort**: approval needed or a key piece missing
- **C prior/reference only**

## Card fields
Identity (repo, accession, version, descriptor DOI) · Access (tier, licence, steps) · Cohort (N, controls, age, sex, epilepsy types, sites) · Modalities & acquisition · Format & size · Labels & outcomes · Derived data · Caveats · Pipeline use · Verbatim evidence

## Worked examples
- PASS HUP ds004100: iEEG + SOZ/resection labels + Engel, CC0 → A
- PASS Epi25: genetic prior (2D), browser + dbGaP route → C
- FAIL Canine Epilepsy Dataset: animal (clause 1)
- FAIL CHB-MIT: 23-patient scalp EEG, no SOZ/outcome (clause 2)
- FAIL single-centre study, data "on request" (clause 3)

## Settings signed with the lock
- Scope: Nicole's 6 + R1/R2 datasets (VEC, ds004100, ds003876) + sweep (Pennsieve/epilepsy.science, OpenNeuro, PhysioNet, ENIGMA)
- Depth: open the actual repository files where reachable (participants, file tree, channel/electrode files, licence, sizes), not just the paper
- Output: house-style R3 HTML report + catalog spreadsheet

## Precedents (added during the round)
