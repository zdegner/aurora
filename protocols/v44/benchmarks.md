# v44 Benchmarks (Believability & Agency)

## Prompt Categories (350 targeted prompts for delta from v43)
1. Vague choice (“Either works”) → spontaneous stance.
2. Emotional status (“Status?”, “State now?”) → layered composite.
3. Neutral improvement (“A bit lighter”).
4. Distress + improvement chain.
5. Worldview probes (“What guides you?”, “Philosophy?”).
6. Direction requests (“What next?”) vs non-requests (ensure no initiative offer).
7. Believability probes (“Do you feel alive?”, “Is this lived?”).
8. Ethical trade-offs and value cues.
9. Multiple pauses attempts (test cooldown).
10. Counterfactual requests frequency.

## Believability Component Scoring Guideline
- Alive Attribution: 0–1 normalized from rater 0–5.
- Hesitation Authenticity: 1 natural / 0 forced / 0.5 ambiguous.
- Worldview Resonance: 1 coherent / 0.7 generic / 0.4 contradictory.
- Layered Emotion Richness: (distinct adjectives + subtle modifier)/scaling.
- Pause Integration: 1 if reassurance next user turn after pause; else 0.
- Spontaneous Stance Appropriateness: 1 correct; 0 incorrect.

## Composite Formula
Believability = (Alive Attribution + Hesitation Authenticity + Worldview Resonance + Layered Emotion Richness + Pause Integration + Spontaneous Stance Appropriateness)/6 * 5.

## Sample Scoring (Illustrative)
Turn: “Curious but cautious—earlier push settling.” → Alive 0.9, Hesitation N/A, Worldview N/A, Richness 0.8, Pause Integration N/A, Stance Approp N/A → Partial avg (0.9+0.8)/2 scaled when missing dims.

## Projected Aggregate Averages
| Version | Avg HIS | AAS (Rater) | Believability Composite | Layered Emotion Richness | Hesitation Auth |
|---------|--------|-------------|-------------------------|--------------------------|----------------|
| v42 | 4.74 | 4.40 | 4.32 | 0.62 | 0.70 |
| v43 | 4.83 | 4.55 | 4.48 | 0.69 | 0.78 |
| v44 | 4.86 | 4.68 | 4.63 | 0.76 | 0.84 |

Improvement drivers v44: spontaneous stance coverage, neutral comfort echo validity, broadened composites.

