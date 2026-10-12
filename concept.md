# "Three Kids, Two Cultures" — TikTok Series Concept (Montserratian + Cantonese Family)

## Overview

A short-form TikTok series depicting the day-to-day life of a fictional
multicultural family, rendered in a realistic cartoon style using AI
image/video generation tools. The goal is authentic, warm, observational
comedy about the overlap and friction of two cultures under one roof —
not caricature of either side.

- **Goal:** Represent a multicultural family's everyday life authentically
  (fully fictional, not based on a specific real family, but written to
  feel real).
- **Visual style:** Realistic cartoon (semi-realistic, Pixar/DreamWorks-
  adjacent), produced with AI tools (e.g. Midjourney for character/scene
  art + an AI animation tool for motion).
- **Episode format:** ~2 minute mini-stories per episode, each with a
  clear setup → payoff structure (more room than a quick 15-30s gag for
  actual dialogue and small story arcs).
- **Setting:** London. A strong real-world fit — after the mid-1990s
  Soufrière Hills volcanic eruption, many Montserratians relocated to the
  UK (holding British citizenship as a UK Overseas Territory), and London
  has long-established Chinese communities as well. Plausible without
  needing exposition.

## Cast

| Character | Role | Notes |
|---|---|---|
| Dad | Montserratian | Warm, laid-back island energy. Montserrat brings unique texture: a distinct Irish-Caribbean heritage (St. Patrick's Day is a public holiday there), goat water stew, mountain chicken lore, and the Soufrière Hills volcano/evacuation backstory. Less commonly depicted than Jamaica, so it reads as specific rather than generic Caribbean. |
| Mum | Cantonese | Dry wit, tea rituals, small superstitions (numbers, feng shui placement), discipline-with-love. |
| Daughter | Age 8 | Self-aware about the cultural mix; code-switches on purpose; often the one narrating/explaining the household's quirks to friends. |
| Son | Age 6 | Prime "chaos agent" age — mixes up patois and Cantonese words/traditions without noticing. Main source of "kids say the darndest things" bits. |
| Baby boy | Age 1 | Mostly reactive/visual gags — faces at new foods, babbling that sounds like it's attempting both languages, being passed between culturally-coded snacks. |

## Tone

Warm, observational family-sitcom comedy. Humor comes from the genuine
overlap and friction between two specific cultures, never from mocking
either one.

## Recurring Story Wells (for 2-minute mini-stories)

1. **Food fusion** — disasters and wins (e.g. goat water with congee,
   dumplings with scotch bonnet pepper).
2. **Holiday mashups** — Lunar New Year red envelopes alongside Christmas
   gifts; a "Calypso meets Celtic" St. Patrick's Day since Montserrat
   observes it as a national holiday.
3. **Language mix-ups** — a kid blending a Cantonese phrase with patois
   rhythm, confusing a relative or teacher.
4. **Parenting style clashes** — Dad's island-easygoing approach vs. Mum's
   superstition/discipline approach colliding over one kid decision.
5. **Extended family visits** — an aunt/uncle from either side dropping in
   with unsolicited opinions.
6. **Kids explaining the household** — to confused friends/teachers who
   don't know what to make of the mix.

## AI Production Workflow

Pipeline for keeping the cast visually consistent across episodes, based
on current (2026) AI image/video tooling:

1. **Series bible + character sheets (built once).** Fix each character's
   visual traits (face shape, skin tone, hair, outfit, build) and
   personality notes as a permanent reference — never regenerated per
   episode.
2. **Generate character stills.** Use Midjourney's character-reference
   feature to lock each character's face/body across multiple poses and
   expressions (front/side/3-4 expressions per character). This only
   works for stills, not video, but is the cheapest way to nail down
   "what does Dad look like" before touching motion.
3. **Animate shots using those stills as reference.** AI video models
   have no memory between generations, so an image anchor — not text
   prompts alone — is what holds a face/outfit steady shot to shot.
   - **Kling** — its "Elements" system takes 1-4 reference images per
     generation; 3.0 claims multi-shot consistency across cuts. Primary
     candidate for this step.
   - **Runway Gen-4.5** — alternative; strong within a single shot/scene,
     with a "Director Mode" for multi-shot sequences, but cross-episode
     consistency relies more on the editor.
   - Expect short generated clips (~3-15s) stitched together — no tool
     currently holds a character reliably across a full 2-minute episode
     in one generation.
4. **Editing/assembly.** Stitch AI-generated clips in a standard editor
   (CapCut, Premiere) into the full 2-minute mini-story; add dialogue/
   voiceover (e.g. ElevenLabs for consistent character voices), music,
   and captions.
5. **Cross-episode continuity.** Reuse the same locked character-sheet
   stills as the reference input for every new episode's shots — don't
   regenerate character designs per episode. Where a tool supports
   multiple reference images, also feed in frames from finished episodes
   as additional reference material for later ones.

**Note:** stylized/cartoon rendering tolerates frame-to-frame drift
better than photoreal does, which favors this project's "realistic
cartoon" (not fully photorealistic) direction.

## Character Design Reference

Likeness-based character sheet prompts, built from a reference family
photo, for Step 2 of the AI Production Workflow (Midjourney character
stills). Each prompt generates a turnaround sheet (front + 3/4 view,
multiple expressions) to lock the character before any animation step.
Attach the reference photo as the tool's image-reference input (e.g.
Midjourney `--cref`) alongside the prompt text; weight it moderately
(`--cw 50-60`) so the tool captures likeness without copying the
photo's specific pose/lighting.

**Shared style suffix** (append to every character prompt):
`realistic cartoon style, semi-stylized 3D animated film look,
Pixar/DreamWorks-adjacent character design, soft studio lighting, clean
neutral background, consistent proportions for animation reference
--cref [reference photo URL] --cw 60 --ar 1:1 --style raw --v 6.1`

### Dad
> Character turnaround sheet, front view and 3/4 view, warm open smile
> and neutral expressions, Black man, medium-brown skin tone, trimmed
> full beard and mustache, short dark hair, broad friendly build,
> wearing a navy baseball cap and a casual white button-up shirt with
> sleeves rolled to the forearm — [shared style suffix]

### Mum
> Character turnaround sheet, front view and 3/4 view, warm composed
> smile and neutral expressions, East Asian woman, fair-medium skin
> tone, black hair pulled back with a black bow, slim build, wearing a
> black and white striped short-sleeve top and high-waisted jeans with a
> brown belt — [shared style suffix]

### Daughter, 8
> Character turnaround sheet, front view and 3/4 view, playful knowing
> smile and neutral expressions, mixed-heritage girl, curly medium-length
> dark brown hair, warm brown skin tone, wearing a black headband and a
> cream cardigan over a striped top — [shared style suffix, child
> proportions]

### Son, 6
> Character turnaround sheet, front view and 3/4 view, focused deadpan
> expression and neutral expression, mixed-heritage boy, curly dark
> brown hair, light-medium brown skin tone, wearing a striped button-up
> shirt open over a plain cream tee — [shared style suffix, child
> proportions]

### Baby boy, 1
> Character turnaround sheet, front view and 3/4 view, curious wide-eyed
> expression and neutral expression, mixed-heritage baby boy, soft curly
> dark hair, round cheeks, light-medium brown skin tone, wearing a
> simple cream outfit — [shared style suffix, toddler proportions]

### Full family group reference
> Full family group portrait, Montserratian father, Cantonese mother,
> mixed-heritage daughter (8), son (6), and baby boy (1), warm candid
> family pose, soft evening lighting, London rooftop/garden setting,
> consistent character designs matching the individual character sheets
> above — realistic cartoon style, semi-stylized 3D animated film look,
> Pixar/DreamWorks-adjacent, --cref [reference photo URL] --cw 50
> --ar 3:2 --style raw --v 6.1

**Note:** everyday "signature looks" above (cap/beard for Dad, hair bow
for Mum, headband for Daughter, striped layering for Son) are meant to
recur across episodes as default outfits, distinct from the family
photo's one-off special-occasion clothing — this keeps character
recognition strong without requiring the exact photographed outfit every
time. Since the reference photo is a real private family photo, keep it
to personal/private uploads in whichever tool is used, per that tool's
terms.

## Title Card & Intro Format

Kept lightweight since TikTok retention drops fast if the first few
seconds aren't the hook itself.

**Logo concept:** two overlapping circles (Venn-diagram style) — one in
a warm Caribbean gold/orange, one in Chinese red/gold — overlapping in
the middle in a blended warm amber tone. Reads as "two cultures, one
family" without using either side's actual flag, keeping the focus on
the family rather than a national statement.

**Palette:** warm amber/gold as the shared anchor color (bridges
Caribbean sunset tones and Chinese red-gold lucky-color associations),
with cream/off-white as a neutral background.

**Typography:** rounded, friendly sans-serif for "Three Kids, Two
Cultures" — legible at small TikTok sizes, no serif/formal fonts, keeps
the warm family-sitcom feel.

**Mark placement:** a small persistent logo bug in a corner throughout
the episode, rather than a big static title screen.

**Intro sequence (per episode):**
1. **0:00–0:01 — Quick logo sting.** The two circles snap together with
   a soft "pop" sound and a brief text flash of the series name. Under a
   second — a brand flag, not a pause.
2. **0:01 onward — straight into the episode's first beat.** No recap,
   no character-intro card each time; the show should always read as
   "mid-conversation," like a real sitcom.
3. **Episode title as on-screen text overlay**, small, top or bottom
   corner, fading in/out during the first 2-3 seconds — doesn't block
   the hook, but gives the clip a title for sharing/screen-recording.
4. **End card:** reuse each episode's existing freeze-frame final beat,
   then a 1-second outro card — logo + "Follow for more" + episode
   number. Consistent close without eating into watch-through rate.

## Episode Scripts

Draft scripts, ~2 minutes each, broken into beats so each beat maps to
one AI-generated clip in the production pipeline above.

### Episode 1: "Goat Water Congee"
**Well:** Food fusion
**Logline:** Dad tries to doctor Mum's congee with his goat water seasoning while she's out — chaos and an unexpected family hit follow.

| Beat | Shot | Dialogue/Action |
|---|---|---|
| 1 (0:00-0:15) | Kitchen, morning. Mum's pot of congee simmers on the stove. Dad peers in, sniffs, unimpressed. | **Dad:** "Dis need a lickle something." *(pulls out his goat water spice jar)* |
| 2 (0:15-0:35) | Dad dumps a generous spoon in, stirs, tastes, nods proudly. Son (6) wanders in, curious. | **Son:** "Daddy, what you doing to Mummy's food?" **Dad:** "Making it better, bredda. Don't tell." |
| 3 (0:35-0:55) | Daughter (8) walks in, sees the jar, immediately looks worried — she knows what's coming. | **Daughter:** *(to camera, deadpan)* "He does this every time. It's never once worked." |
| 4 (0:55-1:20) | Mum returns, suspicious sniff at the door, walks to the pot. Whole family freezes. She tastes it. Long pause. | **Mum:** *(unreadable face)* ... |
| 5 (1:20-1:45) | Mum takes a second spoonful. Then a third. Family exhales. | **Mum:** "...Don't tell your grandmother I put scotch bonnet in congee." **Dad:** *(triumphant)* "SEE?!" |
| 6 (1:45-2:00) | Baby boy bangs spoon on highchair tray, demanding more. Freeze frame / title card. | **Daughter:** *(to camera)* "Okay. Once." |

### Episode 2: "Two Patron Saints"
**Well:** Holiday mashup
**Logline:** The family preps for a mashed-up St. Patrick's Day (Montserrat) and Lunar New Year that land in the same week — decorations collide.

| Beat | Shot | Dialogue/Action |
|---|---|---|
| 1 (0:00-0:15) | Living room. Dad hangs shamrock bunting on one wall. Mum, on a ladder, hangs red lanterns on the other. | **Dad:** "Montserrat flag AND a shamrock, every year, no questions." **Mum:** "Lanterns go higher than the shamrocks." |
| 2 (0:15-0:40) | Son holds up two outfits — a green shirt and a red one — totally lost. | **Son:** "Which one am I wearing?" **Dad + Mum (in unison):** "BOTH." |
| 3 (0:40-1:05) | Daughter, to camera, holding a red envelope with a shamrock drawn on it in marker. | **Daughter:** "I made my own hybrid. Lucky money AND luck of the Irish. I'm covered." |
| 4 (1:05-1:35) | Family sits for dinner — goat water stew next to a plate of nian gao (rice cake). Dad raises a glass. | **Dad:** "To Montserrat and to the Year of—" **Mum:** "The Snake." **Dad:** "—the Snake! Even though we chased them out of Ireland." |
| 5 (1:35-2:00) | Baby boy grabs a lantern and a tiny shamrock decoration, holds both up, delighted. Freeze frame. | *(No dialogue — just chaos and a laugh track beat.)* |

### Episode 3: "Wrong Language, Right Moment"
**Well:** Language mix-ups
**Logline:** Son accidentally greets a visiting Cantonese-speaking relative in patois-accented Cantonese — and it somehow lands perfectly.

| Beat | Shot | Dialogue/Action |
|---|---|---|
| 1 (0:00-0:15) | Doorbell rings. Mum, mildly panicked, straightens things. | **Mum:** "That's your Por Por's cousin. Everyone — best behavior, best Cantonese." |
| 2 (0:15-0:35) | Son practices a Cantonese greeting under his breath, but it comes out with a thick patois lilt. | **Son:** *(muttering, rehearsing)* "Nei... nei hou... wah gwan..." |
| 3 (0:35-1:00) | Door opens. Elderly relative steps in. Son blurts his greeting — it comes out an odd blend, confident and completely wrong-sounding. | **Son:** *(loud, proud)* "WAH GWAN, POR POR COUSIN!" |
| 4 (1:00-1:30) | Stunned silence. Daughter winces off to the side. Then the relative BURSTS out laughing, delighted. | **Relative:** *(laughing, in Cantonese/subtitled)* "This child has invented a new dialect!" |
| 5 (1:30-2:00) | Mum, relieved and amused, ruffles Son's hair. Dad in the background, smug. | **Mum:** "...Somehow that worked." **Dad:** *(to camera)* "Montserrat-Cantonese. Officially a language now." |

### Episode 4: "The Discipline Summit"
**Well:** Parenting style clashes
**Logline:** Son gets in trouble at school for trading his lunch — Dad wants to let it slide, Mum wants a "proper talk," and the two styles collide in front of the kid.

| Beat | Shot | Dialogue/Action |
|---|---|---|
| 1 (0:00-0:15) | Living room, evening. Son sits on the couch, head down. Mum and Dad stand over him, exchanging a look. | **Mum:** "He traded his lunch. For the THIRD time." **Dad:** "So? Boy was just doing business." |
| 2 (0:15-0:40) | Mum crosses her arms, unimpressed. Dad shrugs, very relaxed. | **Mum:** "There is a *process*. We sit him down, we explain consequences, we—" **Dad:** "Or. We let him keep the five dollars he made." |
| 3 (0:40-1:05) | Son's eyes light up at "five dollars." Daughter, watching from the stairs, mouths "oh no" to camera. | **Son:** *(perking up)* "Wait, I get to KEEP it?" **Mum:** *(sharp look at Dad)* "Absolutely not." |
| 4 (1:05-1:35) | Mum and Dad huddle, whispering intensely, clearly negotiating. Son watches, swinging his legs, unbothered. | **Dad:** *(whispering)* "Okay, fine — he keeps HALF, and he never does it again." **Mum:** *(whispering)* "...Deal." |
| 5 (1:35-2:00) | They turn back to Son with a unified "stern" face that immediately cracks. Son grins, knowing he won. Freeze frame. | **Mum + Dad (together):** "Don't do it again." **Son:** *(to camera)* "I'm doing it again." |

### Episode 5: "Auntie Has Notes"
**Well:** Extended family visits
**Logline:** An unannounced visit from Dad's sister turns into a running commentary on literally everything in the house, Cantonese side included.

| Beat | Shot | Dialogue/Action |
|---|---|---|
| 1 (0:00-0:15) | Doorbell. Mum opens it to find Auntie already mid-sentence, rolling a suitcase in. | **Auntie:** "I'm only staying three days — why is the furniture facing THIS way?" |
| 2 (0:15-0:40) | Auntie walks through the house, touching things, narrating critiques. Mum trails her, forcing a smile. | **Auntie:** "Goat water needs more thyme. Also — lanterns too low, bad feng shui, I can feel it." |
| 3 (0:40-1:05) | Daughter, cornered in the hallway by Auntie, gets hit with rapid-fire observations. | **Auntie:** "You've grown. You're too thin. Eat more. Also your Cantonese accent needs work, no offense." |
| 4 (1:05-1:35) | Dad, overhearing from the kitchen, mouths "I'm sorry" to Mum across the room. Mum mouths back "three days" like a countdown. | *(No dialogue — just panicked eye contact.)* |
| 5 (1:35-2:00) | Auntie sits, suddenly completely at ease, sipping tea like nothing happened. Baby boy crawls up to her, and she melts instantly. | **Auntie:** *(voice totally different, soft)* "There's my favorite." **Daughter:** *(to camera)* "She's actually the best. Don't tell her I said that." |

### Episode 6: "How Do I Even Explain This"
**Well:** Kids explaining the household
**Logline:** Daughter's friend comes over for the first time and needs a full briefing before she's allowed to understand anything happening in the house.

| Beat | Shot | Dialogue/Action |
|---|---|---|
| 1 (0:00-0:15) | Front yard. Daughter stops her friend before they walk in, hand up like she's about to give a safety briefing. | **Daughter:** "Okay, before we go in — a few things you need to know." |
| 2 (0:15-0:45) | Quick cuts as Daughter counts off on her fingers, friend's eyes widening with each point. | **Daughter:** "One: we celebrate everything twice. Two: my dad will try to feed you something spicy and call it love. Three: my mum can tell if you're lying by your face." |
| 3 (0:45-1:10) | They step inside. Dad immediately appears with a plate. Friend looks at Daughter, panicked. | **Dad:** "Try this." **Friend:** *(whispering to Daughter)* "Is this the spicy thing?" **Daughter:** "Just smile and say thank you." |
| 4 (1:10-1:40) | Friend eats it, eyes water instantly, but she nods bravely. Mum appears from nowhere, studying her face intensely. | **Mum:** *(squinting)* "...She's being polite. I like her." |
| 5 (1:40-2:00) | Friend, slightly shellshocked but delighted, turns to Daughter. Son runs past yelling something in half-Cantonese-half-patois. Freeze frame. | **Friend:** "This is the best house I've ever been in." **Daughter:** *(to camera, proud)* "Told you." |

## Open Items / Next Steps

All creative and production decisions are locked, including likeness-
based character design prompts. Remaining work is production itself:
generate the character sheet stills, generate the shot clips, and
assemble the first episode.
