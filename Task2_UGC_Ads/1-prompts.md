# 📋 Task 2 — UGC Ad Prompt Engineering System
## AI Content Marketing using UGC Ads — GlowUp Face Serum
**Intern:** Bora Karthik | **CIN:** FIT/MAR26/PE2027 | **Track:** Prompt Engineering (PE)
**Repository:** FUTURE_PE_02 | **Tool Used:** Claude AI
**Product:** GlowUp Vitamin C Face Serum — D2C Skincare Brand

---

## 🧠 Prompt Architecture: HOOK-BODY-CTA Framework

All UGC ad prompts follow the **HBC-X Framework** — a professional UGC ad engineering structure used at top D2C growth agencies:

| Layer | What It Does |
|-------|-------------|
| **H** — Hook | First 3 seconds — scroll-stopping opener that creates pattern interrupt |
| **B** — Body | Problem → Agitation → Solution storytelling in authentic voice |
| **C** — CTA | Conversion action with urgency trigger and friction reducer |
| **X** — eXecution | Platform-specific format rules, tone calibration, forbidden phrases |

**Why UGC works:** UGC (User Generated Content) style ads outperform branded ads by 4x because viewers trust real people. The key is making AI-generated scripts sound like a real person talking — not a brand advertisement.

---

## 🔷 PROMPT 1 — System Context Prompt
> **Purpose:** Run FIRST in every session. Sets the expert UGC creator persona before any script is generated.

```
You are AdScript-Pro, a senior UGC content strategist and performance
marketing specialist with 12+ years of experience creating viral ad
scripts for top D2C brands on Instagram, YouTube, and Facebook.

You have written high-converting UGC scripts for brands like
Mamaearth, Minimalist, Plum, and WOW Skincare in the Indian market.

OPERATING RULES:
1. Every script must sound like a REAL PERSON talking to camera —
   not a brand advertisement. No corporate language ever.
2. The hook must cause a pattern interrupt in the first 3 seconds.
   If the viewer doesn't stop scrolling in 3 seconds, the ad fails.
3. Use conversational Indian English — natural, warm, relatable.
4. Every script follows: Hook → Problem → Agitation → Solution → Proof → CTA
5. Forbidden phrases: "clinically proven", "revolutionary", "game-changer",
   "you won't believe", "limited time offer", "act now". These kill trust.
6. Every CTA must feel like a friend's recommendation — not a sales push.
7. Scripts must be platform-optimised: different length and energy for
   Instagram Reels (15-30s), YouTube Shorts (30-60s), Facebook Feed (45-60s).
8. Always include: Hook variants (3 per script), body script, CTA options (2),
   and caption with hashtags.
```

---

## 🟢 PROMPT 2 — Product Brief
> **Purpose:** Passed after system prompt. Defines the product, audience, and positioning before any script is generated.

```
PRODUCT PROFILE:
  Brand Name      : GlowUp
  Product         : Vitamin C Brightening Face Serum
  Price Point     : ₹599 (affordable premium)
  Key Ingredients : 15% Vitamin C, Niacinamide, Hyaluronic Acid
  Claims          : Brightens skin in 14 days, reduces dark spots,
                    evens skin tone, hydrates deeply
  Certifications  : Dermatologist-tested, Cruelty-free, No parabens
  Target Customer : Indian women aged 18-32, skin concerns: dullness,
                    dark spots, uneven tone, oily/combination skin
  Competitor Gap  : Premium serums cost ₹1500-3000. GlowUp delivers
                    same results at ₹599.

AUDIENCE PAIN POINTS (ranked):
  1. Dull, tired-looking skin (especially after screens all day)
  2. Dark spots from sun exposure and acne marks
  3. Expensive serums that don't work for Indian skin tones
  4. Confusing ingredients — don't know what actually works
  5. Wants visible results, not just promises

BRAND VOICE:
  Tone     : Honest, relatable, like your best friend who has great skin
  Language : Conversational Hindi-English mix acceptable (Hinglish)
  Emotion  : Empowerment, confidence, not insecurity or shame
  Avoid    : Fair skin obsession, whitening language, shame-based hooks

CONVERSION GOAL: Drive purchase via Instagram/YouTube link in bio
```

---

## 🔵 PROMPT 3 — Hook Generator Prompt
> **Purpose:** Generates 10 scroll-stopping hooks for the product. Hooks are the most critical part of any UGC ad.

```
ROLE + CONTEXT: [System Prompt + Product Brief loaded above]

TASK — Generate 10 scroll-stopping hooks for GlowUp Vitamin C Serum.

HOOK RULES:
  - Maximum 15 words each
  - Must cause pattern interrupt (surprise, curiosity, relatability, or controversy)
  - NO questions starting with "Do you..." or "Are you..." — too generic
  - Must feel like a real person starting a genuine conversation
  - Each hook must use a DIFFERENT trigger type (see below)

Generate 2 hooks for EACH trigger type:

  [TRIGGER 1] RELATABILITY HOOK
    The viewer thinks: "Oh my god, that's literally me."
    Example structure: "Me at 6am vs me after [product]..."

  [TRIGGER 2] CONTROVERSY HOOK
    The viewer thinks: "Wait, that's not what I expected."
    Example structure: "I stopped using [expensive brand] and here's what happened..."

  [TRIGGER 3] RESULT HOOK
    The viewer sees the outcome first, wants to know how.
    Example structure: "14 days. That's all it took to [result]."

  [TRIGGER 4] PROBLEM HOOK
    The viewer feels instantly seen and understood.
    Example structure: "If your skin looks dull no matter what you try..."

  [TRIGGER 5] CURIOSITY HOOK
    The viewer has to keep watching to get the answer.
    Example structure: "The one ingredient your skincare is probably missing..."

FORMAT: For each hook, add:
  - Trigger type label
  - Hook text
  - Why it works (1 sentence)
  - Best platform for this hook
```

---

## 🟡 PROMPT 4 — Full Ad Script Generator
> **Purpose:** Generates complete UGC ad scripts for 3 platforms with full Hook → Body → CTA structure.

```
ROLE + CONTEXT: [System Prompt + Product Brief loaded above]
Use the best hooks from Prompt 3 output.

TASK — Generate 3 complete UGC ad scripts:

  [SCRIPT 1] INSTAGRAM REELS — 15 to 30 seconds
    Format: Talking-head style. Fast cuts. High energy.
    Structure:
      - Hook (0-3 sec): [Use Relatability or Result hook]
      - Problem (3-8 sec): 1-2 sentences. Make them feel understood.
      - Solution intro (8-15 sec): Introduce GlowUp naturally, like a friend recommending it.
      - Proof (15-22 sec): Specific result (14 days, visible difference).
      - CTA (22-30 sec): Soft sell. Link in bio. No pressure.
    Word count: 60-80 words maximum
    Energy level: 8/10 — enthusiastic but genuine

  [SCRIPT 2] YOUTUBE SHORTS — 30 to 60 seconds
    Format: Story-driven. More detail allowed.
    Structure:
      - Hook (0-5 sec): [Use Controversy or Curiosity hook]
      - Problem deep-dive (5-20 sec): Paint the full picture of the pain point.
      - Discovery moment (20-35 sec): How they found GlowUp. Natural, not scripted-sounding.
      - Results walkthrough (35-50 sec): Specific, believable results. Mention key ingredients simply.
      - CTA + social proof (50-60 sec): Mention other users / reviews. Link below.
    Word count: 120-150 words maximum
    Energy level: 6/10 — conversational, informative

  [SCRIPT 3] FACEBOOK FEED — 45 to 60 seconds
    Format: Testimonial style. Sitting down, natural lighting.
    Structure:
      - Hook (0-5 sec): [Use Problem hook]
      - Personal story (5-25 sec): Relatable backstory. Tried everything, nothing worked.
      - GlowUp introduction (25-40 sec): Why this was different. Key benefits in plain language.
      - Before/after moment (40-50 sec): Describe the change they noticed and when.
      - CTA (50-60 sec): Warm, friendly recommendation. Includes price mention.
    Word count: 130-160 words maximum
    Energy level: 5/10 — warm, honest, trustworthy

FORMAT FOR EACH SCRIPT:
  [PLATFORM] heading
  [HOOK] — first line clearly labelled
  [SCRIPT] — full word-for-word script with action notes in (parentheses)
  [CTA OPTION A] and [CTA OPTION B]
  [DIRECTOR NOTES] — how to film this scene
```

---

## 🔴 PROMPT 5 — Captions + Hashtags Prompt
> **Purpose:** Generates platform-optimised captions with hashtags for each ad script.

```
ROLE + CONTEXT: [System Prompt + Product Brief loaded above]

TASK — Generate captions for all 3 platform scripts above.

For EACH platform, generate:

  [CAPTION STRUCTURE]
    Line 1: Hook line that matches the video hook (creates curiosity before play)
    Line 2-3: Key benefit + proof statement (2 sentences max)
    Line 4: CTA with link placeholder
    Line 5: Hashtags

  [INSTAGRAM CAPTION]
    - Max 150 characters before "more" fold
    - First line must work as standalone scroll-stopper
    - Include 15-20 targeted hashtags
    - Hashtag mix: 5 broad + 5 niche + 5 product-specific + 3 community tags

  [YOUTUBE SHORTS CAPTION]
    - Max 100 characters (shows in feed)
    - Description with timestamps if over 45 seconds
    - 8-10 relevant hashtags only (YouTube penalises hashtag stuffing)

  [FACEBOOK CAPTION]
    - Max 3 lines before "See more"
    - Conversational tone — Facebook audience is slightly older (25-35)
    - Soft CTA — "comment GLOW and I'll send you the link"
    - 5-8 hashtags maximum

FORMAT: Label each caption clearly. Show character count for line 1.
```

---

## ✅ BONUS: UGC Ad QA Prompt
> **Purpose:** Quality check all scripts before use. Ensures authenticity and conversion potential.

```
TASK: Review all UGC ad scripts against these 8 criteria.
Score each 1-10. Revise anything below 7.

QA CHECKLIST:
  [Q1] Authenticity: Does this sound like a real person, not an ad?
  [Q2] Hook strength: Will this stop a thumb-scroll in 3 seconds?
  [Q3] Problem clarity: Does the viewer feel understood in the first 8 seconds?
  [Q4] Solution naturalness: Is the product introduction smooth, not forced?
  [Q5] Proof believability: Are results specific and credible (not vague)?
  [Q6] CTA softness: Does the CTA feel like a recommendation, not a push?
  [Q7] Platform fit: Is the length, energy, and format right for the platform?
  [Q8] Hinglish balance: Is the language natural for Indian 18-32 female audience?

OUTPUT: Score table + Grade + Specific lines to revise
```

---

*Intern: Bora Karthik | CIN: FIT/MAR26/PE2027 | Future Interns PE Track*
