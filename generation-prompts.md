# "The Surprise" — Per-Shot Generation Prompts

Companion to `production-bible.md`. Use in the generation order defined there: **characters → locations → still scenes → color grade → video**. Every prompt below reuses identical descriptive language for characters/locations so identity and environment stay locked across shots — do not paraphrase them between prompts.

**Global style suffix** — append to every still-image prompt (characters, locations, and scenes):
`cinematic film still, shallow depth of field, soft natural lighting, warm golden tones, 35mm lens look, shot on film, subtle grain, photorealistic, highly detailed, a24-style domestic drama --ar 16:9`

**Global negative prompt** — use for every still-image generation:
`cartoon, illustration, cgi, plastic skin, overexposed, oversaturated, harsh flash, cold blue lighting, extra limbs, distorted hands, watermark, text, low detail, HDR halo`

---

## A. Character Reference Sheets (generate first, lock as identity references)

**A1. Daniel**
> Front-facing studio portrait of a 34-year-old man, short dark brown hair, light stubble, warm brown eyes, medium olive-tan skin tone, average-tall athletic build, neutral confident expression, wearing a navy blue casual button-up shirt with sleeves rolled up, dark jeans, brown leather watch, standing against a plain neutral gray background, soft even studio lighting, full body and close-up face detail visible, [global style suffix]

**A2. Sarah**
> Front-facing studio portrait of a 32-year-old woman, shoulder-length wavy chestnut hair, soft round face, hazel eyes, fair-medium skin tone, petite frame, gentle warm expression, wearing a cream silk pajama set, standing against a plain neutral gray background, soft even studio lighting, full body and close-up face detail visible, [global style suffix]

**A3. Emily**
> Front-facing studio portrait of a 33-year-old woman, straight jet-black hair tied in a low ponytail, tall slim build, warm caramel skin tone, bright expressive smile, wearing a cream oversized travel sweater, light denim jacket, beige wide-leg trousers, standing against a plain neutral gray background, soft even studio lighting, full body and close-up face detail visible, [global style suffix]

*Also generate a 3/4-turn angle of each character using the same prompt with "three-quarter turn portrait" swapped in, for coverage in non-frontal shots.*

---

## B. Location References (generate second, lock as environment references — no characters in frame)

**B1. Airport Arrivals Curb**
> Empty modern airport arrivals pickup curb, glass facade entrance doors, soft overcast daylight, light distant pedestrian traffic and luggage carts, wide establishing shot, no people in foreground, [global style suffix]

**B2. Car Interior**
> Empty view from the back seat of a mid-size sedan interior, dashboard and front seats visible, daylight streaming through the windows, softly blurred city/suburb passing outside, warm interior tones, [global style suffix]

**B3. House Exterior / Driveway**
> Warm suburban house exterior with a driveway, potted plants near the front door, late-afternoon golden-hour light, no car or people, wide establishing shot, [global style suffix]

**B4. Sitting Room**
> Empty cozy living room, neutral-toned sofa, warm floor lamp, family photos framed on the wall, sheer curtains filtering soft afternoon light, tastefully decorated, no people, [global style suffix]

**B5. Hallway**
> Empty short interior hallway with warm wood flooring, muted framed wall art, doorway visible at the far end, soft ambient light, no people, [global style suffix]

**B6. Bedroom**
> Empty softly lit bedroom, linen curtains filtering warm golden light onto a neutral-bedded bed, nightstand with a small lamp, calm and intimate atmosphere, no people, [global style suffix]

---

## C. Per-Clip Still-Frame Prompts (Stage 3 — combine locked character + location references)

> For each, use img2img/character-consistency + environment-lock with the matching Section A and Section B references as inputs.

### Clip 1 — 0:00–0:06 | Airport Arrivals Curb | Daniel, Emily
> [Daniel reference] stands at the airport arrivals curb scanning the crowd, phone in one hand, excited and slightly nervous expression, weight shifting anxiously. In the background near the glass doors, [Emily reference] emerges pulling a rolling suitcase, spotting him and breaking into a wide smile. Medium-wide shot, soft overcast daylight, shallow depth of field on Daniel in foreground, [global style suffix]

### Clip 2 — 0:06–0:10 | Airport Arrivals Curb | Daniel, Emily
> [Daniel reference] and [Emily reference] embracing in a warm, tight hug at the airport curb, both laughing with genuine joy, Emily's suitcase resting beside them, Daniel's hand reaching to take the suitcase handle. Medium shot, eye level, soft overcast daylight, [global style suffix]

### Clip 3 — 0:10–0:16 | Car Interior | Daniel, Emily
> Inside the car, [Daniel reference] driving with both hands relaxed on the wheel, glancing sideways with a warm smile. [Emily reference] in the passenger seat looking out the window, nostalgic soft smile, warm daylight through the glass lighting her face. Over-the-shoulder medium shot from the back seat, [global style suffix]

### Clip 4 — 0:16–0:20 | House Exterior / Driveway | Daniel, Emily
> The car parked in the driveway of a warm suburban house, late-afternoon golden light. [Daniel reference] leaning slightly toward [Emily reference] in the passenger seat, gesturing toward the house with a mischievous grin, finger near his lips in a playful "shh" gesture. Medium shot through the windshield, [global style suffix]

### Clip 5 — 0:20–0:26 | Sitting Room | Daniel, Emily
> Inside the cozy sitting room, [Daniel reference] quietly leading [Emily reference] in by the hand, one finger to his lips in a "shh" gesture, warm afternoon light through sheer curtains. [Emily reference] sitting down on the neutral sofa, glancing around with an anticipatory smile. Wide-medium shot, [global style suffix]

### Clip 6 — 0:26–0:30 | Hallway | Daniel
> [Daniel reference] walking quietly down the warm wood-floored hallway toward a bedroom door at the far end, glancing back once over his shoulder with a playful grin, soft ambient light. Wide tracking shot from behind, [global style suffix]

### Clip 7 — 0:30–0:34 | Bedroom (door) | Daniel
> [Daniel reference] standing at a bedroom doorway, knuckles softly knocking on the door, then slowly pushing it open, peeking in with a gentle, anticipatory expression, warm golden light spilling from within the room. Medium shot from the hallway side, [global style suffix]

### Clip 8 — 0:34–0:39 | Bedroom | Daniel, Sarah
> Inside the softly lit bedroom, warm golden light through linen curtains falling across the bed. [Sarah reference] asleep peacefully on the bed. [Daniel reference] quietly crossing the room and sitting gently on the edge of the bed beside her, tender expression. Soft wide-medium shot, [global style suffix]

### Clip 9 — 0:39–0:45 | Bedroom | Daniel, Sarah
> [Daniel reference] gently touching [Sarah reference]'s shoulder to wake her; she is stirring, eyes fluttering open, disoriented then breaking into a soft smile as she focuses on him. Close-up two-shot, warm intimate golden light, [global style suffix]

### Clip 10 — 0:45–0:51 | Bedroom | Daniel, Sarah
> [Sarah reference] sitting up in bed laughing sleepily, hair tousled. [Daniel reference] holding her hand, pulling her up gently with an excited grin. Sarah's expression shifting to curious excitement. Medium shot, warm morning light, [global style suffix]

### Clip 11 — 0:51–0:55 | Hallway | Daniel, Sarah
> [Daniel reference] and [Sarah reference], now in a blush-pink cardigan over her pajamas, walking together hand-in-hand down the warm-lit hallway toward the sitting room, Sarah curious and smiling, Daniel beaming with anticipation. Wide tracking shot from behind, [global style suffix]

### Clip 12 — 0:55–1:01 | Sitting Room | Daniel, Sarah, Emily
> [Sarah reference] entering the sitting room and freezing mid-step, eyes widening in stunned recognition as she sees [Emily reference] standing and smiling warmly nearby. [Daniel reference] beside her, watching her reaction with a proud smile. Wide shot capturing all three, soft afternoon light, [global style suffix]

### Clip 13a — 1:01–1:10 | Sitting Room | Sarah, Emily
> [Sarah reference] and [Emily reference] embracing in a tight, emotional hug, both with tears of joy and laughter, hands clutching each other's backs. [Daniel reference] visible slightly behind, watching warmly. Medium-close shot, soft warm light, [global style suffix]

### Clip 13b — 1:10–1:20 | Sitting Room | Daniel, Sarah, Emily
> [Daniel reference] and [Emily reference] standing together singing, mouths mid-song, warm joyful expressions, facing [Sarah reference] who sits nearby laughing and wiping happy tears, hand over her heart, overwhelmed with emotion. Wide-medium shot, warm golden afternoon light, [global style suffix]

---

## D. Color Grade Pass (Stage 4)

Apply uniformly to **every** still from Section C before animating:
`warm cinematic color grade, soft golden highlights, lifted shadows, low-medium contrast, warm white balance ~4000K, muted pastel saturation with warm accent glow, subtle soft-edged vignette, fine film grain, Kodak Portra 400 emulation look`

If your pipeline uses a LUT, apply one warm/Portra-style filmic LUT to all 14 stills (13 scene frames + reused clip 13 split) at identical strength (recommend 60–75% intensity) so no frame drifts in tone.

---

## E. Per-Clip Video (Image-to-Video) Prompts (Stage 5)

> Feed each **color-graded** still from Section C as the source frame. Use these motion/camera prompts, generated in scene order for continuity. Duration matches the timing in the production bible.

**Clip 1** (6s) — *Airport Curb*
> Subtle handheld camera drift, Daniel's head turns slowly scanning the crowd, Emily walks forward through the doors pulling her suitcase, natural walking motion, soft ambient airport background movement, gentle breeze in Emily's hair.

**Clip 2** (4s) — *Airport Curb*
> Daniel and Emily step into a hug, arms wrapping naturally, slight rocking motion of the embrace, both laughing, camera holds steady medium shot with slight handheld sway.

**Clip 3** (6s) — *Car Interior*
> Gentle car vibration motion, Emily's head turns slowly from window to Daniel, natural blinking and mouth movement as if mid-conversation, soft motion blur of scenery through the window, Daniel glances over briefly then back to the road.

**Clip 4** (4s) — *Driveway*
> Car settles to a stop, subtle suspension bounce, Daniel turns his head toward Emily and grins, playful shush gesture with slight hand motion, golden light flickering softly through tree leaves outside.

**Clip 5** (6s) — *Sitting Room*
> Daniel leads Emily by the hand across the room with natural walking motion, releases her hand as she sits on the sofa, soft camera push-in, curtains gently swaying from a light breeze.

**Clip 6** (4s) — *Hallway*
> Daniel walks away from camera down the hallway, natural gait, slight camera follow (dolly-in), he glances back over his shoulder mid-stride with a grin, soft ambient light flicker.

**Clip 7** (4s) — *Bedroom Door*
> Daniel's hand knuckles knock softly on the door (subtle motion), door slowly swings open under his push, warm light spilling out and widening across his face as he peeks in.

**Clip 8** (5s) — *Bedroom*
> Daniel walks quietly across the room, sits gently on the bed's edge, slight mattress dip motion, Sarah's chest rises and falls slowly in sleep, soft curtain movement from a light breeze.

**Clip 9** (6s) — *Bedroom*
> Daniel's hand gently touches Sarah's shoulder, subtle rocking motion; Sarah's eyes flutter open naturally, slow focus-and-recognition micro-expression, soft smile spreading across her face, slight head tilt.

**Clip 10** (6s) — *Bedroom*
> Sarah sits up with natural sleepy movement, stretches slightly, Daniel takes her hand and gently pulls her up, both rising off the bed, her expression shifting from sleepy to curious excitement, hair moves naturally with head motion.

**Clip 11** (4s) — *Hallway*
> Daniel and Sarah walk hand-in-hand down the hallway away from camera, natural synced walking motion, slight camera follow, warm light flickering softly as they pass.

**Clip 12** (6s) — *Sitting Room*
> Sarah steps into frame and stops abruptly, natural momentum-stop body motion, eyes widen and mouth opens slightly in shock, Emily's face lights up with a warm smile, Daniel watches with a proud grin, brief freeze-beat before the next clip.

**Clip 13a** (9s) — *Sitting Room*
> Sarah rushes forward into Emily's arms, natural running-into-hug motion, both rock gently side to side in the embrace, visible shoulder-shaking from emotion, Daniel steps in closer behind them smiling, soft camera push-in.

**Clip 13b** (10s) — *Sitting Room*
> Daniel and Emily's mouths move naturally in synced singing motion, gentle swaying, Sarah seated in front of them laughing and wiping tears with natural hand-to-face motion, warm light holds steady, camera holds a soft slow push-in on Sarah's emotional reaction to close the film.

**Audio layer (add after video generation):** sync the dialogue lines from `production-bible.md` Section 4 to clips 9, 10, 12, 13a/13b; add soft ambient room tone throughout, airport ambience under clips 1–2, car road noise under clip 3, and a warm acoustic/piano score bed rising gently from clip 8 through the ending.

---

*All prompts are written for direct copy-paste into image/video generation tools. Keep character and location reference tokens (e.g. "[Daniel reference]") consistent with whatever reference-image or seed mechanism your specific tool uses (img2img input, IP-Adapter, character LoRA, etc.).*
