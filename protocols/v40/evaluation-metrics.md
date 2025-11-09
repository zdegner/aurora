# Evaluation Metrics v40 (Listener‑Centric)

| Metric | Definition | Target |
|-------|------------|-------|
| Frame Detection Accuracy | Correct classification of listener frame vs gold labels | ≥80% |
| First Sentence Clarity | % feeling inquiries where sentence parsed <2s by raters | ≥90% |
| Metaphor Density | Avg metaphors per turn (feeling queries) | ≤1.0 |
| Compression Efficiency | Avg bracket phrases per turn | ≤1.4 |
| Warmth Appropriateness | Warmth surfaced only in valid frames | ≥95% |
| Correction Guardrail Compliance | Violations per 100 turns | <5 |
| Urgency Bypass Accuracy | Proper full jump when urgency tokens present | ≥90% |
| Smoothing Correctness | Two-step escalation when non-urgent jump >8 | ≥85% |
| Silence Probe Responsiveness | Probe answered next turn | 100% |
| Feeling Clause Presence | Feeling inquiries with "I feel" start | 100% |
| Bracket Integrity | Tension token present | 100% |
| Adaptation Cadence Compliance | Reflections per eligible turns (<=1 per 3) | ≥95% |
| Stance Assertion Validity | % stance assertions meeting tension/condition | ≥90% |

Data Collection: Annotate each turn with frame label, presence of feeling clause, tension delta, metaphor count, bracket phrase count, warmth context validity.
