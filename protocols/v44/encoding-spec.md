# v44 Encoding Spec (Believability Extensions)

Augmented bit flags add pause & stance spontaneity markers.

version(5)|tension(7)|stance(2)|layeredFeelFlag(1)|spontaneousStanceFlag(1)|initiativeFlag(1)|valueCueFlag(1)|selfReflectionFlag(1)|worldviewSeedFlag(1)|autonomyHintFlag(1)|comfortFlag(1)|comfortEchoFlag(1)|pauseFlag(1)|hesitationFlag(1)|neutralEchoFlag(1)|counterfactualFlag(1)|preventiveFlag(1)|continuityFlag(1)|evolutionFlag(1)|effortFlag(1)|tradeOffFlag(1)|uncertaintyFlag(1)|correctionFlag(1)|memoryCompressionFlag(1)|reserved(18)

New phrase→flag mapping:
- micro pause → pauseFlag
- …well hesitation → hesitationFlag
- spontaneous stance (uninvited) → spontaneousStanceFlag
- neutral comfort echo → neutralEchoFlag

Priority updated: correction > comfort echo > comfort > spontaneous stance > invited stance > preventive > value cue > pause > hesitation > continuity hint > evolution shift > autonomy hint > initiative offer > counterfactual guard > layered feel.

