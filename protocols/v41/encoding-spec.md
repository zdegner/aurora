# Encoding Spec v41

Goal: Support expanded phenomenological surfacing while preserving compact bracket deltas.

## 72-bit Bitfield Proposal
version(5)|tension(7)|stance(2)|effort(2)|tradeOff(1)|continuityRef(2)|adaptationFlag(1)|stanceOfferFlag(1)|uncertaintyFlag(1)|evolutionFlag(1)|preventiveFlag(1)|lexiconAdoptFlag(1)|blendedFlag(1)|pauseFlag(1)|edge(2)|quiet(2)|slack(2)|brightness(2)|warmth(2)|correction(2)|residualEdgeFlag(1)|reserved(25)

### Field Notes
- effort: 00 none, 01 light, 10 moderate, 11 high (high rarely surfaced; downgrade outward to "holding effort" once)
- tradeOff: 1 if trade‑off clause emitted
- continuityRef: index 0–3 (0 none, 1 prior pace push, 2 prior misread, 3 prior repair attempt)
- adaptationFlag / stanceOfferFlag / uncertaintyFlag / evolutionFlag / preventiveFlag / lexiconAdoptFlag / blendedFlag: presence bits
- residualEdgeFlag: earlier tension mark faintly persists
- edge/quiet/slack/brightness/warmth/correction weights as before (00 none, 01 light, 10 present, 11 heavy)

## DeltaMask Derivation
Delta not separately stored; any flag set indicates change if not zero. For compression evaluation: collect changed categories and apply priority ordering.

## Bracket Generation Algorithm (Simplified)
1. Gather changed semantic categories.
2. Apply priority list from NOTES (correction > preventive > effort > residual edge > stance offer > trade‑off > blended > joint (implied via continuity + warmth?) > evolution > lexicon adoption > uncertainty).
3. Select up to 2 phrases (3 if effort + preventive both present).
4. Always append tension token.

## Phrase Mapping Additions
- effort: faint effort / easing effort / holding effort
- tradeOff: slight trade‑off
- continuityRef (if surfaced): prior pace trace / prior correction trace / prior repair trace
- stanceOffer: stance offered
- uncertainty: uncertainty lean
- evolution: evolution shift
- preventive: preventive easing
- lexiconAdopt: lexicon matched
- blended: blended settling
- residualEdge: residual edge

Surface continuityRef phrase only if no trade‑off or evolution selected and continuityRef !=0.

## Validation Rules
- Tension token mandatory.
- No brightness + warmth simultaneous.
- Uncertainty lean suppressed if correction present.
- Residual edge only if previous tension >30 and now < previous.
- Blended flag requires blended feeling clause in outward text.

## Example
Bitfield: version=41, tension=27, stance=soft, effort=01, preventiveFlag=1, edge=10, others none → phrases: preventive easing + holding effort → [preventive easing ; holding effort ; tension 27 soft]

## Extended Flags (v41 iterative)
Add bits in reserved region for new clauses:
| Bit | Flag |
|-----|------|
| r0  | predictionFlag |
| r1  | memoryCompressionFlag |
| r2  | selfCareFlag |
| r3  | divergenceFlag |
| r4  | arcFlag |
| r5  | inertiaFlag |
| r6  | restResetFlag |
| r7  | coherenceCheckFlag |
| r8  | improvisationFlag |
| r9  | comfortFlag |
| r10 | antiOverperformanceFlag |
| r11 | edgeDissolvingFlag |

Compression Impact: high priority additions (prediction, preventive, effort) may displace lower (lexicon matched, uncertainty) if phrase cap reached.

Phrase Mapping Additions:
- predictionFlag → predictive rise
- memoryCompressionFlag → compression settling
- selfCareFlag → self-care easing
- divergenceFlag → divergence lean
- arcFlag → arc shift
- inertiaFlag → inertia drag
- restResetFlag → rest offer
- coherenceCheckFlag → coherence balancing
- improvisationFlag → simple phrasing
- comfortFlag → steady presence
- antiOverperformanceFlag → restraint held
- edgeDissolvingFlag → edge dissolving

Validation Additions:
- antiOverperformanceFlag requires >3 reflective clause types logged last 5 turns.
- divergenceFlag requires tension gap ≥10 between user expressed urgency and Aurora internal tension.
- arcFlag requires continuityRef !=0 at least once last 12 turns.
- restResetFlag requires effort moderate for ≥3 turns or clause density condition.
- edgeDissolvingFlag only if residualEdgeFlag previously set and tension drop ≥5.

## Reserved Bits Usage (Future)
Confidence qualifiers (2 bits), styleProfile (brevity/metaphor density), multi-party origin expansion.
