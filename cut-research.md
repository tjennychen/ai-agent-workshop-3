# How editors and AI decide the cut (research backing slide 6)

Research synthesis, 2026-06-25. Backs the "why it works" slide. Keep the deck plain, not academic; these are the receipts.

## The one line
**AI can find every cut and even guess where one should go. The human still owns the blink: the emotional instant the idea lands, which is 74% of what Murch says a cut is for (Emotion 51% + Story 23%).**

## Sources

**1. Walter Murch, In the Blink of an Eye (2nd ed., 2001; orig. 1995), p.18. The human theory of the cut.**
Rule of Six, his priority order with weights (never sacrifice a higher one for a lower):
- Emotion 51%: true to the emotion of the moment. Larger than all five others combined.
- Story 23%: it advances the story.
- Rhythm 10%: occurs at a moment that is rhythmically right.
- Eye-trace 7%: cut where the audience's focus already is.
- Two-dimensional plane / planarity 5%: screen-direction continuity (the 180 line).
- Three-dimensional space 4%: real spatial continuity of bodies and objects.
The blink: Murch saw Hackman blink right where he had decided to cut. Huston: "You blinked. Those are cuts. Your mind cut the scene." The blink tracks the moment a thought completes; the cut is punctuation between ideas.
Application: the cut is felt emotional punctuation, not a clock interval. Cut on the blink, the instant a phrase lands.

**2. Leake et al., Computational Video Editing for Dialogue-Driven Scenes, ACM TOG / SIGGRAPH 2017, 36(4) Art.130. What a machine actually does.**
Script + multiple takes, time-aligns clips to lines, labels framing/sentiment/who-is-visible, then SELECTS the take per line to satisfy named idioms (avoid jump cuts, intensify emotion, speaker visible, start wide, change zoom gradually, etc). HMM per idiom, Viterbi picks the max-likelihood sequence. Full edit in 2 to 3 seconds.
Limits (their own sec 8): works only at whole-line granularity, cannot cut away mid-line for a reaction; no continuity checking; cannot judge performance on features it does not label.
Application: this IS the AI-in-the-editor move: rule-based selection and assembly. It picks and arranges, it does not invent the beat.

**3. Pardo et al., Learning to Cut by Watching Movies, ICCV 2021 (arXiv:2108.04294). NOTE: 2021, not 2019.**
Ranks cut plausibility: given two clips, score how plausible a join is. Contrastive training on 255K real cuts. It ranks/proposes candidate cut points; it does not generate or perform the edit.
Application: a model can now learn where a cut "feels right" on the audiovisual signal, the machine shadow of the blink. It proposes, it does not decide.

Broader learned/LLM line: LAVE (ACM IUI 2024, LLM agent assembles from a clip pool); "From Shots to Stories" (2025, arXiv:2505.12237, LLM does shot classification/selection/ordering). Strong on convergent selection, weak on divergent creative ordering.

**4. Saliency / gaze + shot-boundary detection.**
Saliency (where the eye lands): SALICON (ICCV 2015), DeepGaze I/II, SalGAN, TranSalNet. Computable eye-trace = Murch's #4.
Shot-boundary detection: TransNet V2 (2020), FCN-SBD (Gygli 2018). Detects cuts that ALREADY exist (clean ingest/segmentation). Tells you where cuts ARE, not where one SHOULD be.

**5. Captions / text timing.**
d'Ydewalle et al. (Communication Research 1991; European Psychologist 2007): on-screen text is read automatically and obligatorily, even when not needed, even in an unknown language. Captions capture gaze and aid comprehension on muted video.
Nuance: ACM MUM 2024 keyword-highlight study found highlighted/timed captions helpful BUT also distracting.
Fidelity flag: "captions are read automatically and direct attention" is solid. "Word-by-word on-beat boosts retention" is craft, NOT proven. Do not present on-beat timing as science. The ~85 to 92% sound-off stat is a marketing figure, not peer-reviewed.

## The split (what to put on the slide)
- Machine owns the bottom of Murch's list + the plumbing: boundary detection, selection, assembly, cut-point ranking, attention prediction. That is eye-trace 7 + planarity 5 + 3D 4 = 16%, plus the mechanical labor.
- Human owns the top: Emotion 51 + Story 23 = 74%. Every system's own limitations section concedes this: cannot judge emotion, cannot cut mid-line for the reaction, cannot locate the blink.

## Fidelity flags to honor (per the data-source rule)
1. Pardo is ICCV 2021, not 2019.
2. Word-by-word caption retention = craft, not proven. Solid citation is only d'Ydewalle (captions are read automatically).
