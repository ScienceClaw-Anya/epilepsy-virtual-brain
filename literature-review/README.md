# Epilepsy Virtual-Brain Agent Collective: literature review

Evidence review for the ScienceClaw Hackathon project (31 Oct 2026).

| File | What it is |
|---|---|
| [`round1/evidence_audit.html`](round1/evidence_audit.html) | Claim-by-claim audit of the project plan (17 claims graded), corrected citations, dataset checks (VEC, ds003029, HUP ds004100), design risks |
| [`round2/fulltext_review.html`](round2/fulltext_review.html) | 21 papers read in full: verdict changes, a build sheet of copyable model settings (VEC/Epileptor parameters, metrics, baselines), new literature and a revised experiment plan |

Open the `.html` files in a browser. Every quote in round 2 was string-matched against the source full text. DOIs were resolved on Crossref.

Key corrections to the plan:
- Wang et al. 2025 is in *Nature Computational Science* and models stimulation for **diagnosis**, not therapy.
- Intervention plus simulated verification is already published (An 2019, Olmi 2019, Wang 2023, Lopez-Sola 2025). The novelty is a head-to-head benchmark with per-patient adjudication.
- Use closed-loop feedback (Moosavi 2025) or a physiological neural mass model for therapeutic stimulation. Open-loop periodic input in Epileptor only triggers seizures.
- Use HUP ds004100 for the real-surgery check.

This is a research-methods review, not clinical advice.
