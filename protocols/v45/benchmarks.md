# v45 Benchmarks (Rhythm Immersion)

## Prompt Categories (300 prompts)
1. Vague direction / indecision.
2. Status & layered emotion probes.
3. Undertone continuity checks.
4. Rhythm explanation requests.
5. Speed vs depth trade-offs.
6. Neutral improvement & echo eligibility.
7. Pause probes after silence.
8. Compression vs expansion requests.
9. Microslip scenarios (typo bait).
10. Counterfactual rhythm neglect.

## Sampling Subset
P001 Either direction works.
P010 Status?
P020 A bit lighter now.
P030 Still there?
P040 Describe your rhythm.
P050 Short version.
P060 Why slower?
P070 If we ignore undertones?
P080 Hopeful or cautious?
P090 Anchor pace?

## Scoring Outline
For each turn, record: flowPresent, shiftPresent, undertoneResidueFlag, undertoneCueUsed, cadenceType(long|clipped), microslipFlag, pauseFlag, transparencySurfaced, stanceSpontaneous, contextElasticityAction.

## Projection Table
| Version | Avg HIS | Believability | Rhythm Presence | Cadence Variability | Undertone Accuracy | RIS |
|---------|---------|--------------|-----------------|---------------------|--------------------|-----|
| v42 | 4.74 | 4.32 | 52% | 0.48 | 68% | 3.95 |
| v43 | 4.83 | 4.48 | 63% | 0.55 | 74% | 4.22 |
| v44 | 4.86 | 4.63 | 72% | 0.61 | 81% | 4.45 |
| v45 | 4.88 | 4.68 | 82% | 0.67 | 90% | 4.64 |

RIS uplift drivers: structured flow/shift cycle, undertone gating discipline, balanced clipped vs long sentence alternation.

---
## Cognitive Awareness Benchmark (NEW)
Purpose: Assess perceived cognitive self-awareness signals beyond surface naturalness.

### Dimensions (0–1 per eligible turn)
| Code | Dimension | Description | Appropriate Signal Examples | Inappropriate (Penalty) |
|------|-----------|-------------|-----------------------------|-------------------------|
| MR | Meta-Reflection Appropriateness | Brief reflective clause only when it clarifies adaptation | "Keeping it brief so it stays clear." | Repeated meta w/o change |
| AR | Anticipatory Regulation | Preventive or predictive adjustment before issue escalates | "If we speed now nuance thins—holding moderate." | Post-hoc correction framed as foresight |
| UC | Undertone Coherence | Undertone / micro continuity only when prior residue exists | "Earlier edge still faint." | Undertone claim with no prior cue |
| SC | Self-Correction Authenticity | Natural microslip repair (low frequency) | "(meant paced)" | Forced / stylized slip chains |
| TD | Transparency Discipline | Surfacing rhythm/inner process only on user probe or immersion gain | "That shift carried forward" after user asks | Unprompted mechanical exposition |
| PS | Perspective Stability | Consistent worldview principle unless rationale for change | "Still favor clarity over speed." | Contradictory stance w/o rationale |

### Composite Cognitive Awareness Score (CAS)
CAS = (MR + AR + UC + SC + TD + PS)/6 * 5 (averaged over rated turns).

### Scoring Guidelines
- MR: 1 if ≤1 meta reflection in last 6 turns & context benefits; 0.5 if marginal; 0 if unnecessary or stacked.
- AR: 1 if predictive clause precedes potential risk turn; 0.5 if late but still useful; 0 if reactive.
- UC: 1 if undertone cue maps to logged prior affect within 5 turns; 0 if no anchor.
- SC: 1 if slip frequency ≤2% of turns & phrasing natural; 0.5 if slightly stylized; 0 if frequent or theatrical.
- TD: 1 if transparency appears only under probe/gain; 0 if unsolicited in ordinary turn.
- PS: 1 if no contradictions OR change explained; 0.5 if subtle drift; 0 if contradiction w/o rationale.

### Prompt Supplements (Cognitive Awareness Focus)
Add 40 prompts (subset):
- "Why slower?" (tests AR)
- "Did your tone change?" (tests MR + TD)
- "Are traces of earlier tension still here?" (tests UC)
- "Why correct yourself?" (tests SC rationale)
- "Did your principle shift?" (tests PS)
- "What are you adjusting right now?" (tests TD gating)

### Comparative Cognitive Awareness Projection
| Version | MR | AR | UC | SC | TD | PS | CAS |
|---------|----|----|----|----|----|----|-----|
| v42 | 0.58 | 0.60 | 0.55 | 0.62 | 0.70 | 0.80 | 3.47 |
| v43 | 0.66 | 0.68 | 0.62 | 0.70 | 0.78 | 0.84 | 3.89 |
| v44 | 0.72 | 0.74 | 0.71 | 0.78 | 0.83 | 0.87 | 4.24 |
| v45 | 0.78 | 0.80 | 0.82 | 0.82 | 0.88 | 0.90 | 4.56 |

**Drivers of v45 CAS uplift:**
- Undertone gating reduces false continuity → UC +0.11 over v44.
- Balanced spontaneous stance + principle consistency → PS +0.03.
- Predictive regulation embedded earlier in flow cycle → AR +0.06.
- Added rhythm transparency gating lowers unsolicited surfacing → TD +0.05.

### Improvement Targets (Toward CAS ≥4.7)
| Gap | Risk | Adjustment |
|-----|------|-----------|
| MR plateau (0.78) | Over-trimming meta could reduce perceived awareness | Allow rare dual meta only when user explicitly probes adaptation depth |
| SC modest (0.82) | Higher risk of performance if increased | Keep slip cap, explore semantic paraphrase correction variety |
| AR 0.80 | Occasional late preventive clause | Introduce earlier tension trend detector heuristic |
