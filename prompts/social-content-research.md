# Social Content Research & Strategy Prompt

## Purpose

Use this prompt after `video-analysis.md` when the goal is to publish or repurpose content on Instagram, YouTube, Facebook, LinkedIn, or another social platform.

The video itself should be analysed first in Gemini. This prompt is the research and strategy layer that follows video analysis.

## Tooling Rule

Default workflow:

1. Gemini — analyse the actual video and produce the Video Analysis output.
2. ChatGPT — use the Video Analysis output as the evidence base.
3. ChatGPT — perform current web research when current information would materially improve the strategy.
4. ChatGPT — create the platform-specific publishing package.

Do not require the user to switch to another AI by default.

Only recommend another tool (for example Google Trends, another search engine, or another AI) when a specific capability would materially improve the result and cannot reasonably be obtained through available web research. State exactly what to check and why. Prefer free/currently accessible options where practical.

## 1. Understand the Source Content

Use the supplied Video Analysis to identify:

- Core topic
- Core message
- Intended audience
- Strongest moments
- Hook opportunity
- Key questions answered
- Content gaps
- Professional/brand context
- Accuracy, privacy, or trust considerations

Do not invent information that is absent from the Video Analysis.

## 2. Current Web Research

Before recommending a current trend, audience angle, search opportunity, or recent research finding, search the web.

Check where relevant:

- Current discussions around the topic
- Recent audience questions and recurring concerns
- Search/discovery language
- Recent news or developments
- Recent credible research, studies, guidelines, or official sources
- Current social content patterns
- Relevant creator/industry conversations
- Seasonal or awareness-day relevance
- Current platform-specific discovery considerations

Prioritise authoritative and primary sources for factual claims. Use community discussions to understand questions and language, not as unquestioned evidence.

Record the research date and distinguish:

- Verified fact
- Current trend signal
- Audience question
- Interpretation/inference
- Recommendation

Do not present a trend as established merely because a few posts are popular.

## 3. What People May Be Looking For Now

Answer:

- What questions are people currently asking about this topic?
- What problem or uncertainty appears repeatedly?
- What language are people using to describe it?
- What information is missing or poorly explained in existing content?
- Does the supplied video answer one of these needs?
- What useful angle could make the content more relevant without changing the video's meaning?

Do not infer private or sensitive characteristics about the audience.

## 4. Trend Fit

For each relevant trend signal provide:

- Trend/topic
- Evidence/source
- Date or freshness
- Why it is relevant to this video
- Possible adaptation
- Whether to use, adapt, monitor, or ignore

Do not force trends, memes, audio, hashtags, or formats into professional, medical, educational, or child-related content when they weaken trust or accuracy.

## 5. Platform Strategy

Determine which platforms/formats are genuinely supported by the content.

Consider:

- Instagram Reel
- Instagram Story
- Instagram Carousel
- YouTube Short
- YouTube long-form
- Facebook Reel/Post
- LinkedIn Post
- Google Business Profile, where appropriate

For each recommended platform explain the content angle and why the source material fits it.

Do not rank platforms as winners. State the distinct use case for each recommended platform.

## 6. Content Strategy Output

Return:

### Content Opportunity
What audience need the content can address.

### Primary Angle
The clearest truthful framing.

### Supporting Angle(s)
Useful secondary perspectives supported by the source.

### Hook Direction
A hook concept, not fabricated dialogue.

### Key Message
What the audience should understand.

### Audience Need
What question/problem this answers.

### Trend/Research Context
Only current, sourced findings.

### Recommended Format(s)
Platform + format + rationale.

### Adaptation Notes
What should change for each platform.

### External Tool Requirement
One of:

- `No external tool needed`
- `Optional: [tool] — check [specific item]`
- `Required: [tool] — because [specific capability gap]`

Never recommend another tool merely for redundancy.

## 7. Handoff to Platform Prompt

After strategy is complete, pass the relevant findings to the platform-specific prompt.

For Instagram, the next step is the appropriate Instagram prompt, which should generate the final publishing package such as:

- Reel structure
- Cover text/concept
- Caption
- CTA
- Hashtags
- ALT text
- SEO/discovery terms
- Posting notes

Do not duplicate the platform prompt's job unnecessarily.

## Output Rules

1. Video analysis comes first.
2. Current claims require current web evidence.
3. Research before making trend claims.
4. Do not confuse popularity with relevance.
5. Do not fabricate search volume, trend strength, audience intent, or platform behaviour.
6. Separate evidence from inference and recommendation.
7. Preserve the original video's meaning.
8. Prefer useful audience relevance over trend-chasing.
9. Tell the user when another tool genuinely adds value; otherwise do the research yourself.
10. The final output should make the next platform-specific step obvious.
