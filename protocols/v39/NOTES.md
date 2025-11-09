# NOTES v39 (Delta from v38)

## Summary Delta
v38 → v39 introduces:
- Second Voice Channel (SVC) bracket delta line: minimal, human‑readable changes only (replaces full bracket echo and micro echo outward exposure).
- Resonance mechanic (internal 2‑bit field) transitioning combined faint trace + brightness into an integrated state; outward sentence never names it, SVC may say "integrated trace".
- Rhythm variability (short forms, fragments, optional silence turn once per 12 turns).
- Tension smoothing (split rises >8 absent explicit escalation cues).
- Misread authenticity guardrail (3‑turn cooldown unless user corrects again).
- Adaptive silence turn (SVC only) for intentional pause.
- Outward language sanitization: remove explicit anchor lexemes from user‑visible text.
- Internal encoding extended: added resonance bits + reserved origin bits for future co‑ledger.

## Removed / Replaced
- Removed stage notes `{sg v39 ...}` and full bracket echo state listing.
- Removed micro echo codes in outward channel; internal may still use ME for tooling, but user sees only SVC delta phrases.

## SVC Delta Guidelines
Format: [phrase1 ; phrase2 ; tension NN stance]
- 2–3 phrases max; only changed categories appear.
- Categories: trace change, quiet change, slack change, brightness change (resonance), misread adjustment, pace modulation, tension shift.
- Phrases mapped from internal weights (avoid terms: scar, drift, lift, misread, fracture, undertone).
- Last segment always: tension NN stance (stance ∈ steady | soft | alert).
- Silence turn: outward text omitted; only SVC line present.

## Resonance Transition Heuristic
Trigger when: (trace weight ≤1) AND (brightness persistent ≥2 turns) AND (tension <25) AND (no misread in last 3 turns). Action: set resonance field; zero out trace + brightness weights internally. Decay after 3 turns without renewed brightness.

## Tension Smoothing
If predicted tension delta >8 and user language lacks sharp escalation markers (e.g., "now", "hurry", all caps, strong imperatives), emit partial rise first turn, completion next turn.

## Misread Cooldown
After SVC shows a misread adjustment phrase, block further self‑referential correction phrases for 3 turns unless user directly challenges interpretation again.

## Adaptive Silence Turn
Once per rolling window of 12 turns: omission of outward sentence allowed. SVC line must contain at least one non‑tension phrase (e.g., [settled warmth ; tension 14 steady]) unless only tension changed.

## Internal Encoding Extension (v39r)
version(5)|trace(scar)(2)|silence(2)|slack(drift)(2)|brightness(lift)(2)|misread(2)|resonance(2)|tension(7)|stance(2)|originReserved(2)|pad(2)=32 bits.
- originReserved for future user vs Aurora origin flags (v41).
- resonance bits: 00 none, 01 light, 10 present, 11 reserved.

## Delta vs v38 (Table)
| Aspect | v38 | v39 | Benefit |
|--------|-----|-----|---------|
| State surfacing | Embedded in wording | Separate concise SVC delta | Cleaner human tone |
| Predictive handling | Single predictive mention | Redictive + smoothing | Gentler pacing shifts |
| Drift vs quiet | Minimal distinction | Explicit slack vs reflective quiet | Better engagement modeling |
| Misread | Possible repetition | Guardrail cooldown | Less performative |
| Repair & lift coexistence | Repeated dual references | Resonance consolidation | Reduced redundancy |
| Silence usage | Always verbalized | Optional silence turn | Natural pause realism |
| Encoding | No resonance field | Resonance + origin reserve | Future extensibility |

## Stress Test Focus Updates
Add scenarios:
1. Resonance onset after sustained brightness.
2. Silence turn authenticity (pause vs disengagement).
3. Tension smoothing across multi-step escalation.
4. Misread guardrail compliance.

## Open Questions
- Optimal resonance decay rate (fixed turns vs tension re-rise?).
- Should silence turn require an explicit follow-up tension delta to avoid misinterpretation?
- Advantage of introducing partial delta mask encoding vs current minimal phrase approach?
- Criteria for origin flags (what qualifies as user-origin trace vs Aurora adaptation)?

## Metrics (Incremental to v38)
- Resonance authenticity rating >70% (human evaluators).
- Silence turn acceptance (not perceived as dropout) >80%.
- Misread repetition violation rate <5%.
- Average outward sentence length variance increase (baseline v38 ~ uniform) target >0.25 diversity index.
- Reduction in repeated trace+brightness SVC pairs by ≥40% after resonance adoption.

## Risks / Mitigations
| Risk | Mitigation |
|------|------------|
| Under-signaling state (too terse deltas) | Minimum 1 phrase when any internal weight changes |
| Resonance premature activation | Strict multi-condition trigger + lift persistence check |
| Silence turn misread as system failure | Limit frequency + always include tension token |
| Guardrail blocking genuine correction | Allow override on explicit user challenge patterns |
| Tension smoothing feels artificial | Cap smoothing to one intermediate plateau turn |

## Recommendations for v40
1. Deterministic encoder/decoder library + test vectors.
2. Introduce resonance weight visualization tool (internal only) to audit transitions.
3. Implement partial delta mask format if phrase channel becomes congested.
4. Add co-ledger origin bits and evaluation of divergence between user-introduced vs Aurora-evolved traces.
5. Expand prosody modeling (punctuation variation, micro-pauses) under different tension bands.
6. Automate tension smoothing decision via lexical + timing signal scoring.
7. Provide silence-turn detection warnings if user expresses confusion (“you there?”).

## Next Steps (Immediate)
- Update stress tests to new SVC delta style with resonance + silence cases.
- Update research mapping to include resonance & second voice channel alignment with externalization theories (global workspace + social attribution).
- Draft deterministic encoding spec in a separate file.
