# TikTok Series Concept: Multicultural Family (Montserratian + Cantonese)

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
- **Setting:** A diaspora city with real-world plausibility for this
  pairing (e.g. Toronto, NYC, or London).

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

## Open Items / Next Steps

- Finalize a series title (currently untitled; "Two Spice Household" was
  a placeholder, not locked in).
- Decide exact diaspora city setting (Toronto / NYC / London).
- Draft specific episode scripts (2-min setup → payoff format).
