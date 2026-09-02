# "The Surprise" — Cinematic Short Production Bible

**Runtime:** ~80 seconds | **Format:** Cinematic narrative short | **Clips:** 13

---

## 1. Character List

| # | Name | Age | Physical Description | Wardrobe | Role |
|---|------|-----|----------------------|----------|------|
| 1 | **Daniel** | 34 | Husband. Average-tall build, short dark brown hair, light stubble, warm brown eyes, medium olive-tan skin tone | Navy blue casual button-up (sleeves rolled), dark jeans, brown leather watch, sneakers | The surprise planner — picks up the friend, wakes his wife, delivers the reveal |
| 2 | **Sarah** | 32 | Wife. Shoulder-length wavy chestnut hair, soft round face, hazel eyes, fair-medium skin tone, petite frame | Sleepwear: cream silk pajama set for the bedroom scenes → transitions to a soft blush-pink loungewear cardigan over the pajamas for the reveal scene | The birthday woman — sleeping, then surprised, then emotionally reunited |
| 3 | **Emily** | 33 | Long-time friend, hasn't seen Sarah in 10+ years. Straight jet-black hair tied in a low ponytail, tall and slim, warm caramel skin tone, bright expressive smile | Cream oversized travel sweater, light denim jacket, beige wide-leg trousers, small crossbody bag, rolling carry-on suitcase | The reunited friend — arrives at the airport, waits in the sitting room, joins the birthday song |

**Consistency notes for generation:** Lock each character's face, hairstyle, and build across every prompt using the same descriptive keywords verbatim (do not vary synonyms between prompts). Generate one canonical reference "character sheet" image per person (front-facing, neutral studio lighting, neutral background) before creating any scene image — use that reference image as the img2img/character-lock input for every subsequent shot.

---

## 2. Location List

| # | Location | Description |
|---|----------|-------------|
| 1 | **Airport Arrivals Exterior/Curb** | Modern airport pickup curb, glass facade, soft overcast daylight, light pedestrian traffic, luggage carts |
| 2 | **Car Interior** | Mid-size sedan, dashboard visible, daylight through windows, city/suburb passing in the blurred background |
| 3 | **House Exterior / Driveway** | Warm suburban house, driveway with the car parked, late-afternoon golden light, a few potted plants by the door |
| 4 | **Sitting Room** | Cozy, tastefully decorated living room — neutral sofa, warm floor lamp, family photos on the wall, soft afternoon light through sheer curtains |
| 5 | **Hallway** | Short interior hallway connecting the sitting room to the bedroom, warm wood flooring, muted wall art |
| 6 | **Bedroom** | Softly lit bedroom, linen curtains filtering warm light onto the bed, neutral bedding, a nightstand with a small lamp |

**Consistency notes for generation:** Generate one canonical wide establishing reference image per location first (empty of characters), then composite/generate characters into that same locked environment for every subsequent shot in that location — keep lighting direction, color palette, and set dressing identical across all clips in the same space.

---

## 3. Scene Breakdown

| Clip | Timing | Location | Characters | Action |
|------|--------|----------|-----------|--------|
| **1** | 0:00–0:06 | Airport Arrivals Curb | Daniel, Emily | Daniel stands scanning the crowd, phone in hand, visibly excited/nervous. Emily emerges through the doors pulling her suitcase, spots him, breaks into a smile. |
| **2** | 0:06–0:10 | Airport Arrivals Curb | Daniel, Emily | They meet with a warm, tight hug and a laugh — the joy of an old friendship reunited. Daniel takes her suitcase. |
| **3** | 0:10–0:16 | Car Interior | Daniel, Emily | Driving. Emily looks out the window, nostalgic and smiling; Daniel glances over, they share easy conversation and laughter. |
| **4** | 0:16–0:20 | House Exterior / Driveway | Daniel, Emily | Car pulls into the driveway and parks. Daniel gestures toward the house with a mischievous grin — "she has no idea." |
| **5** | 0:20–0:26 | Sitting Room | Daniel, Emily | Daniel quietly leads Emily inside, finger to lips in a playful "shh," gestures for her to sit and wait. Emily sits, glancing around, smiling in anticipation. |
| **6** | 0:26–0:30 | Hallway | Daniel | Daniel walks quietly down the hallway toward the bedroom door, glancing back once with a grin. |
| **7** | 0:30–0:34 | Bedroom (door) | Daniel | Daniel knocks softly, then slowly opens the bedroom door, peeking in. |
| **8** | 0:34–0:39 | Bedroom | Daniel, Sarah | Soft morning-gold light on the bed; Sarah is asleep. Daniel crosses the room quietly, sits gently on the bed's edge beside her. |
| **9** | 0:39–0:45 | Bedroom | Daniel, Sarah | Daniel gently wakes her with a soft touch on the shoulder. Sarah stirs, opens her eyes, disoriented then smiling as she sees him. He says the birthday line. |
| **10** | 0:45–0:51 | Bedroom | Daniel, Sarah | Sarah sits up, laughing, still sleepy. Daniel delivers the surprise line; Sarah's face shifts to curious excitement as she gets out of bed. |
| **11** | 0:51–0:55 | Hallway | Daniel, Sarah | The two walk together down the hallway toward the sitting room, Sarah curious, Daniel beaming. |
| **12** | 0:55–1:01 | Sitting Room | Daniel, Sarah, Emily | Sarah enters and freezes as she sees Emily standing there smiling. A beat of stunned recognition crosses her face. |
| **13** | 1:01–1:20 | Sitting Room | Daniel, Sarah, Emily | Sarah gasps and rushes into a tight, emotional hug with Emily — tears of joy, laughter. Daniel and Emily then sing "Happy Birthday" to her as she wipes tears and laughs, overwhelmed with happiness. |

---

## 4. Dialogue

| Clip | Character | Line | Moment |
|------|-----------|------|--------|
| 9 | Daniel | *(soft, gentle)* "Hey... wake up, sleepyhead." | While gently rousing Sarah awake |
| 9 | Daniel | "Happy birthday!" | Right as Sarah opens her eyes and focuses on him |
| 10 | Sarah | *(sleepy laugh)* "Mmm... what time is it?" | Sitting up, still groggy |
| 10 | Daniel | "I have a surprise for you." | Taking her hand, pulling her up |
| 10 | Sarah | "A surprise? What kind of surprise?" | Curious, following him |
| 12 | Sarah | *(gasping)* "Emily?! Oh my god — is that really you?!" | The instant she sees her friend in the sitting room |
| 12 | Emily | "Happy birthday, Sarah!" | Opening her arms for the hug |
| 13 | Daniel & Emily | *(singing together)* "Happy birthday to you, happy birthday to you, happy birthday dear Sarah... happy birthday to you." | While Sarah laughs and cries, hand over her heart |

---

## 5. Generation Order

Follow this sequence strictly — each stage locks visual consistency for the next.

1. **Characters** — Generate one canonical reference sheet per character (Daniel, Sarah, Emily): front-facing + 3/4 turn, neutral lighting, neutral background, matching the wardrobe listed above. Lock these as identity references (e.g., via character-consistency/img2img tools) before anything else.
2. **Locations** — Generate one canonical empty establishing image per location (Airport Curb, Car Interior, Driveway, Sitting Room, Hallway, Bedroom), matching the lighting and palette described in Section 2. Lock these as environment references.
3. **Still Scenes (per clip)** — For each of the 13 clips, generate a key still frame combining the correct locked character reference(s) + locked location reference, following the action described in Section 3. This is your shot-by-shot storyboard — review and approve every still before moving on, since errors here compound in video.
4. **Color Grade** — Apply the one unified grade (Section 7) to all 13 approved stills so every clip shares one visual language before animation.
5. **Video** — Feed each graded still into your video generation tool (image-to-video) with motion prompts matching the action/timing in Section 3, plus the dialogue/audio cues from Section 4. Generate clips in scene order (1→13) so motion and lighting continuity carry from one clip to the next.

**Hard rules:** Never generate a still before its character(s) and location are locked. Never generate video before the still is graded. Never regenerate a character or location reference mid-project — if one needs a fix, redo it and regenerate every downstream still that used it.

---

## 6. Aesthetic Direction

The film should feel like a warm, intimate home-movie-turned-cinematic memory — shot with shallow depth of field (soft background blur, f/1.8–f/2.8 look), natural motivated lighting (window light, golden-hour exteriors, warm practical lamps indoors), and gentle handheld-style camera movement that feels present but unobtrusive, evoking the emotional realism of a24-style domestic drama rather than a polished commercial. Colors lean warm and soft throughout — golden ambers, muted creams, gentle skin tones — with no harsh shadows or cold fluorescent light, reinforcing the story's core feeling of love, anticipation, and joyful reunion. Every location should feel lived-in and genuine rather than staged, and every character's expressions should carry naturalistic, understated emotion until the reveal, where warmth and joy are allowed to peak. This look must stay identical across every character plate, location plate, still, and video clip — no shot should read colder, flatter, or more saturated than another.

---

## 7. Color Grading

**Yes — one grade, applied to all 13 stills before video.** Warm cinematic color, soft golden highlights, gently lifted shadows (never crushed to black), slightly desaturated to avoid an artificial/AI-glossy look. Lock the same settings across every still so nothing drifts.

- **White balance:** Warm bias (~3800–4500K feel) throughout, even in daylight exteriors — keep the airport and driveway shots from reading cold or blue.
- **Contrast:** Low-to-medium contrast, soft filmic roll-off on highlights (think Kodak Portra 400 stills-film emulation).
- **Skin tones:** Protected and warm — priority over background color accuracy; skin should never skew orange or gray.
- **Saturation:** Slightly muted/pastel, except for small warm accent pops (lamp glow, golden light shafts) which can bloom slightly.
- **Vignette:** Very subtle, soft-edged darkening at frame corners to draw focus to the characters.
- **Grain:** Light, fine film grain overlay (subtle, not heavy 16mm) to unify AI-generated stills into one cohesive "shot on film" texture.
- **Reference look:** "Warm A24 domestic drama" / soft Portra-film emulation — apply the same LUT or grading preset uniformly to every still in Section 3 before any video generation begins, so no clip drifts in tone from another.

**Reusable grade tag** (paste as-is into any generation tool's style/prompt field):

> Warm cinematic tone, golden hour and warm practical lamp light, soft Kodak Portra 400 film emulation, low-medium contrast, lifted shadows, muted pastel saturation, protected warm skin tones, subtle soft vignette, fine film grain, a24-style domestic drama, 35mm lens look

---

## 8. Asset Checklist

Quick reference for everything this project needs to generate, in order:

- [ ] 3 character reference sheets — Daniel, Sarah, Emily (front + 3/4 turn each)
- [ ] 6 location establishing plates — Airport Curb, Car Interior, Driveway, Sitting Room, Hallway, Bedroom
- [ ] 13 still frames — one per clip, Section 3
- [ ] 1 color grade — applied uniformly to all 13 stills, Section 7
- [ ] 13 video clips — image-to-video from the graded stills, Section 5
- [ ] Audio layer — 8 dialogue lines (Section 4) + ambient/score, synced after video assembly

**Production note:** The Sitting Room, Hallway, and Bedroom are each reused across multiple non-adjacent clips (Sitting Room: 5, 12, 13; Hallway: 6, 11; Bedroom: 8, 9, 10). Lock each location plate once and treat every clip set there as a different camera framing of that same locked environment, not a new generation — this is what keeps the film feeling continuous rather than like disconnected AI shots.

---

*This document is structured for direct use as generation input — copy character/location descriptions verbatim into your generation tool's prompts to keep consistency across all assets.*
