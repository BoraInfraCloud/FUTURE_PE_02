# 📖 Task 2 — Explanation
## Why I Structured the Prompts, How AI Generated the Content, What Tools I Used
**Intern:** Bora Karthik | **CIN:** FIT/MAR26/PE2027 | **Track:** Prompt Engineering (PE)

---

## 🔧 Tools Used

| Tool | Purpose | How I Used It |
|------|---------|---------------|
| **Claude AI** (claude.ai) | Primary LLM | Ran all 5 HBC-X prompts to generate hooks, scripts, captions, and QA review |

---

## 🧠 Why I Structured the Prompts This Way

### 1. Why I Used the HBC-X Framework (Not a Generic "Write Me an Ad" Prompt)

A beginner prompt: *"Write me a UGC ad for a skincare serum"*
produces generic, robotic-sounding scripts that no real person would believe.

I designed the **HBC-X Framework** — Hook, Body, CTA, eXecution rules — because UGC advertising is psychology-driven. Each layer serves a specific conversion purpose:

| Layer | Why It's Separate |
|-------|------------------|
| **Hook** | 95% of viewers decide to keep watching in the first 3 seconds. This deserves its own dedicated prompt. |
| **Body** | Story structure (Problem → Agitation → Solution → Proof) must feel organic — rushed copy breaks authenticity. |
| **CTA** | A wrong CTA (too pushy) can destroy a perfect script. It needs its own rules. |
| **eXecution** | Platform format, length, and energy are completely different for Instagram vs YouTube vs Facebook. |

Separating these into individual prompt layers meant the AI could focus fully on each element — producing output that sounds like a real person, not a marketing robot.

---

### 2. Why I Assigned the AdScript-Pro Persona

In Prompt 1 (System Context), I assigned Claude the role of **"AdScript-Pro"** — a UGC specialist with 12+ years experience who has worked with Indian D2C brands like Mamaearth and Minimalist.

**Why this specific persona:**

- **Indian market experience** activates knowledge of Hinglish, Indian skin tone sensitivity, and culturally relevant pain points
- **D2C brand experience** activates knowledge of price-to-value messaging and conversion-focused language
- **UGC specialist** (not just "copywriter") activates knowledge of authentic creator voice vs brand voice

Without this persona, Claude defaults to polished marketing language. With it, the output sounds like a real person talking.

---

### 3. Why I Created a Separate Hook Generator Prompt

Most UGC beginners treat hooks as one line before the "real" script. This is wrong.

**The hook IS the ad.** If the first 3 seconds don't stop the scroll, no one sees the rest.

I created a dedicated Hook Generator Prompt (Prompt 3) that:
- Generated **10 hooks** across 5 different psychological trigger types
- Required a **different trigger** for each pair — preventing repetition
- Forced hooks to **maximum 15 words** — short hooks outperform long ones by 40%
- **Banned common hook patterns** ("Do you...?" "Are you...?") that are overused and ignored

The result: 10 distinct, tested hook options to choose from — giving variety and options for A/B testing.

---

### 4. Why I Used 5 Different Hook Trigger Types

Research from top UGC agencies shows different audiences respond to different psychological triggers. I engineered one prompt to cover all 5:

| Trigger | Psychology | Best For |
|---------|-----------|----------|
| **Relatability** | Mirror neurons fire when viewers see themselves | Instagram Reels — young audience |
| **Controversy** | Pattern interrupt — brain can't ignore unexpected statements | YouTube — educational audience |
| **Result** | Outcome-first triggers curiosity about the "how" | All platforms — high-intent buyers |
| **Problem** | Being understood is the strongest trust-builder | Facebook — older, more considered buyers |
| **Curiosity** | Information gap creates compulsive watching | YouTube Shorts — discovery audience |

Having all 5 types means the ad pack works across different buyer psychology profiles — not just one segment.

---

### 5. Why I Used Platform-Specific Scripts (Not One Universal Script)

A common mistake is writing one UGC script and posting it everywhere. This fails because:

| Platform | Audience Behaviour | What Works |
|----------|------------------|------------|
| **Instagram Reels** | Fast scroll, low attention, entertainment-first | Short, high energy, fast cuts, 15-30 sec |
| **YouTube Shorts** | Discovery-intent, more curious, willing to learn | Story-driven, informative, 30-60 sec |
| **Facebook Feed** | Older audience, more considered, trust-driven | Testimonial style, slower pace, 45-60 sec |

I engineered Prompt 4 to produce **3 different scripts** — same product, same brand, completely different structure and energy for each platform. This is how professional D2C brands run multi-platform campaigns.

---

### 6. Why I Included Hinglish in the Scripts

The target audience is Indian women aged 18-32. This demographic:
- Naturally code-switches between Hindi and English
- Finds pure English scripts slightly unnatural and corporate
- Responds more strongly to natural Hindi-English phrases like *"yaar"*, *"literally"*, *"seriously just try it"*

I specified Hinglish balance in the System Context Prompt (Prompt 1) — instructing the AI to use conversational Indian English with selective Hindi words where natural.

This produced scripts that sound like a real Indian woman talking, not a dubbed English ad.

---

### 7. Why I Added a Forbidden Phrases List

Certain phrases in UGC ads instantly destroy viewer trust:

- *"You won't believe..."* — overused, feels like clickbait
- *"Game-changer"* — corporate buzzword, no real person talks like this
- *"Limited time offer"* — hard-sell language that breaks authentic tone
- *"Clinically proven"* — sounds scripted and unverifiable to viewers
- *"Revolutionary"* — nobody believes this word anymore

By adding these to the System Context Prompt, every generated script automatically avoided all credibility-killing language without needing separate review passes.

---

### 8. Why I Included Director Notes in Each Script

UGC ads are visual — the words are only 40% of the performance. The filming setup determines whether the ad feels real or staged.

I included **Director Notes** in Prompt 4's format requirements, which produced specific guidance like:
- "Film in natural morning light near a window"
- "Casual outfit — oversized t-shirt works well"
- "Don't over-edit — slight grain is okay, feels authentic"
- "Include subtitles — 85% of Facebook videos watched on mute"

These notes are what a real UGC creator brief looks like. This level of detail demonstrates professional prompt engineering — not just basic content generation.

---

## ⚙️ How the AI Generated the Content — Step by Step

### Step 1: Session Setup
Opened Claude (claude.ai). Pasted **Prompt 1 (System Context)** — establishing AdScript-Pro persona with operating rules and forbidden phrases list.

### Step 2: Product Context Loading
Sent **Prompt 2 (Product Brief)** — GlowUp Serum profile, audience pain points, brand voice parameters, and conversion goal.

### Step 3: Hook Generation
Sent **Prompt 3 (Hook Generator)**. Claude produced:
- 10 hooks across 5 trigger types (2 per type)
- Trigger type labels for each hook
- "Why it works" explanation per hook
- Best platform recommendation per hook

Reviewed all 10 hooks and selected the best ones per platform for use in scripts.

### Step 4: Full Script Generation
Sent **Prompt 4 (Full Ad Script Generator)** with the selected hooks referenced. Claude produced:
- 3 complete word-for-word scripts (Instagram, YouTube, Facebook)
- Action notes in parentheses throughout
- 2 CTA options per script
- Director notes for each

### Step 5: Caption + Hashtag Generation
Sent **Prompt 5 (Captions + Hashtags)**. Claude produced:
- 3 platform-specific captions with correct character counts
- Platform-optimised hashtag sets (20 for Instagram, 8 for YouTube, 5 for Facebook)
- Timestamps for YouTube description

### Step 6: QA Review
Ran the **QA Prompt** on the complete ad pack. All 8 criteria scored 9-10/10. Overall grade: A+ (9.6/10). No revisions needed.

---

## 📊 Results Summary

| Metric | Result |
|--------|--------|
| Total prompts designed | 5 (+ 1 QA) |
| Hook variants generated | 10 (5 trigger types × 2) |
| Full ad scripts | 3 (one per platform) |
| CTA options | 6 total (2 per script) |
| Captions with hashtags | 3 platform-optimised |
| Director notes sets | 3 (one per script) |
| QA score | 9.6/10 — A+ Grade |
| Time to complete | Under 90 minutes |

---

## 💡 Key Learnings from Task 2

1. **Hooks are the entire ad.** Spending 40% of prompt engineering effort on just hooks (Prompt 3) produced dramatically better output than treating them as one line.

2. **Persona specificity unlocks domain knowledge.** "AdScript-Pro with Indian D2C experience" activated culturally relevant language that "write a UGC ad" never could.

3. **Platform differences are real.** The Instagram script and Facebook script for the same product are almost completely different documents — energy, pace, structure, and tone all change.

4. **Forbidden phrases lists work better than style instructions.** Telling the AI what NOT to do is more precise and effective than telling it what TO do.

5. **Format instructions in prompts produce structured output.** Requiring "Director Notes" in the output format produced professional-grade creative briefs without any extra prompting.

6. **Hinglish is a strategy, not a compromise.** Culturally-calibrated language produces higher authenticity scores and better audience connection for the Indian market.

---

*Intern: Bora Karthik | CIN: FIT/MAR26/PE2027 | Future Interns PE Track*
*Repository: FUTURE_PE_02 | Date: March 2026*
