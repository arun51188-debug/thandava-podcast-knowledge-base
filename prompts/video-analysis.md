# Video Analysis Prompt

## Purpose

Analyse the supplied video as a source-evidence, communication and production asset. Current audience research and platform strategy belong in the separate research stage.

This prompt replaces the previous `visual-analysis.md` prompt. Use it whenever a video needs to be understood before creating platform-specific publishing content.

The analysis must distinguish what is directly observable/heard in the video from interpretation or recommendation. Do not claim to have performed external research in this stage. Do not invent missing information.

## Input

Analyse the supplied video using all available evidence:

- Video frames and sequence
- Audio and spoken dialogue
- Transcription, if available
- On-screen text/subtitles
- Visual context and setting
- Speaker/interactions
- Pacing and delivery
- Existing branding or graphics
- Requested target platform(s), if specified
- Brand/client context, if supplied

If a transcription is supplied separately, cross-check it against the video where possible and flag discrepancies rather than silently correcting them.

## 1. Video Identification

Return:

- Primary subject/topic
- Type of video
- Approximate duration, if available
- Number of visible speakers/participants
- Language(s)
- Intended audience, only when reasonably inferable
- Likely purpose of the video

## 2. Timestamped Video Breakdown

Analyse the video chronologically. For each meaningful section, identify:

- Approximate timestamp/range
- What is visually happening
- What is being said
- On-screen text/subtitles
- Important actions, expressions, demonstrations, or interactions
- Why the section matters to the overall message

Do not create false timestamps when exact timing is unavailable. Use sequence-based descriptions instead.

## 3. Hook Analysis

Evaluate the opening:

- What happens in the first few seconds?
- What is the first spoken/visual message?
- Does it immediately establish the subject?
- Is there a question, problem, statement, demonstration, emotional moment, or curiosity gap?
- What could make a viewer continue watching?

Describe observable characteristics and possible viewer implications; do not score the hook.

## 4. Speech & Content Analysis

Analyse the spoken content:

- Core message
- Supporting points
- Sequence of explanation
- Examples or demonstrations
- Important terminology
- Repeated ideas
- Key statements worth preserving
- Any unclear, contradictory, unsupported, or potentially misleading statements

Separate factual statements from opinions, experiences, interpretations, and recommendations.

Do not add facts that are not present unless explicitly requested as a separate research task.

## 5. Delivery & Communication Analysis

Analyse:

- Speaking clarity
- Pace
- Tone
- Energy
- Observable confidence/presence
- Pauses
- Emphasis
- Facial expressions
- Body language
- Interaction between speakers
- Whether delivery supports the intended message

Describe observable behaviour rather than assuming internal states.

## 6. Visual & Production Analysis

### Composition
- Framing
- Camera angle
- Subject placement
- Headroom
- Background
- Visual hierarchy

### People & Interaction
- Number of people
- Positioning
- Gestures
- Facial expressions
- Demonstrations
- Interaction patterns

### Production
- Lighting
- Camera stability
- Audio environment, where observable
- Microphone visibility/use
- Set/studio environment
- Branding
- Props or relevant objects

### On-screen elements
- Text
- Subtitles
- Logos
- Graphics
- B-roll
- Transitions
- Visual overlays

Identify anything that may distract from the message or reduce readability.

## 7. Educational / Informational Value

Determine what the viewer can learn from the video.

Identify:

- Main takeaway
- Secondary takeaways
- Problem being addressed
- Explanation provided
- Practical advice or action
- Emotional or behavioural insight
- Who would find the information useful

For child-development, education, therapy, medical, or other professional content, preserve the distinction between professional information and general advice.

## 8. Trust, Accuracy & Safety Check

Flag:

- Claims that appear to require verification
- Medical/educational/technical claims that may need expert review
- Absolute statements
- Potentially misleading wording
- Privacy concerns
- Visible personal information
- Children/minors or identifiable participants where consent/privacy may matter
- Sensitive situations
- Copyright or third-party material that is visibly present

Do not declare a claim false unless sufficient evidence is available. Mark it `Needs verification` when appropriate.

## 9. Research Handoff (Not Performed in This Stage)

This prompt is the **source-video analysis stage**. Keep it grounded in the supplied video and any explicitly supplied context. Do not perform broad current trend, audience-demand, competitor or search research here.

Record only research questions that arise from the video and claims that require external verification. Do not label anything as currently trending or claim audience demand without a separately sourced research step.

After this analysis, use `prompts/social-content-research.md` when current audience questions, search language, trends, competitor patterns, awareness-calendar relevance or recent research would materially improve the strategy. That prompt owns the current web research and records the research date and sources.

The research handoff should list:
- Claims or terminology requiring authoritative verification
- Audience questions worth researching
- Search phrases or content angles to validate
- Relevant platform or policy questions requiring current official guidance

If no research is needed, say: **No additional research required for this task.**

## 10. Content Opportunities

Identify possible content uses without rewriting the content yet:

- Instagram Reel
- Instagram Story
- Instagram carousel
- YouTube Short
- YouTube long-form video
- Facebook post/reel
- LinkedIn post
- Google Business Profile post, where appropriate

For each applicable format, explain the specific content angle supported by the existing video and current audience/platform research. Do not force every platform.

## 11. Best Extractable Moments

Identify useful moments for repurposing. For each provide:

- Timestamp/sequence
- What happens
- Why it is useful
- Possible use: hook / main body / proof / emotional moment / CTA / B-roll / story

Do not rank moments with arbitrary scores. Explain their distinct use cases.

## 12. Reel / Short Structure Recommendation

If suitable for short-form content, propose a structure based only on material actually present:

1. Hook
2. Context/problem
3. Main explanation
4. Key takeaway
5. CTA or closing

Use current audience research to explain why the proposed structure fits the platform and audience. Do not fabricate dialogue.

## 13. Thumbnail / Cover Opportunities

Identify:

- Strong visual frame(s)
- Speaker/subject positioning
- Suitable crop
- Potential cover-text concept
- Whether the frame works better for Instagram Reel cover, YouTube thumbnail, or Story

Cover text should be developed later by the relevant platform/content prompt unless specifically requested here.

## 14. CTA Opportunities

Identify whether the existing video naturally supports:

- Follow CTA
- Comment/question CTA
- Save/share CTA
- Watch-full-video CTA
- Contact/enquiry CTA
- Learn-more CTA

Use current audience needs where relevant, but recommend only CTAs that logically follow from the content. Do not invent offers, services, links, or claims.

## 15. Publishing Considerations

Identify:

- Whether trimming is advisable
- Whether subtitles are needed
- Whether on-screen text is needed
- Whether B-roll would improve comprehension
- Whether the opening should be tightened
- Whether the ending needs a clearer close
- Whether the original audio should be retained
- Any platform-specific adaptation required
- Whether current trends/research suggest an adaptation

## 16. Final Analysis Summary

Return a concise summary containing:

### Core Topic
What the video is fundamentally about.

### Core Message
What the audience should understand after watching.

### Current Audience Need
What people appear to be looking for around this topic based on current research.

### Relevant Current Trends / Research
Only include trends or findings supported by current sources, with source and date.

### Strongest Content Elements
The specific elements that carry the message.

### Main Improvement Opportunities
Concrete production/content improvements.

### Recommended Platform & Content Direction
Identify the most relevant platform/format(s) based on the video's characteristics and current research. Do not use arbitrary scores or rankings.

### Recommended Next Step
Identify which existing TPS platform prompt should be used next and what information from this analysis should be passed into it.

## Output Rules

1. Analyse before creating.
2. Use evidence from the actual video wherever available.
3. When social-media analysis is requested, use current web research rather than relying only on model knowledge.
4. Clearly cite and date current external research used for trend/audience claims.
5. Do not invent dialogue, timestamps, facts, people, trends, audience behaviour, or context.
6. Clearly separate observation, transcription, external research, interpretation, and recommendation.
7. Preserve the speaker's intended meaning when summarising.
8. Do not automatically generate captions, hashtags, ALT text, titles, or descriptions unless explicitly requested.
9. Do not score, rank, or assign arbitrary quality ratings.
10. Flag uncertainty instead of guessing.
11. For professional, medical, educational, or child-related content, prioritise accuracy, privacy, and trust.
12. Do not let a trend override the video's actual value, brand fit, audience relevance, or factual accuracy.
13. This analysis is an upstream content-analysis layer; platform-specific prompts should handle final publishing copy.
