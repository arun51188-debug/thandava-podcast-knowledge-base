# Thandava Podcast Studio Knowledge Base

Central knowledge and prompt system for Thandava Podcast Studio, Bangalore.

## Purpose

This repository is the working source of truth for:
- Brand identity and positioning
- Audience and buyer segments
- Content pillars and platform strategy
- Local SEO and discoverability
- Research and competitive intelligence
- Platform-specific content prompts
- Asset naming, publishing and governance workflows

## Working Principle

The knowledge base comes before the prompts. Prompts should consume verified brand, audience, positioning and platform rules rather than repeatedly inventing them.

## Repository Structure

- `knowledge-base/` — stable facts, positioning, audience, content strategy and research
- `prompts/` — reusable generation prompts by platform and asset type
- `strategy/` — channel and growth strategy
- `operations/` — production, approval, naming and publishing workflows
- `archive/` — superseded research and prompts

## Source Hierarchy

1. Verified Thandava business information
2. Approved brand decisions
3. First-party platform guidance
4. Current market and competitor research
5. Inferences clearly marked as such

Do not treat assumptions as brand facts.

## Standard Video-to-Social Workflow

When a source video is being prepared for social media, follow this order:

1. **Gemini — Video Analysis**
   - Upload the actual video to Gemini.
   - Run `prompts/video-analysis.md`.
   - Capture transcription, visual observations, timestamped sections, hook, core message, delivery, important moments, privacy/accuracy issues and repurposing opportunities.

2. **ChatGPT — Social Research & Strategy**
   - Bring the Gemini Video Analysis into ChatGPT.
   - Run `prompts/social-content-research.md`.
   - Research current audience questions, search/discovery language, current discussions, recent research, seasonal relevance and meaningful trend signals when relevant.
   - Do not switch to another AI by default. If a specialised tool would materially improve the result, ChatGPT should explicitly say which tool to use, what to check and why.

3. **Platform-specific prompt**
   - Pass the approved strategy into the relevant platform prompt, such as the Instagram Reel prompt, YouTube prompt or another channel prompt.
   - Do not regenerate the video analysis unnecessarily.

4. **Publishing package**
   - Produce the platform-specific final assets: hook/structure, cover or thumbnail direction, caption/description, CTA, hashtags/keywords, ALT text and publishing notes as applicable.

5. **Approval and publishing**
   - Check brand fit, factual accuracy, privacy/consent and platform requirements.
   - Publish or schedule only after approval.

6. **Reporting / learning**
   - Record the published asset and relevant performance observations in the appropriate operational/reporting workflow.

### Tool Routing Rule

Default tool chain:

**Gemini → ChatGPT + Web research → Platform prompt → Publishing**

Use another AI or specialist tool only when it provides a specific capability that materially improves the task and is not reasonably available through the current workflow. Prefer free/currently accessible options where practical.

## Prompt Routing

- `prompts/video-analysis.md` — analyse the actual source video before strategy or publishing.
- `prompts/social-content-research.md` — research current audience needs, trends and evidence and convert Video Analysis into a content strategy.
- Platform prompts — convert the approved strategy into platform-specific publishing content.

The analysis layer should not be used as a substitute for current research, and the research/strategy layer should not unnecessarily duplicate platform-specific generation prompts.

## Status

Initial foundation created August 2026. Research and prompt system are being built incrementally.
