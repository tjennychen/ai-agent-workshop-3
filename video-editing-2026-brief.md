# AI video editing, mid 2026: a working brief

For Jenny's own short-form vertical editing (and the workshop). Researched 2026-06-26, weighted to the last 3 to 6 months. Skeptic notes are inline; vendor stats are flagged.

## The one shift that matters
Two things genuinely changed this year, everything else is caption polish:
1. **Edit-by-prompt over a real timeline** (Palmier agent, Runway Aleph/Agent, Descript Underlord, CapCut Video Studio). The timeline becomes a review layer of what the agent did.
2. **Vertical-native generative b-roll with synced audio** (Veo 3.1, Kling 3.0, Seedance 2.0), composed for 9:16, not cropped.

For Dr Deb's brand: push hard on prompt-editing + generative b-roll of nature/abstract subjects. Avoid AI avatars and AI voices of a real person; they read as inauthentic for wellness, and the tech still flickers on hands, text, and human motion.

## Try this week (highest leverage, solo-usable)
1. **Palmier Pro agent-on-timeline + inline Seedance/Kling b-roll.** The most on-method move: drive the Palmier timeline from Claude via MCP, generate b-roll inline. Free editor, pay-per-generation. Needs macOS 26 on Apple Silicon; it is v0.3.x, expect rough edges.
2. **Veo 3.1 free tier (via Google Vids / Flow)** for native-vertical 4K b-roll. Best quality-per-effort, real free allowance. US-side only (blocked in mainland without VPN).
3. **Kling 3.0 (Kuaishou)** as the China-accessible b-roll engine, no VPN. New multi-shot storyboard for short sequences. "Same prompt, Veo vs Kling, two markets" is itself good workshop content.
4. **Descript for the talking-head pass:** filler/silence removal + run up to 5 b-roll generations in parallel + Underlord v2 (edit-by-prompt over the transcript). Lowest-friction upgrade to your weekly Dr Deb cut. Check the new ElevenLabs Scribe v2 transcription on her real audio before trusting auto-cuts.
5. **Runway Aleph 2.0 / Edit Studio** for AI relight and fix-on-existing-footage (object swap, background, restyle on your own clip, not generate-from-scratch). One paid month to learn the ceiling. US-side.
6. **Cappy (text-an-editor by SMS), 5-minute workshop novelty only,** free to try. Lands the "you can now text an editor" beat. Label it a toy, not a production tool.

## The repeatable pipeline (run this on every Dr Deb clip)
1. Record A-roll vertical.
2. Auto-transcribe, then text-based edit: cut dud sentences, strip filler and pauses.
3. Auto-caption, restyle once, apply-to-all, fix the wellness terms and names (where it always breaks).
4. Mark cutaway points on the transcript; place ~5s b-roll ON the spoken noun; color-match it to the A-roll.
5. Build the hook in the first ~2 seconds: contrarian or outcome line, multimodal (visual interrupt + 4 to 7 word overlay + spoken keyword).
6. Beat-align the caption punches and the cuts.
7. Shoot 3 hook variants, post, read 3-second retention the next morning, keep the winner (benchmark ~60%+).
8. Human QC pass for taste before publish.

## Techniques that are working (ranked)
1. **Text-based editing as the primary cut tool** (Premiere Text-Based Editing, Descript, FireCut for Resolve). The biggest time-saver experienced editors keep.
2. **Captions: auto-generate, fix 2-3 words, style once, apply to all.** ~85% of social video is watched muted (industry figure, not peer-reviewed).
3. **Word-by-word kinetic captions, lower-middle third, high contrast, subtle animation.** Fade or scale per word beats heavy motion. Reserve the color/size punch for the one stat or punchline per clip.
4. **Multimodal hook in ~2s** (visual + text + spoken at once). Drop-off is concentrated in seconds 0-3.
5. **"1 body, 3 hooks" A/B test.** One clip body, three intros, watch first-hour retention. Highest-ROI habit because it compounds.
6. **B-roll on the noun (vertical-axis editing).** Lay the cutaway on the exact word it illustrates, then cut back to face. This is the craft move AI does not decide for you, and the most worth teaching.
7. **AI b-roll: 6-part prompt** (subject + action + setting + lighting/mood + camera move + style), 2-4 variations, ~5s clips, then color-match. Favor close/abstract/landscape where only hair, cloth, water, or light moves.
8. **Long-to-short clippers (OpusClip etc.) as a FIRST PASS only.** Expect to discard 20-40%; they cut on speech pauses and miss silent visual moments. Realistic yield ~8-12 clips per source hour.

## Overrated / skip
- One-click "set and forget" auto-clippers (draft only, 20-40% discard).
- Maxing out caption animation (constant motion lowers retention).
- The generic "CapCut look" (fast beat-cuts + zoom-punch + same preset); fatiguing, especially for a premium wellness brand.
- AI-generated humans / talking avatars for an authentic brand.
- AI voiceover replacing the real voice by default (reserve for true language expansion, disclose it).
- Tool-collecting. The leverage is the repeatable system, not the app count.

## The research (with links, every URL HTTP-verified)
Foundations:
- Murch, *In the Blink of an Eye* (1995, 2nd ed. 2001). Rule of Six (emotion 51, story 23, rhythm 10, eye-trace 7, plane 5, spatial 4) and the blink. https://en.wikipedia.org/wiki/In_the_Blink_of_an_Eye_(book)
- Leake, Davis, Truong, Agrawala, *Computational Video Editing for Dialogue-Driven Scenes*, SIGGRAPH 2017. Machine selects takes and assembles from named rules. https://graphics.stanford.edu/papers/roughcut/
- Pardo et al., *Learning to Cut by Watching Movies*, ICCV 2021. Ranks where a cut is plausible; proposes, does not decide. https://arxiv.org/abs/2108.04294

2026 frontier:
- Wang et al., *From Long Videos to Engaging Clips (HIVE)*, EMNLP 2025 (peer reviewed). Long-to-short as find-highlight, pick-open/close, prune. https://arxiv.org/abs/2507.02790
- Zhao et al., *CutClaw: Agentic Hours-Long Video Editing via Music Synchronization*, arXiv, March 2026 (preprint). Three agents: plan to music, ground on the beat, review for overlap. https://arxiv.org/abs/2603.29664
- Li et al., *VEU-Bench: Towards Comprehensive Understanding of Video Editing*, CVPR 2025 (peer reviewed). The skeptic's receipt: 11 top video models struggle to recognize cuts and transitions, some below random. https://arxiv.org/abs/2504.17828

Also worth reading:
- *Watching TikTok* eye-tracking study, Communication Today 2026 (peer reviewed). Pacing changes the whole attention regime: fast cuts push viewers into a fragmented, reactive mode, so do not stack dense kinetic captions on fast cuts.
- *RankCut*, IUI 2026 (peer reviewed). Transparent auto-cut (show candidate spans + confidence) beats black-box auto-cut for editor trust. DOI 10.1145/3742413.3789115
- d'Ydewalle et al. (1991, 2007). On-screen text is read automatically and obligatorily. The solid basis for captions. (The "word-by-word boosts retention" claim is craft, not proven.)

## Tool releases, newest first (reference)
- Jun 2026: Runway Studio (real timeline), Runway Agent 2.0 (campaign-scale edit-by-prompt), Descript tone tags + 5 parallel generations, Palmier Pro public launch (v0.3.x).
- May 2026: Runway Aleph 2.0 + Edit Studio (edit/relight existing footage), Descript ElevenLabs Scribe v2 transcription.
- Apr 2026: HeyGen Avatar V, Cappy (text-an-editor), Adobe Premiere Color Mode (beta).
- Mar 2026: CapCut Video Studio (geo-restricted away from US at launch, IP fallout), Descript Regenerate upgrade.
- Feb 2026: Kling 3.0, ByteDance Seedance 2.0.
- Jan 2026: Google Veo 3.1 (free tier, native vertical 4K), Descript Underlord v2.

Dead ends / vaporware: Sora consumer app shut down Apr 26 2026 (API sunset Sept 24 2026); Adobe Firefly AI Assistant "coming soon" not shipped; "Runway Gen-4 May 2026" is an SEO error (Gen-4 shipped Mar 2025); Seedance 2.5 announced not shipped.
