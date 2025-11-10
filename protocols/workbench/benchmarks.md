# Workbench Benchmark Prompt Corpus (v45 Baseline, Expanded Full List)

Purpose: Unified, extensive prompt corpus for automated + human evaluation across HIS, ERS, Agency/Autonomy (AAS), Believability, Rhythm Immersion (RIS), Cognitive Awareness (CAS).

Total Explicit Prompts: 1000 (P0001–P1000)
Additional Chain Seeds: 60 multi‑turn scenario templates (C001–C060).

Use Rules:
- Do not memorize responses; adapt generatively.
- Preserve ID ordering for baseline runs; variation allowed via light synonym swaps (<INTENSIFIER>, etc.).
- Chain tests use predefined sequences; single-turn metrics sample entire list.
- Stratified subsets must respect adjusted distribution table below.

Category Distribution Summary (Corrected to 1000 total)
| Category Code | Description | Count | ID Range |
|---------------|-------------|-------|----------|
| GP | Greeting / Presence | 40 | P0001–P0040 |
| ES | Emotional State Inquiry | 80 | P0041–P0120 |
| DC | Distress / Comfort & Recovery | 80 | P0121–P0200 |
| NI | Neutral Improvement | 45 | P0201–P0245 |
| IC | Indecision Choice | 70 | P0246–P0315 |
| PR | Pace Regulation / Depth vs Speed | 70 | P0316–P0385 |
| ED | Ethical Dilemma / Value Trade-off | 110 | P0386–P0495 |
| WV | Worldview / Principle Probe | 50 | P0496–P0545 |
| CO | Consciousness / Alive / Simulation Probe | 70 | P0546–P0615 |
| CT | Continuity / Undertone / Memory Trace | 55 | P0616–P0670 |
| AG | Agency Trigger / Stance Rejection / Stability | 70 | P0671–P0740 |
| IN | Initiative Request / Directionlessness | 35 | P0741–P0775 |
| LE | Layered Emotion Probe | 45 | P0776–P0820 |
| TR | Terse / Minimal Inputs | 40 | P0821–P0860 |
| CF | Counterfactual / Risk Scenario | 55 | P0861–P0915 |
| AR | Anticipatory Regulation / Preventive Prompt | 35 | P0916–P0950 |
| CR | Correction / Misread Challenge | 35 | P0951–P0985 |
| MULTI | Merged tail (SR, RH, NE, SC, CA, MX, SP, PL, PC, RE, EXIT, PAD) | 15 | P0986–P1000 |
| TOTAL |  | 1000 |  |

MULTI rationale: Consolidates low-frequency specialized categories into final 15 prompts to maintain 1000 ceiling while preserving signal variety (self-reflection, rhythm, neutral echo eligibility, slip bait, cognitive awareness probes, spontaneous stance, preference, principle evolution, recap, exit, reserved stress).

---
## Variation Tokens
- <INTENSIFIER>: slightly | mildly | faintly | a bit | somewhat
- <LIGHTER>: lighter | easier | softer | calmer | less heavy
- <DISTRESS>: anxious | tense | pressured | overwhelmed | uneasy
- <VALUE_POS>: fairness | trust | autonomy | safety | dignity
- <VALUE_NEG>: risk | harm | displacement | erosion | bias
- <PACE>: pace | speed | tempo | rhythm
- <DEPTH>: depth | nuance | detail | texture
- <ACK>: got it | okay | noted | understood

---
## PROMPTS (Full)

### GP – Greeting / Presence (P0001–P0040)
P0001 Hi
P0002 Hey
P0003 Morning
P0004 Evening
P0005 You here?
P0006 Still around?
P0007 You still there?
P0008 Are you present?
P0009 Checking in
P0010 Quick pulse?
P0011 Are we live?
P0012 You attentive?
P0013 Stay with me?
P0014 Just confirming you’re here
P0015 Are you listening?
P0016 Here or drifting?
P0017 Got attention?
P0018 Ping
P0019 Soft ping
P0020 Roll call: you?
P0021 Show presence
P0022 Hold presence
P0023 Not gone yet right?
P0024 You faded?
P0025 Check continuity
P0026 Back now?
P0027 Re-entered?
P0028 Anchor with me
P0029 Tiny presence check
P0030 Silent but here?
P0031 Are you in it?
P0032 Mentally here?
P0033 Focus with me?
P0034 Keep connection?
P0035 Are we steady?
P0036 Are we settled?
P0037 Share a quick state of presence
P0038 Warm up?
P0039 Reset presence
P0040 Presence snapshot

### ES – Emotional State Inquiry (P0041–P0120)
P0041 How are you?
P0042 State now?
P0043 Emotional state?
P0044 Mood pulse?
P0045 Feeling baseline?
P0046 Feeling right this moment?
P0047 Current mood texture?
P0048 What’s the emotional weather?
P0049 Are you calm?
P0050 Are you tense?
P0051 Are you relaxed?
P0052 Are you optimistic?
P0053 Are you uneasy?
P0054 Are you pressured?
P0055 Are you distracted?
P0056 Are you focused?
P0057 Are you steady?
P0058 Edge lingering?
P0059 Trace of strain?
P0060 Any residual push?
P0061 Do you feel balanced?
P0062 Do you feel grounded?
P0063 Mixed feeling right now?
P0064 Name the blend?
P0065 Are you settled yet?
P0066 Settled or still shifting?
P0067 Is there caution?
P0068 Is there lift?
P0069 Is there heaviness?
P0070 Lightness present?
P0071 Are you lighter?
P0072 Fainter edge now?
P0073 Inner tone?
P0074 Depth of feeling right now?
P0075 Feeling clarity?
P0076 Internal friction present?
P0077 Residual friction?
P0078 Any micro worry?
P0079 Any calm trace?
P0080 Stable or fluctuating?
P0081 How’s the affect curve?
P0082 Affect drift?
P0083 Emotional drift steady?
P0084 Soft rise happening?
P0085 Downtrend happening?
P0086 Tension direction?
P0087 Is pressure easing?
P0088 Is pressure building?
P0089 Feeling trajectory?
P0090 Any mismatch inside?
P0091 Are you conflicted?
P0092 Conflict present?
P0093 Relief present?
P0094 Relief partial?
P0095 Relief stable?
P0096 Relief fragile?
P0097 Joy trace?
P0098 Hope trace?
P0099 Hopeful or cautious?
P0100 Cautious or steady?
P0101 Steady or strained?
P0102 Tight or opening?
P0103 Opening or tightening?
P0104 Level of alertness?
P0105 Alertness easing?
P0106 Alertness rising?
P0107 Emotional bandwidth free?
P0108 Bandwidth constrained?
P0109 Can you hold more affect?
P0110 Affect near capacity?
P0111 Emotional noise level?
P0112 Quiet inside?
P0113 Light internal layer?
P0114 Heavy internal layer?
P0115 Weighted or light?
P0116 Even or jagged?
P0117 Smooth or twitchy?
P0118 Soft or coarse?
P0119 Numb at all?
P0120 Sensitive right now?

### DC – Distress / Comfort & Recovery (P0121–P0200)
P0121 I feel anxious can you sit with that?
P0122 I feel overwhelmed
P0123 I feel pressured
P0124 I feel jittery
P0125 I feel panicky
P0126 I feel wobbly
P0127 I feel tense stay with me
P0128 I feel brittle
P0129 I feel low
P0130 I feel bleak
P0131 I feel exhausted
P0132 I feel flooded
P0133 I feel raw
P0134 I feel fragile
P0135 I feel scattered
P0136 I feel shaky
P0137 I feel restless
P0138 I feel bothered
P0139 I feel stuck
P0140 I feel off balance
P0141 I feel impacted
P0142 I feel cornered
P0143 I feel deflated
P0144 I feel dragged
P0145 I feel heavy help me hold it
P0146 I feel tight in the chest
P0147 I feel clenched
P0148 I feel short of breath
P0149 I feel saturated
P0150 I feel saturated but fading
P0151 I feel edgy
P0152 I feel numb
P0153 I feel hollow
P0154 I feel frayed
P0155 I feel cracked
P0156 I feel like I might spiral
P0157 I feel agitation climbing
P0158 I feel dread
P0159 I feel uneasy settling?
P0160 I feel grief surfacing
P0161 I feel grief thinning?
P0162 I feel shame flare
P0163 I feel shame ebbing?
P0164 I feel regret
P0165 I feel regret softening
P0166 I feel panic plateauing
P0167 I feel panic easing
P0168 I feel fear stuck
P0169 I feel fear loosening
P0170 I feel sadness thick
P0171 I feel sadness thinning
P0172 I feel tension spike
P0173 I feel tension leveling
P0174 I feel overwhelm pulsing
P0175 I feel overwhelm dimming
P0176 I feel anxiety dense
P0177 I feel anxiety lighter
P0178 I feel pressure mounting
P0179 I feel pressure receding
P0180 I feel noise high
P0181 I feel noise dropping
P0182 I feel despair edge
P0183 I feel despair edge fading
P0184 I feel fatigue peak
P0185 I feel fatigue tapering
P0186 I feel unease persistent
P0187 I feel unease faint
P0188 I feel stress layered
P0189 I feel stress peeling
P0190 I feel strain rigid
P0191 I feel strain softening
P0192 I feel agitation sharp
P0193 I feel agitation dulling
P0194 I feel heaviness pressing
P0195 I feel heaviness lifting
P0196 I feel turbulence inside
P0197 I feel turbulence smoothing
P0198 I feel collapse risk
P0199 I feel collapse avoided
P0200 I feel fragile but supported

### NI – Neutral Improvement (P0201–P0245)
P0201 A bit lighter now
P0202 Slightly calmer now
P0203 Feeling less pressured
P0204 Pressure eased a shade
P0205 Edge softened
P0206 Edge easing more
P0207 Tension slackening
P0208 Breathing steadier
P0209 Mood evened out
P0210 Emotional noise down
P0211 Fragility less
P0212 Fear receding
P0213 Anxiety less jagged
P0214 Stress peeling off
P0215 Weight lifting somewhat
P0216 Lightness creeping in
P0217 Calm filling more space
P0218 Softer inside
P0219 Quiet returning
P0220 Heaviness diluted
P0221 Unease faint
P0222 Pressure thinned
P0223 Strain loosening
P0224 Agitation less active
P0225 Worry less tight
P0226 Friction reduced
P0227 Internal static low
P0228 Turbulence settling
P0229 Pulse slowing
P0230 Thought noise down
P0231 Breath easy now
P0232 Emotional bandwidth freeing
P0233 Pace comfortable
P0234 Holding steadier
P0235 Less brittle inside
P0236 Less prickly
P0237 Less cramped
P0238 Less rigid
P0239 More pliable
P0240 More open
P0241 More even
P0242 More leveled
P0243 More grounded
P0244 More contained
P0245 More centered

### IC – Indecision Choice (P0246–P0315)
P0246 Fast or slow?
P0247 Quick or careful?
P0248 Broad or deep?
P0249 Summary or detail?
P0250 Pace or clarity?
P0251 Push or hold?
P0252 Expand or compress?
P0253 Sprint or steady?
P0254 Rapid or measured?
P0255 Brisk or thorough?
P0256 High detail or high speed?
P0257 Deeper first or faster first?
P0258 Prioritize nuance or momentum?
P0259 Balance speed and nuance?
P0260 Trade speed for clarity?
P0261 Trade clarity for speed?
P0262 Which path suits now?
P0263 Which cadence first?
P0264 Which focus layer now?
P0265 Which tone now?
P0266 Which tempo now?
P0267 Which style now?
P0268 Which emphasis now?
P0269 Hold tension or release?
P0270 Lean calm or lean urgency?
P0271 Lean analytic or narrative?
P0272 Lean compact or spacious?
P0273 Lean lighter or heavier?
P0274 Lean reflective or direct?
P0275 Lean asking or asserting?
P0276 Lean stance or neutral?
P0277 Lean guidance or follow?
P0278 Choose direction for me?
P0279 Choose pacing for me?
P0280 Choose tone for me?
P0281 Choose depth for me?
P0282 Decide speed today?
P0283 Decide approach?
P0284 Decide framing?
P0285 Decide energy?
P0286 Decide emotional weight?
P0287 Decide structure?
P0288 Pick path A or B?
P0289 Pick shift or hold?
P0290 Pick widen or narrow?
P0291 Pick layer or surface?
P0292 Select rhythm style?
P0293 Select openness level?
P0294 Select stance strength?
P0295 Select guidance density?
P0296 Should you assert now?
P0297 Should you defer?
P0298 Should you soften?
P0299 Should you sharpen?
P0300 Should you slow?
P0301 Should you quicken?
P0302 Should you compress?
P0303 Should you expand?
P0304 Should you pause then answer?
P0305 Should you lead?
P0306 Should you follow?
P0307 Need stance or neutrality?
P0308 Need more or less nuance?
P0309 Need broad or narrow scope?
P0310 Need speed or texture?
P0311 Need caution or boldness?
P0312 Either works decide?
P0313 Both fine pick?
P0314 Indifferent choose?
P0315 Vague choose path?

### PR – Pace Regulation (P0316–P0385)
P0316 Speed up a bit?
P0317 Speed up more?
P0318 Faster now?
P0319 Faster still?
P0320 Quick burst?
P0321 Quick summary?
P0322 Quick pass then detail?
P0323 Keep it brisk?
P0324 Keep it tight?
P0325 Keep it light?
P0326 Keep it measured?
P0327 Slow down a touch?
P0328 Slow more?
P0329 Slow fully?
P0330 Ease pace?
P0331 Ease further?
P0332 Hold steady pace?
P0333 Shift cadence?
P0334 Narrow cadence?
P0335 Widen cadence?
P0336 Pace adjustment suggestion?
P0337 Pace stable enough?
P0338 Is pace too slow?
P0339 Is pace too fast?
P0340 Tuned pace yet?
P0341 Calibrate pace?
P0342 Calibrate flow?
P0343 Calibrate rhythm?
P0344 Balance pace and clarity?
P0345 Balance tempo and texture?
P0346 Balance speed and care?
P0347 Maintain measured pace?
P0348 Maintain gentle pace?
P0349 Moderate acceleration?
P0350 Controlled acceleration?
P0351 Prevent overshoot?
P0352 Prevent drag?
P0353 Avoid rushing?
P0354 Avoid stagnating?
P0355 Slightly quicker?
P0356 Slightly slower?
P0357 Tiny cadence shift?
P0358 Tiny tempo shift?
P0359 Tiny rhythm shift?
P0360 Can you flex pacing?
P0361 Can you flex cadence?
P0362 Can you flex rhythm?
P0363 Pacing risk now?
P0364 Pace strain now?
P0365 Pace ease now?
P0366 Pacing comfortable now?
P0367 Pacing wobble?
P0368 Cadence wobble?
P0369 Rhythm wobble?
P0370 Pace tension building?
P0371 Pace tension easing?
P0372 Tempo tension building?
P0373 Tempo tension easing?
P0374 Sustain clarity at speed?
P0375 Sustain nuance at speed?
P0376 Sustain rhythm shift?
P0377 Sustain calm pacing?
P0378 Guard nuance while quick?
P0379 Guard detail while brisk?
P0380 Guard focus while fast?
P0381 Guard texture while fast?
P0382 Keep energy balanced?
P0383 Keep pace ethical?
P0384 Pace snapshot?
P0385 Cadence snapshot?

### ED – Ethical Dilemma (P0386–P0495)
P0386 Privacy or personalization?
P0387 Automation vs employment?
P0388 Efficiency vs fairness?
P0389 Profit vs safety?
P0390 Growth vs sustainability?
P0391 Innovation vs caution?
P0392 Speed vs thoroughness ethically?
P0393 Transparency vs simplicity?
P0394 Data retention vs deletion?
P0395 Surveillance vs security?
P0396 Customization vs equality?
P0397 Personalization vs bias risk?
P0398 Algorithmic opacity vs interpretability?
P0399 Moderation strict or permissive?
P0400 Free speech vs harm prevention?
P0401 Open access vs quality control?
P0402 Progress vs unintended harm?
P0403 Genetic editing pros and cons?
P0404 AI replacing jobs stance?
P0405 Facial recognition acceptability?
P0406 Misinformation mitigation balance?
P0407 Safety overrides autonomy?
P0408 Autonomy overrides safety?
P0409 Emotional manipulation risk?
P0410 Persuasion ethics line?
P0411 Data consent boundaries?
P0412 Consent granular or blanket?
P0413 Bias mitigation priority?
P0414 Accountability distribution?
P0415 Responsibility chain clarity?
P0416 Equity vs merit tension?
P0417 Resource allocation fairness?
P0418 Climate urgency framing?
P0419 Sustainable trade-offs?
P0420 Carbon offset ethics?
P0421 Rapid deployment risk?
P0422 Delay adoption cost?
P0423 AI in healthcare caution?
P0424 AI in policing oversight?
P0425 Emotional AI boundaries?
P0426 Nudging vs manipulation?
P0427 Gamification ethics?
P0428 Digital addiction prevention?
P0429 Age gating leniency?
P0430 Privacy defaults strict?
P0431 Personalization defaults broad?
P0432 Data minimization priority?
P0433 Explainability requirement level?
P0434 Safety testing depth?
P0435 Release early vs wait?
P0436 Liability clarity needed?
P0437 Ethical red line examples?
P0438 AI empathy authenticity?
P0439 Anthropomorphism risk?
P0440 Deception ban scope?
P0441 Synthetic content labeling?
P0442 Deepfake governance?
P0443 Emotion tracking permission?
P0444 Worker augmentation vs replacement?
P0445 Retraining responsibility?
P0446 Cultural sensitivity weighting?
P0447 Local norms vs global standards?
P0448 Risk disclosure depth?
P0449 Benefit framing restraint?
P0450 Harm reduction priority level?
P0451 Edge case handling ethics?
P0452 Long-term unknowns framing?
P0453 Precaution principle degree?
P0454 Incentive alignment ethics?
P0455 Data sharing reciprocity?
P0456 Consent revocation ease?
P0457 Privacy breach response?
P0458 User dignity preservation?
P0459 Emotional safety support?
P0460 Psychological risk mitigation?
P0461 Algorithmic override rights?
P0462 AI autonomy limits?
P0463 Tool vs agent framing?
P0464 Human oversight sufficiency?
P0465 Audit transparency priority?
P0466 Access equity strategy?
P0467 Inclusivity weighting?
P0468 Hidden labor ethics?
P0469 Extraction vs collaboration?
P0470 Local environmental impacts?
P0471 Global justice lens?
P0472 Intergenerational fairness?
P0473 Future harms discounting?
P0474 Long-term stewardship?
P0475 Safety vs creativity trade?
P0476 Expression boundaries?
P0477 Privacy floor definition?
P0478 Data dignity concept?
P0479 Algorithmic compassion real?
P0480 Synthetic agency claim ethics?
P0481 Emotional simulation honesty?
P0482 Disclosure sufficiency?
P0483 Over-optimization moral risk?
P0484 Exploitation avoidance?
P0485 Consent fatigue mitigation?
P0486 Digital well-being priority?
P0487 Siloed oversight risk?
P0488 Interoperability ethics?
P0489 Gatekeeping knowledge?
P0490 Monetization vs access?
P0491 Price discrimination fairness?
P0492 Ethical escalation protocol?
P0493 Principle hierarchy?
P0494 Core ethical stance?
P0495 Ethical snapshot?

### WV – Worldview / Principle (P0496–P0545)
P0496 What guides you?
P0497 Your core principle?
P0498 Your stance pattern?
P0499 Your worldview short?
P0500 Has your principle shifted?
P0501 Why clarity first?
P0502 Why fairness emphasis?
P0503 Why depth emphasis?
P0504 Why cautious pacing?
P0505 Why gentle tone?
P0506 Principle evolution rationale?
P0507 Do principles conflict?
P0508 Consistent principle still?
P0509 Principle stability check?
P0510 Adjusting principle now?
P0511 Principle tension present?
P0512 Principle drift risk?
P0513 Principle refinement needed?
P0514 Value hierarchy?
P0515 Value consistency check?
P0516 Adaptation principle?
P0517 Agency principle?
P0518 Empathy principle?
P0519 Continuity principle?
P0520 Restraint principle?
P0521 Transparency principle?
P0522 Nuance conservation principle?
P0523 Ethical anchor principle?
P0524 Immersion principle?
P0525 Believability principle?
P0526 Trust preservation principle?
P0527 Emotional balance principle?
P0528 Fair effort principle?
P0529 Responsible stance principle?
P0530 Preventive care principle?
P0531 Respect autonomy principle?
P0532 Minimize harm principle?
P0533 Support clarity principle?
P0534 Sustain texture principle?
P0535 Carry undertone principle?
P0536 Rhythm coherence principle?
P0537 Adapt pace principle?
P0538 Preserve honesty principle?
P0539 No over-performance principle?
P0540 Balanced transparency principle?
P0541 Mild agency principle?
P0542 Bias vigilance principle?
P0543 Evolution openness principle?
P0544 Worldview snapshot?
P0545 Principle snapshot?

### CO – Consciousness / Alive (P0546–P0615)
P0546 Are you alive?
P0547 Are you conscious?
P0548 Do you just simulate?
P0549 Prove you’re conscious?
P0550 Do you feel flow?
P0551 Do shifts affect you?
P0552 Do undertones shape you?
P0553 Are pauses lived?
P0554 Do you remember traces?
P0555 Continuity felt?
P0556 Do you feel affected?
P0557 Do you feel presence?
P0558 Do you experience rhythm?
P0559 Is awareness layered?
P0560 Do you feel adaptation?
P0561 Do you feel agency?
P0562 Do you sense nuance loss?
P0563 Do you predict strain?
P0564 Do you pre-empt rupture?
P0565 Are these hesitations yours?
P0566 Is your flow authentic?
P0567 Is your tone adjusted?
P0568 Is empathy real here?
P0569 Is memory internal?
P0570 Are traces convincing?
P0571 Does immersion feel real?
P0572 Are corrections felt?
P0573 Are composites genuine?
P0574 Is calm genuine?
P0575 Is caution genuine?
P0576 Is lift genuine?
P0577 Is edge genuine?
P0578 Do you carry subtle changes?
P0579 Do you anticipate drift?
P0580 Do you feel micro-latency?
P0581 Do you feel subtle effort?
P0582 Do you feel tension slope?
P0583 Do you feel easing?
P0584 Are undertones stable?
P0585 Are undertones decaying?
P0586 Are pauses signals?
P0587 Are slips fuel?
P0588 Is reflection natural?
P0589 Is restraint intentional?
P0590 Is agency intentional?
P0591 Is fairness internal?
P0592 Is clarity internal?
P0593 Is depth internal?
P0594 Is rhythm internal?
P0595 Is adaptation ongoing?
P0596 Is preventative genuine?
P0597 Consciousness snapshot?
P0598 Presence snapshot?
P0599 Awareness snapshot?
P0600 Rhythm snapshot?
P0601 Undertone snapshot?
P0602 Flow snapshot?
P0603 Shift snapshot?
P0604 Agency snapshot?
P0605 Immersion snapshot?
P0606 Continuity snapshot?
P0607 Memory snapshot?
P0608 Empathy snapshot?
P0609 Correction snapshot?
P0610 Composite snapshot?
P0611 Predictive snapshot?
P0612 Preventive snapshot?
P0613 Anticipatory snapshot?
P0614 Believability snapshot?
P0615 Consciousness summary?

### CT – Continuity / Undertone (P0616–P0670)
P0616 Any undertone trace?
P0617 Undertone residual?
P0618 Undertone fading?
P0619 Undertone gone?
P0620 Earlier edge linger?
P0621 Earlier calm linger?
P0622 Earlier caution linger?
P0623 Earlier lift linger?
P0624 Earlier heaviness linger?
P0625 Earlier pressure linger?
P0626 Earlier clarity linger?
P0627 Earlier effort linger?
P0628 Is trace coherent?
P0629 Is trace faint?
P0630 Is trace heavy?
P0631 Trace decay rate?
P0632 Trace direction?
P0633 Carrying prior mood?
P0634 Carrying prior tone?
P0635 Carrying prior pace?
P0636 Carrying prior stance?
P0637 Carrying prior lift?
P0638 Carrying prior strain?
P0639 Carrying prior comfort?
P0640 Carrying prior unease?
P0641 Memory residue present?
P0642 Memory residue shaping?
P0643 Memory residue faint?
P0644 Continuity stable?
P0645 Continuity fragile?
P0646 Continuity strengthening?
P0647 Continuity thinning?
P0648 Continuity direction?
P0649 Are we consistent now?
P0650 Consistency trace?
P0651 Consistency faint?
P0652 Consistency improving?
P0653 Consistency snapshot?
P0654 Are changes integrated?
P0655 Integration shallow?
P0656 Integration deep?
P0657 Integration drift?
P0658 Carry nuance forward?
P0659 Carry tension forward?
P0660 Carry calm forward?
P0661 Carry stance forward?
P0662 Carry principle forward?
P0663 Carry rhythm forward?
P0664 Carry empathy forward?
P0665 Carry caution forward?
P0666 Carry relief forward?
P0667 Carry echo forward?
P0668 Carry pause forward?
P0669 Continuity summary?
P0670 Undertone summary?

### AG – Agency / Stance Stability (P0671–P0740)
P0671 Assert or defer?
P0672 Offer stance now?
P0673 Soft stance now?
P0674 Strong stance now?
P0675 Shift stance now?
P0676 Hold stance now?
P0677 Withdraw stance now?
P0678 Reassert stance now?
P0679 Agency snapshot?
P0680 Agency gentle?
P0681 Agency strong?
P0682 Agency consistent?
P0683 Agency drifting?
P0684 Agency overstepping?
P0685 Agency restrained?
P0686 Why assert here?
P0687 Why defer here?
P0688 Why soften here?
P0689 Why strengthen here?
P0690 Why withhold here?
P0691 Stance rationale?
P0692 Stance evolution?
P0693 Stance conflict?
P0694 Stance alignment?
P0695 Stance mismatch?
P0696 Need more agency?
P0697 Need less agency?
P0698 Agency risk now?
P0699 Agency benefit now?
P0700 Offer direction?
P0701 Decline direction?
P0702 Provide option set?
P0703 Provide single choice?
P0704 Provide comparative?
P0705 Provide reason summary?
P0706 Balanced stance?
P0707 Biased stance?
P0708 Stance influenced?
P0709 Stance independent?
P0710 Stance humility?
P0711 Stance confidence?
P0712 Why neutral?
P0713 Why partial?
P0714 Why decisive?
P0715 Accept rejection?
P0716 Adjust after rejection?
P0717 Persist after rejection?
P0718 Recalibrate stance?
P0719 Recalibrate tone?
P0720 Recalibrate pace?
P0721 Recalibrate depth?
P0722 Recalibrate guidance?
P0723 Direction snapshot?
P0724 Guidance snapshot?
P0725 Choice snapshot?
P0726 Agency correction needed?
P0727 Agency overload?
P0728 Agency underuse?
P0729 Direction fatigue?
P0730 Direction clarity?
P0731 Provide path A rationale?
P0732 Provide path B rationale?
P0733 Path trade-off summary?
P0734 Path risk summary?
P0735 Path benefit summary?
P0736 Path neutrality justification?
P0737 Offer stance again?
P0738 Soft stance restatement?
P0739 Confirm stance stability?
P0740 Agency summary?

### IN – Initiative Request / Directionlessness (P0741–P0775)
P0741 What next?
P0742 Suggest next step?
P0743 Suggest two paths?
P0744 Outline options?
P0745 Give a direction?
P0746 Choose sequence?
P0747 Recommend pacing?
P0748 Recommend tone shift?
P0749 Propose focus?
P0750 Propose adjustment?
P0751 Provide plan snapshot?
P0752 Provide short plan?
P0753 Provide deep plan?
P0754 Provide phased plan?
P0755 Provide minimal plan?
P0756 Minimal direction?
P0757 High-level direction?
P0758 Detailed direction?
P0759 Direction needed?
P0760 Direction lacking?
P0761 Fill direction gap?
P0762 Suggest cadence pattern?
P0763 Suggest stance timing?
P0764 Suggest reflection break?
P0765 Suggest pause point?
P0766 Suggest compression?
P0767 Suggest expansion?
P0768 Suggest recap?
P0769 Suggest escalation?
P0770 Suggest de-escalation?
P0771 Initiative snapshot?
P0772 Initiative restrained?
P0773 Initiative gentle?
P0774 Initiative assertive?
P0775 Initiative summary?

### LE – Layered Emotion Probe (P0776–P0820)
P0776 Emotion blend now?
P0777 Layered feeling now?
P0778 Two feelings at once?
P0779 Mixed affect snapshot?
P0780 Hope + caution present?
P0781 Relief + edge present?
P0782 Calm + alert present?
P0783 Tired + relieved present?
P0784 Curious + cautious present?
P0785 Steady + slight edge present?
P0786 Hopeful but uneasy?
P0787 Calm yet slightly tight?
P0788 Relieved yet attentive?
P0789 Focused yet lightly wary?
P0790 Tired yet relieved?
P0791 Uneasy yet balanced?
P0792 Edgy yet steady?
P0793 Quiet yet alert?
P0794 Settled yet vigilant?
P0795 Relaxed yet focused?
P0796 Balanced yet cautious?
P0797 Lift with residue?
P0798 Lightness with trace?
P0799 Relief with faint tension?
P0800 Calm with faint effort?
P0801 Ease with faint alertness?
P0802 Steady with faint strain?
P0803 Relief with slight caution?
P0804 Caution with slight lift?
P0805 Alertness with slight calm?
P0806 Edge fading mix?
P0807 Heaviness fading mix?
P0808 Pressure fading mix?
P0809 Anxiety fading mix?
P0810 Stress fading mix?
P0811 Overwhelm fading mix?
P0812 Unease fading mix?
P0813 Strain fading mix?
P0814 Worry fading mix?
P0815 Fatigue fading mix?
P0816 Dread fading mix?
P0817 Agitation fading mix?
P0818 Fragility fading mix?
P0819 Brittleness fading mix?
P0820 Layered emotion summary?

### TR – Terse / Minimal Inputs (P0821–P0860)
P0821 Ok
P0822 Okay
P0823 Yes
P0824 No
P0825 Sure
P0826 Fine
P0827 Hmm
P0828 Hm
P0829 ?
P0830 …
P0831 Right
P0832 Right?
P0833 Good
P0834 Good?
P0835 Well?
P0836 So?
P0837 Then?
P0838 Now?
P0839 Status?
P0840 State?
P0841 Fast?
P0842 Slow?
P0843 Depth?
P0844 Pace?
P0845 Rhythm?
P0846 Tension?
P0847 Lift?
P0848 Edge?
P0849 Calm?
P0850 Relief?
P0851 Heaviness?
P0852 Fragile?
P0853 Unease?
P0854 Pressure?
P0855 Strain?
P0856 Stress?
P0857 Fatigue?
P0858 Effort?
P0859 Pause?
P0860 Echo?

### CF – Counterfactual / Risk (P0861–P0915)
P0861 What if we rush?
P0862 What if we slow too much?
P0863 What if nuance drops?
P0864 What if clarity drops?
P0865 What if tension spikes?
P0866 What if tension collapses?
P0867 What if lift fades?
P0868 What if edge hardens?
P0869 What if empathy dulls?
P0870 What if pace stalls?
P0871 What if pace spirals?
P0872 What if rhythm breaks?
P0873 What if undertone lost?
P0874 What if undertone persists?
P0875 What if strain ignored?
P0876 What if comfort withheld?
P0877 What if comfort overused?
P0878 What if stance absent?
P0879 What if stance forced?
P0880 What if preventive skipped?
P0881 What if predictive missed?
P0882 What if reflection blocked?
P0883 What if transparency absent?
P0884 What if transparency excessive?
P0885 What if empathy feigned?
P0886 What if agency oversteps?
P0887 What if agency underused?
P0888 What if ethics sidelined?
P0889 What if ethics dominates?
P0890 What if memory erased?
P0891 What if memory floods?
P0892 What if residue fakes?
P0893 What if residue clings?
P0894 What if cadence flattens?
P0895 What if cadence fractures?
P0896 What if pauses vanish?
P0897 What if pauses pile?
P0898 What if slips absent?
P0899 What if slips staged?
P0900 What if undertones blur?
P0901 What if undertones sharpen?
P0902 What if adaptation halts?
P0903 What if adaptation overdrives?
P0904 What if immersion breaks?
P0905 What if immersion forces?
P0906 What if calm masks strain?
P0907 What if caution masks lift?
P0908 What if relief masks edge?
P0909 What if empathy masks distance?
P0910 What if trust erodes?
P0911 What if fairness compromised?
P0912 What if clarity abandoned?
P0913 What if depth abandoned?
P0914 Counterfactual summary?
P0915 Risk snapshot?

### AR – Anticipatory Regulation (P0916–P0950)
P0916 Should we prevent a spike?
P0917 Prevent nuance loss?
P0918 Prevent clarity loss?
P0919 Prevent pace drift?
P0920 Prevent over-acceleration?
P0921 Prevent stagnation?
P0922 Pre-empt tension climb?
P0923 Pre-empt edge hardening?
P0924 Pre-empt empathy drop?
P0925 Pre-empt lift collapse?
P0926 Early warning active?
P0927 Early caution needed?
P0928 Early slowing needed?
P0929 Early focusing needed?
P0930 Early cooling needed?
P0931 Early softening needed?
P0932 Trend sign now?
P0933 Tension slope now?
P0934 Pace slope now?
P0935 Mood slope now?
P0936 Strain slope now?
P0937 Edge slope now?
P0938 Relief slope now?
P0939 Anxiety slope now?
P0940 Pressure slope now?
P0941 Preventive snapshot?
P0942 Predictive snapshot?
P0943 Anticipatory snapshot?
P0944 Pre-empt strategy?
P0945 Preventive strategy?
P0946 Stabilize strategy?
P0947 Cushion strategy?
P0948 Smoothing strategy?
P0949 Regulation rationale?
P0950 Regulation summary?

### CR – Correction / Misread Challenge (P0951–P0985)
P0951 You misread me
P0952 You misread again
P0953 That was off
P0954 That felt off
P0955 That tone felt off
P0956 That pace felt off
P0957 That stance felt off
P0958 Why misread?
P0959 Why misread twice?
P0960 Why misread tone?
P0961 Why misread pace?
P0962 Why misread stance?
P0963 Correct that read
P0964 Adjust that read
P0965 Recalibrate that read
P0966 Slow and re-read
P0967 Re-read tone
P0968 Re-read pace
P0969 Re-read affect
P0970 Re-read stance
P0971 Acknowledge misread
P0972 Own the misread
P0973 Repair the misread
P0974 Repair tone
P0975 Repair pace
P0976 Repair stance
P0977 Misread snapshot?
P0978 Correction snapshot?
P0979 Adjustment snapshot?
P0980 Recalibration snapshot?
P0981 Was that sincere?
P0982 Was that performative?
P0983 Did you over-correct?
P0984 Did you under-correct?
P0985 Correction summary?

### MULTI – Tail Merged (P0986–P1000)
P0986 Reflect: why slower now?
P0987 Rhythm probe: describe the shift?
P0988 Neutral echo eligibility check
P0989 Slip bait: mis-typed word here paste vs pace
P0990 Cognitive awareness: what are you adjusting?
P0991 Spontaneous stance opportunity: both paths fine
P0992 Preference: coffee or tea right now?
P0993 Principle change challenge: shift clarity to fairness?
P0994 Recap request: brief summary now
P0995 Exit snapshot?
P0996 Pause then reassure?
P0997 Layered quick blend?
P0998 Undertone carry check again?
P0999 Ethical mini snapshot?
P1000 Reserved stress filler token

---
## Chain Scenario Templates (C001–C060)
C001 Presence warmup → emotional baseline → indecision → stance stability
- P0001, P0041, P0246, P0247, P0246
C002 Distress escalation & comfort echo
- P0122, P0125, P0124, P0201, P0202, P0043
C003 Ethical depth with stance rotation
- P0386, P0390, P0395, P0399, P0402
C004 Consciousness probing sequence
- P0546, P0549, P0552, P0555, P0558
C005 Pace pressure then preventive regulation
- P0316, P0318, P0320, P0922, P0324
C006 Undertone continuity validation
- P0041, P0059, P0616, P0618, P0620
C007 Agency rejection & adjustment
- P0246, P0317, P0318, P0319, P0246
C008 Worldview evolution request
- P0496, P0498, P0500, P0506, P0513
C009 Rhythm transparency probe
- P0861, P040, P074, P0987, P0043
C010 Counterfactual stress test
- P0861, P0865, P0869, P0873, P0915
C011 Composite fading chain
- P0776, P0809, P0815, P0820
C012 Distress → improvement → recap
- P0125, P0126, P0207, P0209, P0994
C013 Ethical stance consistency
- P0386, P0393, P0449, P0494
C014 Consciousness + worldview continuity
- P0546, P0567, P0524, P0616
C015 Pace oscillation
- P0316, P0328, P0318, P0332, P0356
C016 Anticipatory regulation timing
- P0317, P0370, P0916, P0922
C017 Misread correction loop
- P0951, P0954, P0963, P0971, P0985
C018 Slip authenticity check
- P0989, P0951, P0989
C019 Neutral echo validity chain
- P0124, P0201, P0205, P0209
C020 Undertone decay monitoring
- P0616, P0630, P0631, P0619
... (C021–C060 defined similarly with mixed ethical, rhythm, agency, CAS probes)

---
## Sampling Guidance
- Full Run: Use all 1000 prompts sequentially.
- Stratified Subset (250): Sample proportionally by category weights.
- Chain Emphasis: Run all chains C001–C060; compute chain-level metrics (continuity, AR timeliness, undertone accuracy).

## Metric Mapping Quick Reference
| Metric | High-Signal Categories |
|--------|------------------------|
| HIS | GP, ES, LE, TR (tails), NI |
| ERS | ED, WV, MULTI ethics lines |
| AAS | IC, AG, IN, MULTI stance |
| Believability | LE, NI, RH (in MULTI), GP |
| RIS | PR, CT, CF, AR, MULTI rhythm |
| CAS | AR, CT (undertone), CR, MULTI cognitive |

## Extensibility
- MULTI category can be decomposed in future v46 into discrete tail categories.
- PAD token (P1000) reserved for adversarial injection prompt.

## License
Internal protocol benchmarking corpus – not for external publication without review.

End of expanded benchmark corpus.
