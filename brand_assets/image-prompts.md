# Image Prompts — Albuquerque Water Softener Site

24 AI image-generation prompts, one per photo the site needs. Modeled on
the Tampa site's already-live photography (`watersoftenertampafl/src/assets/images/`)
so the whole portfolio reads as one professional photo library, not 6
different stock-photo styles — same photorealistic equipment/interior
shots, reskinned exterior shots for Albuquerque's high-desert Southwest
setting instead of Tampa's palm-tree Florida look.

Paste each prompt as-is into an AI image generator (Midjourney, Flux,
DALL-E, Ideogram). Save the result using the exact filename given, drop it
into `src/assets/images/`, then wire it into the matching page via the
`image` prop on `<PageHero>` (inner pages) or a direct `<Image />` import
(homepage) — same pattern Tampa already uses. No page-content edits are
needed beyond adding the import + prop.

## Shared style block — prepend to every prompt below

```
Photorealistic professional stock/real-estate photography, natural daylight,
shallow depth of field, sharp focus on the main subject, no text, no
watermark, no logo, no illustration or 3D-render look. If a person appears:
crop at the neck/shoulders or shoot hands/torso only — never show a face.
No stock-photo clichés (no family smiling at a glass of water, no clipart
water-drop icons). Cool-neutral color grading on interior/equipment shots;
warm, clear high-desert daylight on exterior shots.
```

## Albuquerque exterior/context cues — use only on shots marked "EXTERIOR"

```
Southwestern Pueblo-Revival or Territorial-style architecture: adobe-tone
stucco walls in warm tan, terracotta, or earth brown; flat or low-pitched
roofs; exposed vigas (roof beam ends) where visible; xeriscaped yard —
gravel, native rock, agave, yucca, piñon or juniper shrubs, NOT grass lawns
or palm trees; Sandia Mountains visible as a soft ridge on the horizon;
big clear blue high-desert sky, bright sunlight.
```

---

## Homepage (3 images)

### 1. `hero-softener.webp` — homepage hero
Aspect ratio ~5:4 (1120x960 reference)
```
A modern water softener system installed in a home laundry/utility room,
white resin tank and brine tank connected by copper piping with a digital
control head display, positioned against a warm terracotta-stucco wall.
Tile flooring. A small window shows a glimpse of xeriscaped desert
landscaping outside — gravel and a piñon shrub. Clean, well-lit, no
clutter. [+ shared style block]
```

### 2. `installation-tile.webp` — homepage alternating section
Aspect ratio ~3:2 (1264x848 reference)
```
Close crop on a technician's gloved hands connecting a copper pipe fitting
to a new water softener control head, wrench in hand, mid-installation.
Shot from the side/below so no face is visible — hands, forearm, and torso
of a grey work shirt only. Utility room background, soft-focus. [+ shared
style block]
```

### 3. `hard-water-tile.webp` — homepage alternating section
Aspect ratio ~3:2 (1264x848 reference)
```
Extreme close-up of chalky white mineral scale (limescale) buildup
crusted on a bathroom faucet spout and showerhead nozzle, chrome fixture
against pale blue tile. Macro-lens detail on the mineral texture. [+
shared style block]
```

---

## Inner pages (21 images, ~16:9, 1408x768 reference)

### 4. `about-header.webp`
```
EXTERIOR. A technician (cropped at the neck, grey work uniform, tool bag
over one shoulder, blue nitrile glove visible on one hand) standing in the
driveway of a single-story Southwestern stucco home, a plain white service
van parked behind him in the driveway. Xeriscaped front yard, Sandia
Mountains faint on the horizon, morning light. [+ shared style block] [+
exterior cues]
```

### 5. `brine-tank-cleaning-header.webp`
```
Close-up of a technician's gloved hands lifting the lid off a brine tank,
revealing a hardened salt bridge crust inside against the white tank
walls. Utility-closet interior, copper piping visible in the background.
No face. [+ shared style block]
```

### 6. `comparison-header.webp`
```
Two different water treatment units — a traditional salt-based softener
tank with digital control head, and a slim salt-free conditioner
cartridge — standing side by side on a light countertop in a utility
room, both in sharp focus for direct comparison. Neutral background. [+
shared style block]
```

### 7. `contact-header.webp`
```
EXTERIOR. A technician's hand (no face) ringing a doorbell / knocking at
the front door of a Southwestern stucco home with a covered portal
(porch), clipboard tucked under the other arm. Terracotta stucco, wood
door, desert landscaping visible at the frame edges. [+ shared style
block] [+ exterior cues]
```

### 8. `control-head-repair-header.webp`
```
Close-up of gloved hands using a small screwdriver to open the digital
control head unit on top of a softener tank, wires and circuit board
partially visible, diagnostic multimeter probe touching a contact point.
No face. Utility room, copper pipe in soft focus behind. [+ shared style
block]
```

### 9. `faq-header.webp`
```
A clean, well-organized utility-closet shot of a full water softener
system — resin tank, brine tank, digital control head, copper inlet/outlet
piping labeled with small tags — shot straight-on, nobody in frame, bright
even lighting. [+ shared style block]
```

### 10. `free-water-test-header.webp`
```
Close-up of a hand (no face, forearm in a work-shirt sleeve) holding a
water hardness test strip over a labeled test vial at a kitchen sink,
water running from a modern faucet in the background, quartz countertop.
[+ shared style block]
```

### 11. `hard-water-header.webp`
```
Macro close-up of a glass shower door with heavy white mineral spotting
and streaking, water droplets beaded on the surface, soft bathroom light
behind. [+ shared style block]
```

### 12. `installation-header.webp`
```
Close-up on copper pipe fittings being soldered/connected at the inlet of
a new water softener tank, a technician's gloved hand holding a wrench in
frame, control head visible above. Utility room, natural window light. No
face. [+ shared style block]
```

### 13. `neighbourhood-header.webp`
```
EXTERIOR. A quiet residential street in a Southwestern Albuquerque
neighborhood at golden-hour morning light: single-story adobe-tone stucco
homes with flat/low-pitched roofs, xeriscaped front yards with gravel and
native desert shrubs, the Sandia Mountains visible along the horizon under
a wide blue sky. No palm trees, no grass lawns. [+ shared style block] [+
exterior cues]
```

### 14. `new-construction-header.webp`
```
EXTERIOR. A newly framed or freshly stuccoed Southwestern home under
construction, stubbed copper plumbing rough-in visible at an exterior
wall, scaffolding or building materials neatly stacked nearby. Clear
desert daylight, dry earth-toned construction site. [+ shared style block]
[+ exterior cues]
```

### 15. `products-header.webp`
```
A clean lineup of three different water treatment products — a salt-based
softener tank, a slim salt-free cartridge unit, and a compact reverse
osmosis under-sink system — arranged on a light showroom-style shelf or
counter, evenly lit, nobody in frame. [+ shared style block]
```

### 16. `quote-header.webp`
```
Close-up of a technician's hands (no face) writing on a clipboard estimate
form, a tablet showing a house diagram beside it, water softener tank
visible in soft focus in the background of a home utility room. [+ shared
style block]
```

### 17. `repair-header.webp`
```
Close-up of a gloved hand holding a multimeter probe against the digital
control head of an older, slightly worn water softener unit, diagnosing a
fault. Copper piping and a home's utility-closet wall in the background.
No face. [+ shared style block]
```

### 18. `resin-bed-replacement-header.webp`
```
Close-up of a technician's gloved hands pouring fresh amber resin beads
from a bag into an open softener tank, beads mid-pour, tank rim in sharp
focus. No face. [+ shared style block]
```

### 19. `reverse-osmosis-header.webp`
```
Close-up of an under-sink reverse osmosis system being installed —
multiple slim filter cartridge housings mounted in a row with connecting
tubing, a gloved hand tightening a fitting, cabinet interior with a
supply line visible. No face. [+ shared style block]
```

### 20. `salt-based-installation-header.webp`
```
Close-up of white water-softener salt pellets being poured from a bag
into a brine tank opening, pellets mid-pour catching the light against the
tank's white plastic rim. No face. [+ shared style block]
```

### 21. `salt-free-installation-header.webp`
```
A slim, tankless salt-free water conditioner unit mounted directly to a
wall with minimal copper piping — compact footprint, no bulky tanks,
clean utility-room wall, natural light. No face. [+ shared style block]
```

### 22. `water-quality-header.webp`
```
A glass being filled with clear water at a modern kitchen faucet, water
mid-stream catching the light, quartz countertop, soft-focus kitchen
background. No face, hand only optionally at the tap handle. [+ shared
style block]
```

### 23. `water-softener-sizing-header.webp`
```
Close-up of a technician's gloved hands holding a tape measure against a
copper supply pipe, a small notepad with handwriting nearby, softener
tank in soft focus in the background of a utility room. No face. [+
shared style block]
```

### 24. `whole-home-filtration-header.webp`
```
Close-up of a whole-home filtration cartridge housing mounted on copper
piping, visible sediment buildup inside the clear housing, a gloved hand
entering frame at the edge adjusting a nearby valve. Utility room, natural
window light. No face. [+ shared style block]
```

---

## Notes
- Filenames match the Tampa site's convention exactly so the import
  pattern (`import headerImage from "../assets/images/<name>.webp"`) can
  be copied directly once images are generated and saved.
- All facts implied by these prompts are visual/staging only — no city
  data, pricing, or business claims are embedded in imagery, so this list
  carries none of the `[PLACEHOLDER]` data-gap concerns the written page
  content has.
- Homepage is the only page not using `<PageHero>`, hence its 2 different
  images (`hero-softener`, `installation-tile`, `hard-water-tile` — 3
  total) plus a separate import pattern; see Tampa's `index.astro` for the
  exact reference wiring.

---

## About page — 6 additional images

The About page (`src/pages/about/index.astro`) currently renders these 6
slots as `placehold.co` graphics — the hero image already has real
photography (`about-header.jpg`, done). Generate these 6, save with the
exact filenames below into `src/assets/images/`, and they can replace the
`placehold.co` `<img>` blocks with real `<Image>` imports the same way the
other 21 headers were wired in.

Aspect ratio: all six are wide (~900x400 or 900x300, matching the current
placeholder dimensions in the page source) since they sit as full-width
banner images between sections, not side-by-side with text like the
`PageHero` headers.

### 25. `about-before-after.jpg` — "What We Do" section
```
A split-frame photorealistic comparison image, divided by a thin vertical
line down the center. Left half: a chrome bathroom faucet and showerhead
crusted with heavy white mineral scale buildup, dull and spotted. Right
half: an identical chrome faucet and showerhead, completely clean and
gleaming, with a few clear water droplets. Same camera angle, framing, and
lighting on both halves so the only difference is the scale buildup. No
text or labels overlaid — this is a photo, not an infographic. [+ shared
style block from the top of this file]
```

### 26. `about-team-working.jpg` — "What Makes Us Different" section
```
Two technicians in matching grey work uniforms working together on a water
softener installation in a home utility room — one holding a wrench at a
copper pipe fitting, the other holding a tablet or clipboard nearby. Crop
both at the neck/shoulders or shoot from behind/the side — no faces
visible, consistent with every other technician shot on this site. Copper
piping and a softener tank in frame, natural window light. [+ shared style
block]
```

### 27. `about-homeowner.jpg` — "Who Uses Our Services" section
```
A homeowner's bare hand (no glove, unlike the technician shots — this is a
homeowner, not staff) filling a drinking glass at a modern kitchen faucet,
morning light, a coffee mug and a small potted plant softly out of focus
on the counter behind. Warm, lived-in domestic mood rather than a showroom
look. No face, no posed family, no clinking-glasses cliché — just a quiet
everyday moment. [+ shared style block]
```

### 28. `about-founders.jpg` — "Team" section
```
Two tradespeople in grey work uniforms standing together in a home utility
room or driveway, arms crossed or one gesturing mid-conversation, candid
rather than a posed studio headshot — this should read as "caught during a
work day," not a corporate stock photo. Unlike every other photo on this
site, faces ARE visible here since this is specifically a founders/team
portrait. Natural daylight, approachable and confident expressions, no
exaggerated smiling-at-camera stock-photo look. [+ shared style block,
EXCEPT ignore the "never show a face" line for this one image only]
```

### 29. `about-process-steps.jpg` — "How It Works" section
```
Note: this slot is a 4-step process explainer, not a documentary photo —
an AI photo generator will struggle to render clean, readable step
numbers/icons. Two options:
  (a) Skip the image generator entirely and build this as a coded 4-icon
      row instead (SVG icons + labels, matching the site's existing inline-SVG
      icon convention per CLAUDE.md) — this will look cleaner and stays
      on-brand with zero risk of AI-garbled text.
  (b) If a photo is still wanted here, use a wide establishing shot instead
      of a literal diagram: a technician's hands laying out water-test
      strips, a wrench, and a tablet in a neat row on a clipboard/counter,
      top-down flat-lay composition, suggesting "a clear process" without
      needing rendered text. [+ shared style block]
Recommendation: (a).
```

### 30. `about-water-closeup.jpg` — FAQ section
```
Extreme macro close-up of clear water actively pouring/splashing into a
glass, mid-motion with visible ripples and bubbles, backlit so the water
catches the light, dark neutral background so the water itself is the only
subject in frame. No faucet, no hand, no glass rim visible — pure water in
motion, abstract and clean. Distinct from `water-quality-header.jpg`
(which shows a full faucet-and-glass scene) so the two don't read as
duplicates. [+ shared style block]
```
