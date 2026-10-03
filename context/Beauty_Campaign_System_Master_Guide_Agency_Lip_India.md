# Beauty Campaign System: Master Guide (v1)
**For:** Agency use, lip products, India market, English + Hinglish
**Built from:** (1) Lip Gloss Global Product Prompt Pack (docx + web page), (2) the pilot brand's reference-board visual direction
**AI tools:** Gemini, ChatGPT (image), Magnific, Google Flow
**Status:** Docs phase complete. Figma library comes next (see Section 9).

---

## 1. What the Prompt Pack actually teaches (analysis in easy words)

The pack looks like "10 pretty prompts", but the real value is the **system hiding inside it**. It works on one idea: **LOCK what must never change, VARY only what is allowed to change.**

| Part of the pack | What it does | Why it matters |
|---|---|---|
| **Universal Product Lock** | A paragraph describing the exact bottle, cap, logo band, gloss. Pasted into every prompt. | AI tools love to "redesign" products. This stops that. Product stays real. |
| **Shade Lock (#D18878)** | One hex + words: undertone, shimmer, finish. | Color is the first thing AI drifts. Hex + words pins it. |
| **Universal Negative Direction** | A "never do this" list: fake text, extra fingers, plastic skin, wrong product. | Removes the most common AI failures in one block. |
| **10 concept prompts** | Each has: scene, material, light, camera, mood, ratio, "Best for". | Each is a different campaign *route*, same product. |
| **Quick Global Variables** | PRODUCT, SHADE, ENVIRONMENT PALETTE, MATERIAL, CAMERA, LIGHTING, REALISM, OUTPUT. | This is how you reuse the pack for any other product or shade. |
| **4-step workflow (web page)** | Choose prompt, upload reference, replace variables, generate and refine ONE variable at a time. | Prevents "change everything, lose everything". |

### Strengths
- Product fidelity protection is excellent.
- Prompts are copy-ready and consistent in structure.
- Every concept has a use-case ("Best for"), so strategy is built in.
- The variables table makes it reusable.

### Gaps (this is where your agency system adds value)
1. **No India context:** no skin-tone range, undertone matching, festivals, or Indian beauty-platform formats.
2. **No Hinglish/copy layer:** every prompt says "no added text". The pack never says how text gets added.
3. **Style clash risk:** several concepts (Red Ribbon, Burgundy Satin, Chessboard) are dark and dramatic. The pilot brand board is soft, powdery, warm and minimal. Not every concept fits.
4. **Model likeness and realism rules are thin:** only a short realism line. No consent or "AI face" policy.
5. **No quality check (QC) list:** nothing tells you when an output is "approved".
6. **Tool-specific steps missing:** nothing about which tool to use for which stage.
7. **Only 3 ratios named:** 3:4, 9:16, 1:1. Missing 4:5 and marketplace and banner sizes.
8. **No campaign planning:** no sequence (teaser, launch, sustain), no calendar.

---

## 2. The system architecture (6 layers)

```
LAYER 0  LOCKS         Product Lock + Shade Lock + Negative Direction   (never changes)
LAYER 1  BRAND THEME   Palette, light, materials, mood, composition     (changes per client)
LAYER 2  CONCEPTS      Scene routes (the 10 + your new ones)            (pick one per shot)
LAYER 3  VARIABLES     Model, skin tone, occasion, material, camera, light, ratio
LAYER 4  OUTPUT        Figma templates: text, logo, price, CTA, English/Hinglish
LAYER 5  QC LOOP       Checklist, fix ONE variable at a time, approve, archive
```

**Golden rules**
1. Layer 0 is pasted first, unchanged, every time.
2. Change one thing per re-generation.
3. AI makes the picture. **Figma adds all text and logos.** Never let AI write text on packaging or ads.
4. Each client gets their own Layer 1. Layers 0, 2-5 are reusable.

---

## 3. Layer 0: Locks (ready to reuse)

Template for any new product (replace the bracketed parts). Pilot example uses the real pack text.

**PRODUCT LOCK template**
> Use the exact uploaded [PRODUCT] as the hero object. Preserve [body shape], [cap/closure], [packaging], [logo/band details], exact proportions, material transitions and the real [formula] visible inside. The shade must remain [SHADE WORDS], approximately [#HEX]. Do not redesign, simplify, relabel, recolor, reshape, or convert the product into any other product type.

**SHADE LOCK format:** `#HEX + undertone + shimmer/finish + how it reflects light`
Pilot: `#D18878, warm peach-coral nude, muted rosy undertone, fine rose-gold + champagne micro-shimmer, glossy translucent luminous.`

**NEGATIVE DIRECTION (keep as is, add India-specific items)**
Original list + add: *no lightened or bleached skin tone, no mismatched undertone, no stereotyped styling, no garbled Devanagari or Latin text, no cultural costume clichés unless the concept asks for them.*

---

## 4. Layer 1: Pilot brand theme (from the reference board)

**Core feel:** soft luxury, contemporary femininity, tactile materials. Polished but not over-glossy. Premium but not cold. Minimal but not sterile. Pink is a refined *accent*, never the loud commercial pink.

**Mood words:** Elegant, Soft, Feminine, Contemporary, Sensual, Refined, Calm, Premium, Tactile, Minimal.

**Palette (proposed starting values, confirm against the real board and client)**
| Role | Name | Hex (proposed) |
|---|---|---|
| Background light | Soft ivory | `#F8F1EA` |
| Background base | Creamy beige | `#EBDDCF` |
| Soft accent | Powder pink | `#EBC9C4` |
| Muted nude | Warm nude | `#D9B5A3` |
| **Product shade (locked)** | Peach-coral nude | `#D18878` |
| Depth / text | Restrained cocoa | `#5A3A32` |
| Rare dramatic accent | Deep burgundy | `#5E1F2B` |

**Lighting rules**
- Soft diffused studio light, large apparent light source, smooth gradients.
- Controlled specular highlights on gloss and packaging, never blown out.
- Gentle contact shadows, soft edge falloff, warm-neutral white balance.
- Shadows lean warm brown/beige, not black.

**Material language:** translucent and semi-gloss cosmetics, glass/acrylic/clean metal details, satin and velvet-matte, creamy textures, soft reflective surfaces, fine macro detail. Key contrast: **soft matte vs controlled gloss**, not everything shiny.

**Composition rules:** hero product dominant, clear foreground-midground-background, generous negative space on purpose, straight-on or subtle three-quarter or controlled macro, no exaggerated lens distortion, remove anything that doesn't help product recognition or premium feel.

**One-line summary (use as a header in every prompt):**
> Soft warm palette + tactile materiality + diffused premium lighting + strong product hierarchy + intentional negative space + editorial macro detail.

---

## 5. Layer 2: Concept routes, fit check against the pilot theme

| # | Concept | Fit with soft-luxury theme | Use for |
|---|---|---|---|
| 07 | Soft Sculptural Peach Architecture | **Perfect** | Website hero, e-commerce banner |
| 09 | Acrylic Vanity + Satin | **Perfect** (keep satin champagne-blush; use burgundy sparingly) | Luxury still life, gifting |
| 04 | Molten Liquid-Glass Platform | **Strong** | Launch poster, hero |
| 10 | Futuristic Metallic Folds | **Strong** (keep pearl/blush, cool highlights light) | Launch cover, ad cover |
| 03 | Gloss-Dipped Jewelry Hand | **Good** (warm ivory background; jewellery can be Indian gold styling) | Surreal key visual |
| 08 | Retro Turntable Pastel Set | **Medium** (mint is off-palette; swap to blush/cream) | Reels cover, collab |
| 02 | Faux-Fur Gen-Z Editorial | **Medium** (playful; tone down) | Model-led social |
| 05 | Burgundy Satin Nest | **Accent only** | Festive, dark-luxury moments |
| 01 | Red Ribbon Beauty Portrait | **Accent only** | Festive, wedding season, shade storytelling |
| 06 | Queen of the Chessboard | **Off-theme** | Brand-statement concept only |

**New India routes to add (Layer 2 extension)**
- **N1. Festive Glow:** Diwali / wedding season. Warm gold bokeh, ivory and blush, brass diya glow as light source, kept soft not loud.
- **N2. Shade-Match Lineup:** one product, three or more skin tones, same light, same framing. Pure shade proof.
- **N3. Everyday Desk-to-Dinner:** small lifestyle still life (handbag, mirror, soft sunlight).
- **N4. Texture Macro:** gloss smear, droplet, wand pull. Cosmetic texture close-up.
- **N5. Hinglish Social Pack:** simple clean image + text overlay done in Figma.

---

## 6. Layer 3: Variables (expanded for India)

| Variable | Pack rule | India add-on |
|---|---|---|
| PRODUCT | Exact uploaded ref, never redesign | Same |
| SHADE | Shade + undertone + finish + shift | Always test on at least 3 skin tones: fair-neutral, medium-warm (wheatish), deep-warm |
| MODEL | (not defined) | Indian skin-tone range and undertones, real texture, hair and features natural, age range stated. No bleaching or flattening of tone |
| ENVIRONMENT PALETTE | Tonal or complementary, don't contaminate product | Use theme palette in Section 4 |
| MATERIAL | Satin, acrylic, liquid glass, marble, lacquer, metal, paper/plaster | Add: brass, raw silk (sparingly), flower petals (marigold, rose), matte ceramic |
| CAMERA | Macro/85-100mm luxury, low angle power, 45 degree still life | Same |
| LIGHTING | Large diffused key + rim + true reflections | Warm-neutral. Check Indian skin does not go grey or orange |
| REALISM | Pores, weave, imperfections, true refraction | Same, plus "natural lip lines" |
| OUTPUT | 3:4, 9:16, 1:1 | Add: **4:5** (feed), **1.91:1** (link/ad banner), **16:9** (YouTube/web), marketplace **1:1** white-ish bg versions |

---

## 7. Tool roles (Gemini, ChatGPT, Magnific, Google Flow)

| Stage | Best tool | Job |
|---|---|---|
| 1. Generate stills with product reference | **Gemini** (image with reference upload) | First pass of each concept; test product fidelity |
| 2. Targeted edits / fixes / text-safe edits | **ChatGPT image** | "Change only the background", fix a hand, adjust colour; conversational one-variable edits |
| 3. Detail and skin realism upscale | **Magnific** | Upscale, add micro-texture. Keep creativity LOW so the product doesn't change |
| 4. Motion for Reels | **Google Flow** | Animate approved stills: slow camera push, gloss shimmer, fabric movement |
| 5. Layout, text, logo, price | **Figma** | All typography in English/Hinglish, grids, templates |

**Important:** exact capabilities and settings of these tools change often. Treat the above as the working plan and confirm in a 5-image test on your pilot brand.

**Pipeline per asset:** Paste Layer 0 + Layer 1 header, then Layer 2 concept, then Layer 3 variables. Generate in Gemini. Check against QC list. Fix one variable in ChatGPT. Upscale in Magnific. Place into the Figma template. Animate in Flow if needed.

---

## 8. Layer 4 and 5: Output and QC

### Hinglish copy layer (examples; always native-review before publishing)
| Use | English | Hinglish |
|---|---|---|
| Hero line | Shine that speaks for you | Shine jo khud bole |
| Shade line | Your everyday peach-coral nude | Aapka everyday peach-coral nude |
| Texture | Glass-like gloss, zero stickiness | Glass jaisa gloss, bilkul non-sticky |
| Festive | Glow into the festive season | Festive season mein glow karo |
| CTA | Shop now | Abhi shop karein |

Rule: claims (non-sticky, hydrating, long-lasting) must be approved by the client and be provable.

### QC checklist (every output)
**Product:** shape, cap, logo band, proportions correct. No invented text. Gloss visible inside.
**Color:** shade matches #D18878 on the product; environment hasn't tinted it.
**Skin/model:** realistic pores and lip lines; hands and fingers correct; tone and undertone natural; no over-smoothing.
**Light/material:** soft warm-neutral light; highlights not blown; shadows keep detail.
**Brand fit:** palette, mood, negative space follow Layer 1.
**Compliance:** no unapproved claims, AI-person policy followed, no real person's likeness.
**Output:** correct ratio, resolution, file name.

**Refine rule:** one variable per round (background, OR light, OR pose, OR crop). Never change two.

### File naming
`[Client]_[Product]_[Concept#]_[Variant]_[Ratio]_[v#]` e.g. `Pilot_LipGloss_07_Peach-Architecture_3x4_v2`

---

## 9. Figma library plan (next phase)

**Scope:** Full library, agency-reusable. Tokens first, then components, then templates.

**Collections**
- **Primitives:** ivory, beige, powder pink, nude, shade `#D18878`, cocoa, burgundy, neutrals.
- **Color (semantic):** modes = `Pilot Soft Luxury`, `Festive Dark` (extendable per client).
- **Spacing / Radius:** 4-pt scale.
- **Typography:** heading, body, caption, price, legal, plus Hinglish-safe fonts (Latin + Devanagari support).

**Components:** Logo lockup, Shade swatch, Claim badge, Price tag, CTA button, Product card, Disclaimer strip.
**Templates:** Feed post 3:4 and 4:5, Story/Reel 9:16, Square 1:1, Web banner 16:9, Ad 1.91:1, Marketplace tile, Carousel set.
**Pages:** Cover, Getting Started, Foundations, Components, Templates, Prompt Library (reference), QC.

**Figma plan found:** "Pooja Jalwan's team" (Full seat, admin). **Still blocked on:** pilot brand name, logo, fonts, and palette confirmation.

---

## 10. Still needed from you
1. (Done) Figma plan: Pooja Jalwan's team.
2. Pilot brand name, logo, and preferred fonts (or approval to propose them).
3. Confirmation of the proposed palette in Section 4 against the real board.
4. Permission to add the 5 new India routes (N1-N5) and 4:5 ratio as standard.
5. Any claim restrictions or compliance rules from the client.
