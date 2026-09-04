# "Kirkolt" — Per-Shot Generation Prompts

Companion to `kirkolt-production-bible.md`. Use in the generation order defined there: **characters → locations → still scenes → color grade → video**. Every prompt below reuses identical descriptive language for characters/locations so identity and environment stay locked across shots — do not paraphrase them between prompts.

**Global style suffix** — append to every still-image prompt (characters, locations, and scenes):
`cinematic film still, moody neo-noir lighting, low-key contrast, teal-and-amber color palette, shallow depth of field, 35mm lens look, shot on film, subtle grain, photorealistic, highly detailed, crime-thriller atmosphere --ar 16:9`

**Global negative prompt** — use for every still-image generation:
`cartoon, illustration, cgi, plastic skin, overexposed, flat bright lighting, cheerful colors, cheerful expression, extra limbs, distorted hands, watermark, text, low detail, HDR halo`

---

## A. Character Reference Sheets (generate first, lock as identity references)

**A1. Investigator Smith**
> Front-facing studio portrait of a 44-year-old man, tall lean-muscular build, close-cropped dark hair greying at the temples, tired hazel eyes with faint under-eye shadows, light stubble, fair-olive skin, a thin old scar through the left eyebrow, weary and guarded expression, wearing a rumpled white dress shirt with sleeves rolled to the forearm, a loosened navy tie pulled low, charcoal trousers, an ID badge clipped to the breast pocket, brown leather wristwatch, standing against a plain neutral gray background, soft even studio lighting, full body and close-up face detail visible, [global style suffix]

**A2. Hannah**
> Front-facing studio portrait of a 58-year-old woman, tall with upright posture, silver-grey hair in a neat low chignon, sharp pale blue-grey eyes, fine lines at the eyes and mouth, fair skin, composed and guarded expression, wearing a charcoal-grey knee-length wool coat over a cream silk blouse, dark tailored trousers, low block-heel boots, a thin grey scarf, carrying a brown leather satchel bag, standing against a plain neutral gray background, soft even studio lighting, full body and close-up face detail visible, [global style suffix]

*Also generate a 3/4-turn angle of each character using the same prompt with "three-quarter turn portrait" swapped in, for coverage in non-frontal shots.*

*For A1, also generate a variant with a dark grey wool overcoat added over the shirt and tie, collar turned up — this is Smith's park-scene layer; keep every other descriptor identical.*

---

## B. Location References (generate second, lock as environment references — no characters in frame)

**B1. Smith's Office**
> Empty detective's office at night, rain streaking down a window, a single desk lamp casting warm light, venetian blinds casting slatted shadows across the room, a case board on the wall covered in photographs of missing men connected with red string and pins, cluttered case files stacked on the desk, moody low-key lighting, wide establishing shot, no people, [global style suffix]

**B2. Harold Park**
> Empty municipal park at night, thick fog drifting low across the ground, a single sodium-vapor lamp post casting a warm amber pool of light over a wooden bench and gravel path, distant blurred city lights beyond a dark tree line, otherwise silent and empty, wide establishing shot, no people, [global style suffix]

---

## C. Per-Clip Still-Frame Prompts (Stage 3 — combine locked character + location references)

> For each, use img2img/character-consistency + environment-lock with the matching Section A and Section B references as inputs.

### Clip 1 — 0:00–0:06 | Smith's Office | Smith
> [Smith reference] sitting alone at his desk in the dim office, rain streaking the window behind him, desk lamp casting warm light across tired features, staring at the case board of missing men on the wall, somber and worn expression. Medium-wide shot, low-key lighting, [global style suffix]

### Clip 2 — 0:06–0:10 | Smith's Office | Smith
> [Smith reference] looking up sharply from his desk toward the office door, startled out of his thoughts, one hand still resting on a case file, desk lamp light on his face. Medium shot, [global style suffix]

### Clip 3 — 0:10–0:16 | Smith's Office | Smith, Hannah
> [Hannah reference] stepping into the office doorway, composed and upright, satchel over one shoulder. [Smith reference] rising from his desk chair, a tense beat of mutual recognition between them. Wide-medium two-shot, low-key lamp light, [global style suffix]

### Clip 4 — 0:16–0:24 | Smith's Office | Smith, Hannah
> [Hannah reference] standing just inside the office, speaking evenly to [Smith reference], who listens with a guarded, tired expression, arms crossed. Rain still visible on the window behind them. Medium two-shot, [global style suffix]

### Clip 5 — 0:24–0:30 | Smith's Office | Smith, Hannah
> [Hannah reference] leaning slightly forward, a knowing look, saying something in confidence. [Smith reference] wary but intrigued, eyebrows drawn, leaning in. Close-medium two-shot, warm lamp light against shadow, [global style suffix]

### Clip 6 — 0:30–0:36 | Smith's Office | Smith, Hannah
> [Hannah reference] glancing toward the door as if checking for eavesdroppers, lowering her voice, speaking to [Smith reference] who nods slowly, understanding the need for secrecy. Medium two-shot, low-key lighting, [global style suffix]

### Clip 7 — 0:36–0:40 | Smith's Office | Smith, Hannah
> [Smith reference] and [Hannah reference] shaking hands firmly across the desk, both with resolute expressions, sealing an unspoken agreement. Medium shot, desk lamp light, [global style suffix]

### Clip 8 — 0:40–0:44 | Smith's Office | Smith
> [Hannah reference] exiting through the office doorway, back to camera, as [Smith reference] watches from behind his desk, the door easing shut, leaving him alone again in the lamp-lit room. Wide shot, [global style suffix]

### Clip 9 — 0:44–0:50 | Harold Park | (no characters)
> Establishing night shot of Harold Park, thick fog drifting low under the sodium-vapor lamp post, empty bench, gravel path glistening faintly, distant blurred city lights, still and silent at 11:30 p.m. Wide shot, [global style suffix]

### Clip 10 — 0:50–0:56 | Harold Park | Smith
> [Smith reference, overcoat variant] walking into the lamplit clearing of the park at night, collar turned up, glancing around cautiously, fog curling around his legs, coming to a stop near the bench. Wide-medium shot, [global style suffix]

### Clip 11 — 0:56–1:02 | Harold Park | Hannah
> [Hannah reference] emerging from the fog along the gravel path, a brown envelope held in one hand against her coat, expression composed and purposeful, amber lamp light catching her face. Medium-wide shot, [global style suffix]

### Clip 12 — 1:02–1:10 | Harold Park | Smith, Hannah
> [Smith reference, overcoat variant] and [Hannah reference] standing face to face under the lamp post, she extends the brown envelope toward him, his hand reaching to take it, both expressions serious. Medium two-shot, amber lamp light against foggy dark background, [global style suffix]

### Clip 13 — 1:10–1:16 | Harold Park | Smith, Hannah
> [Hannah reference] speaking earnestly to [Smith reference], who now holds the envelope against his chest, nodding with quiet gratitude and resolve. Close-medium two-shot, amber lamp light, [global style suffix]

### Clip 14 — 1:16–1:22 | Harold Park | Smith
> [Hannah reference] walking away into the fog, becoming a fading silhouette. [Smith reference, overcoat variant] left in the foreground looking down at the brown envelope, beginning to open the flap, resolute expression under the lamp light. Wide-medium shot, [global style suffix]

---

## D. Color Grade Pass (Stage 4)

Apply uniformly to **every** still from Section C before animating:
`neo-noir teal-and-amber color grade, cool desaturated shadows, warm amber practical highlights, moderate-high contrast, deep detailed blacks, protected warm skin tones, subtle vignette, fine film grain, faint atmospheric haze on exteriors`

If your pipeline uses a LUT, apply one teal-amber crime-thriller LUT to all 14 stills at identical strength (recommend 65–80% intensity) so no frame drifts in tone.

---

## E. Per-Clip Video (Image-to-Video) Prompts (Stage 5)

> Feed each **color-graded** still from Section C as the source frame. Use these motion/camera prompts, generated in scene order for continuity. Duration matches the timing in the production bible.

**Clip 1** (6s) — *Office*
> Subtle handheld camera drift, rain trickles visibly down the window glass, Smith's eyes shift slowly toward the case board, slow blink, chest rising and falling in a tired breath.

**Clip 2** (4s) — *Office*
> Smith's head snaps up toward the door, natural startled micro-expression, hand lifts slightly off the case file, desk lamp light flickers subtly.

**Clip 3** (6s) — *Office*
> Hannah steps forward into the room with natural walking motion, door closing softly behind her, Smith rises from his chair, both hold a still, tense eye-contact beat.

**Clip 4** (8s) — *Office*
> Hannah's mouth moves naturally as she speaks, subtle hand gesture, Smith's arms cross slowly, his expression tightening as he listens, rain continues sliding down the window behind them.

**Clip 5** (6s) — *Office*
> Hannah leans in slightly, natural mouth movement mid-sentence, Smith's eyebrows draw together, he leans in a few inches, lamp light flickers softly across both faces.

**Clip 6** (6s) — *Office*
> Hannah glances toward the door and back, lowers her voice with a subtle head tilt, Smith nods slowly, both speaking in hushed, natural lip movement.

**Clip 7** (4s) — *Office*
> Both hands meet in a firm handshake across the desk, natural grip-and-release motion, brief nod exchanged between them.

**Clip 8** (4s) — *Office*
> Hannah walks toward the door and exits, natural gait, door swings shut with a soft click, Smith remains still, watching, lamp light holds steady on his face.

**Clip 9** (6s) — *Park*
> Fog drifts slowly across the frame in real time, lamp post light flickers faintly, distant tree branches sway gently in a light breeze, otherwise the scene holds still.

**Clip 10** (6s) — *Park*
> Smith walks into frame with natural gait, coat collar catching the breeze, head turning side to side scanning the area, footsteps slow to a stop near the bench.

**Clip 11** (6s) — *Park*
> Hannah emerges from the fog with steady walking motion, envelope held close, fog curling around her legs as she moves, amber light catching her face as she nears.

**Clip 12** (8s) — *Park*
> Hannah extends her arm offering the envelope, natural hand motion, Smith reaches out and takes it, brief shared look, fog drifting softly behind them.

**Clip 13** (6s) — *Park*
> Hannah's mouth moves naturally mid-sentence, subtle earnest hand gesture, Smith nods, holding the envelope against his chest, natural breathing motion.

**Clip 14** (6s) — *Park*
> Hannah turns and walks away, natural gait, gradually dissolving into the fog. Smith looks down, fingers beginning to peel open the envelope flap, slow determined exhale, camera holds a soft push-in on his face to close the film.

**Audio layer (add after video generation):** sync the dialogue lines from `kirkolt-production-bible.md` Section 4 to clips 1 (V.O.), 4, 5, 6, 12, and 13; add soft rain ambience and a distant ticking clock under clips 1–8, night ambience (wind, distant traffic hum, faint owl or insect sound) under clips 9–14, and a low, tense atmospheric score bed that builds gradually from clip 9 through the final push-in on clip 14.

---

*All prompts are written for direct copy-paste into image/video generation tools. Keep character and location reference tokens (e.g. "[Smith reference]") consistent with whatever reference-image or seed mechanism your specific tool uses (img2img input, IP-Adapter, character LoRA, etc.).*
