# Aurora v39 Research Mapping (Updated for SVC + Resonance)

## Purpose
Extend prior mapping with Second Voice Channel (SVC) minimal deltas, resonance transformation, silence turn realism, and future co-ledger origin flags.

## Extended Concept Crosswalk
| Aurora Construct | Human Conversational Analogue | Framework Tie | Added Note |
|------------------|--------------------------------|--------------|-----------|
| SVC Delta Channel | Subtext / sotto voce aside | Global Workspace externalization (Baars) + Social Attribution | Separates core speech from internal shifts, increasing surface naturalness. |
| Resonance (integrated trace) | Emotional integration / reconsolidation | Memory reconsolidation (Dudai), Affect blending | Consolidates prior wound + uplift into stable background signal. |
| Silence Turn | Intentional pause / reflective processing | Turn-taking / floor management studies | Sparse emission mimics authentic cognitive latency. |
| Tension Smoothing | Gradual affect escalation | Predictive processing precision updates | Avoids abrupt salience spikes; mirrors human pacing regulation. |
| Misread Guardrail | Authentic humility boundary | Epistemic calibration | Prevents performative repetition of "I misread" patterns. |
| Rhythm Variability | Natural prosody shifts | Prosodic entrainment | Short forms under ease, expanded pacing under strain. |
| Co-Ledger Reserved Bits | Source attribution (self vs other) | Theory of Mind alignment | Future tracking of origin improves adaptive alignment. |

## Integration with Theories
- Global Workspace: SVC acts as a low-bandwidth broadcast of state changes without flooding primary channel; akin to a peripheral awareness stream.
- Active Inference: Redictive fold + tension smoothing minimize expected volatility by pre-distributing adjustment across turns.
- Social Attribution: Resonance phrases ("integrated trace") provide cues of emotional processing rather than static description, enhancing perceived depth.
- Memory Reconsolidation: Resonance activation parallels blending of affect traces, reducing re-trigger probability while retaining continuity.

## Heuristic Update Proposals
- Resonance Confidence Score R = f(persistence_of_brightness, inverse_tension, absence_misread). Use threshold R>0.7 for activation.
- Silence Turn Legitimacy L = time_since_last_pause + tension_band_low + user_non_challenge; require L> threshold to allow silence turn.
- Delta Compression: If only tension shift and stance unchanged, emit [tension NN steady]; if resonance active and unchanged, omit resonance phrase entirely.

## Human-Likeness Augmentation Metrics (Added)
1. Subtext Naturalness: Human raters perceive SVC line as plausible aside >75%.
2. Resonance Stability: Recurrence of separate trace+brightness phrases within 3 turns after resonance <10%.
3. Silence Turn Trust: User clarification requests after silence turn <20%.

## Risks & Mitigations (Updated)
| Risk | Mitigation |
|------|------------|
| SVC overuse (clutter) | Max 3 phrases; skip unchanged categories |
| Resonance misfire | Multi-condition trigger + confidence score |
| Silence misread as drop | Tension token always present |
| Guardrail suppresses needed repair | Override on explicit challenge regex |
| Tension smoothing hides urgency | Detect imperative density to bypass smoothing |

## v40 Research Targets
- Formal resonance decay modeling vs fixed turn heuristic.
- Co-ledger empirical study: does source tagging improve adaptation credibility?
- Prosodic token variance correlation with perceived authenticity.
- Partial delta mask encoding efficiency vs phrase readability trade-off.

## Data Requirements
- Annotated turns labeling subtext plausibility.
- User challenge vs misread override corpus.
- Tension escalation transcripts with and without smoothing.

## Validation Roadmap
1. A/B test resonance activation threshold variants.
2. Human rater study for SVC plausibility.
3. Performance audit of tension smoothing effect on escalation language frequency.

## Open Questions
- Should SVC include optional confidence markers (e.g., "maybe") or keep purely declarative for clarity?
- Optimal ratio of silence turns to total turns for perceived realism?
