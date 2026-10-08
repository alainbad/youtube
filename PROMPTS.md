# YouTube Prompt Library

Seven prompts, ordered as a workflow (pick niche → identity → plan → script → package → repurpose → monetize).
Each has the **original** and a **sharpened** version. The sharpened versions fix the main failure mode of the
original: the model fills gaps with generic, confident-sounding guesses.

Fill these variables once and reuse them everywhere:

| Variable | Example |
|---|---|
| `[niche]` | Personal finance for nurses |
| `[audience]` | US nurses, 25–40, paying off student loans |
| `[subs]` | 1,200 |
| `[avg_views]` | 800 views/video |
| `[my_edge]` | I'm an RN who paid off $90k in 3 years |
| `[hours_per_week]` | 8 |

---

## 1. Niche research

**Original**
> Analyze the top 10 YouTube niches with high CPM, low competition, and strong evergreen demand. For each one give me: average CPM, content difficulty, monetization avenues beyond AdSense, and a 3-word channel concept.

**Problem:** The model has no live CPM data, so the numbers are invented. And a "low competition" list that
everyone running this prompt receives is, by definition, not low competition.

**Sharpened**
> My background: [my_edge]. I can produce [hours_per_week] hours/week. Suggest 10 YouTube niches where *my
> background* is an unfair advantage. For each: why advertisers pay well in that niche (reasoning, not a CPM
> number), what competing channels look like, the hardest part of making the content, 2 non-AdSense revenue
> streams, and a 3-word channel concept. Label every factual claim as verified or estimated. Then tell me
> which 2 to test and how to tell within 10 videos which one to keep.

---

## 2. Channel identity

**Original**
> I'm starting a YouTube channel about [niche]. Create a complete identity: channel name (5 options), slogan, target audience profile, 4 content pillars, and a 'unique mechanism' that sets me apart from existing creators.

**Sharpened**
> I'm starting a YouTube channel about [niche] for [audience]. My edge: [my_edge]. Create: 5 channel names
> (under 15 characters, no hyphens, say which are likely taken), a slogan, an audience profile (their problem,
> what they've already tried, what they search at 11pm), 4 content pillars (one search-driven, one
> story-driven, one opinion/contrarian, one that leads to a product), and a "unique mechanism" built from my
> real edge, not something invented. Name 3 existing channels I'd compete with and how I differ.

---

## 3. 90-day content calendar

**Original**
> Build a 90-day YouTube content calendar for a new channel in [niche]. Include: 12 search-optimized titles, publishing schedule, which videos to prioritize for SEO vs. virality, and a progression that builds authority over time.

**Sharpened**
> Build a 90-day calendar for a new [niche] channel; I can publish 1 video/week at [hours_per_week] hrs/week.
> Give 12 titles: 8 search-first (questions people actually type, low-view-count competitors) and 4
> browse-first (curiosity/emotion). For each: target search phrase, SEO or virality, and which earlier video
> it links to. Order them so weeks 1–4 build search traffic, 5–8 test formats, 9–12 double down. Add a
> checkpoint at day 30 and day 60: which metrics (CTR, avg view duration, subs/video) mean "keep going" vs
> "change format".

---

## 4. Script

**Original**
> Write a full YouTube script for '[video title]'. Use this structure: hook (first 30 seconds to stop the scroll), problem agitation, walkthrough of the solution, 3 key takeaways, call to action, and a teaser for the next video in the end screen.

**Problem:** 30 seconds is too long for a hook. Viewers decide in the first 5–10.

**Sharpened**
> Write a YouTube script for '[video title]' aimed at [audience], target length [X] minutes (~150 words/min).
> Structure: hook in the first 2 sentences that confirms the title's promise, then a reason to stay; problem
> agitation (specific, not dramatic); solution walkthrough with one concrete example from [my_edge]; 3
> takeaways; one CTA only (not like+subscribe+comment+bell); end-screen teaser for '[next video]'. Mark
> B-roll/visual cues in [brackets]. Write it to be spoken: short sentences, no "in this video I will".

---

## 5. Packaging (thumbnail, title, description, tags)

**Original**
> For the video '[title]' give me: 3 thumbnail concepts with overlay text, an SEO-optimized title (under 60 characters), a description with timestamps, keywords, and links, and 10 tags. Also suggest A/B test variations for the thumbnail.

**Problem:** Tags have almost no ranking weight on YouTube today; don't spend effort there. Timestamps can't be
written without the script.

**Sharpened**
> For the video '[title]' (script below): give 3 thumbnail concepts that each show a *different* idea (not
> color swaps), overlay text max 4 words that adds to the title rather than repeating it; 3 title options under
> 60 characters (one search-phrased, one curiosity, one result-focused); a description whose first 2 lines
> work as a search snippet, then timestamps from the script, then links [links]; 5 tags. Pair title+thumbnail
> into 3 combos for YouTube's built-in Test & Compare and say what each tests.
>
> [paste script]

---

## 6. Repurposing

**Original**
> Take this YouTube script or transcript and repurpose it into: an X thread, a LinkedIn post, 3 Shorts hooks, an email newsletter, and a Pinterest description. Also suggest which platforms to prioritize based on my niche: [niche]

**Sharpened**
> My niche: [niche], audience: [audience]. First, rank these platforms for *this* audience: X, LinkedIn,
> Shorts/TikTok, email, Pinterest. Drop any that don't fit and say why. Then produce content only for the top
> 3. Each piece must stand alone (no "watch my video to find out") and link back once. Shorts: 3 hooks + a
> 45-second script for the strongest one, pulled from an actual moment in the transcript.
>
> [paste transcript]

---

## 7. Monetization roadmap

**Original**
> I have a YouTube channel in [niche] with [X] subscribers. Build me a monetization roadmap beyond AdSense: affiliate opportunities, digital product ideas, sponsorship pitch template, and a lead magnet to build an email list.

**Sharpened**
> Channel: [niche], [subs] subscribers, [avg_views] avg views, audience [audience]. Build a roadmap staged by
> what's realistic at my size, not in general: (1) now — a lead magnet and email list setup; (2) next —
> 5 affiliate programs I could actually be approved for, with typical commission structure (mark as
> estimated); (3) at ~5k email subs — 2 digital product ideas validated by my audience's problems, with a
> way to pre-sell before building; (4) sponsorship pitch template using views-per-video, not sub count, plus
> how to price it. Tell me which step to skip if I have only [hours_per_week] hrs/week.
