# Beauty Campaign System: Blueprint v0
**Type:** Agency, reusable across client brands
**Category:** Lip products (gloss, lipstick, balm, liner, tint)
**Market:** India
**Status:** Draft. Built from my own framework, NOT yet aligned to the Lip Gloss Global Prompt Pack (docx) or the digitalarnabofficial.com page. Both were unreadable in this session.

---

## 1. What this system is (simple words)
A repeatable "recipe book" so every campaign for any lip-product client looks consistent, on-brand, and is fast to produce. You change only the inputs (brand, product, shade). The rules do the rest.

**Three layers:**
1. **Brand Input Sheet:** facts about one client (colors, tone, product, price, audience).
2. **Visual Rules:** fixed rules for lighting, background, camera, model, props, color grading.
3. **Prompt + Template Library:** ready AI prompts and Figma templates that combine layers 1 and 2.

## 2. Brand Input Sheet (fill once per client)
- Brand name, tagline, logo, brand colors (hex), fonts
- Product name, type (gloss / lipstick / balm / tint), finish (glassy / matte / satin / shimmer), shade list with hex
- Price band (mass / masstige / premium), hero claim (plumping, hydrating, long-wear, vegan)
- Target audience (age, city tier, skin-tone range, occasion)
- Tone of voice (playful / luxe / clean / desi-festive)
- Do and Don't list (competitors, banned claims, regulated words)

## 3. Visual Rules (core of the system)
| Rule area | What gets defined | India-specific note |
|---|---|---|
| Lighting | Soft beauty light, specular highlight on gloss, warm vs cool | Warm daylight flatters Indian skin tones; avoid washed-out cool light |
| Skin tones | Always show a range (fair to deep, warm/neutral/olive undertones) | Shade-match each lip color to 3+ skin tones |
| Backgrounds | Studio seamless, texture, lifestyle, festive | Festive set: Diwali, Karwa Chauth, wedding season, Holi, Eid |
| Camera | Macro lip close-up, product flat-lay, portrait, texture swatch | Mobile-first vertical 9:16 and 4:5 |
| Product shots | Hero, texture smear, cap-off, in-hand | Show true color accuracy |
| Props | Minimal / floral / jewelry (jhumka, bindi, maang tikka used tastefully) | Avoid stereotypes |
| Color grading | One LUT or look per brand | Keep skin natural, not over-smoothed |
| Models | Diversity of age, skin tone, features | Consent and likeness rules if using AI faces |

## 4. Campaign Modules (the reusable pieces)
1. Product hero (packshot)
2. Texture and swatch (gloss shine, smear, drip)
3. Model beauty close-up
4. Shade-range lineup
5. Lifestyle / festive scene
6. Ad creative (static, carousel, reel cover)
7. Marketplace images (Nykaa, Amazon, Myntra, Flipkart)
8. Influencer brief and UGC guide

## 5. Prompt formula (for AI image/video tools)
`[Subject] + [Product and finish] + [Shade] + [Skin tone/model] + [Pose and framing] + [Lighting] + [Background] + [Camera/lens] + [Color grade] + [Mood] + [Aspect ratio] + [Avoid list]`

Example skeleton:
> Macro close-up of lips wearing {shade} {finish} lip gloss, {skin tone and undertone} skin, soft warm key light with crisp specular highlight, {background}, 100mm macro, shallow depth of field, natural skin texture, {mood}, 4:5. Avoid: over-smoothing, plastic skin, warped lips, extra teeth, garbled text.

## 6. Figma library plan (built in phase 2 via figma-generate-library)
- **Variables:** brand colors, shade palette, neutral/background colors, spacing, radius. Light/Dark modes. Brand mode per client (this is what makes it agency-reusable).
- **Text styles:** headline, subhead, body, price, legal/disclaimer.
- **Components:** Shade swatch, Price tag/badge, Claim badge, CTA button, Logo lockup, Product card.
- **Templates:** IG post 4:5, Story/Reel 9:16, Marketplace tile 1:1, Festive banner, Carousel set.

## 7. Open items needed from you
1. The docx content and the link content (paste text or commit to repo)
2. First client or sample brand to build the pilot on
3. Figma: an existing file or a new one (and team/plan)
4. Languages needed (English / Hindi / Hinglish)
5. Which AI tools you use (Midjourney, Firefly, Higgsfield, Nano Banana, etc.)
6. Regulatory and claim restrictions to bake in
