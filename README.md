# From IAM to Prompt Injection

Slides for a 90-minute technical session at **AWS Student Community Day Mysuru 2026**, Vidyavardhaka College of Engineering.

**Speakers:** Subramanya Navada KR and Pradyoth Prashanth

The session follows one fictional customer-support assistant as it grows from an API into a document assistant and then an agent with a mock refund tool. It covers the AWS controls the application needs before a model is added, how prompt injection reaches the model, what Amazon Bedrock Guardrails can and cannot check, and why document access and tool actions need their own authorization. It ends with a 20-minute participant exercise.

## Present it

Open `index.html` in a browser. It's a single self-contained page; fonts load from Google Fonts.

| Key | Action |
| --- | --- |
| → · Space · click | Next reveal or slide |
| ← · click left edge | Back |
| F | Fullscreen |
| N | Speaker notes |
| Home / End | First / last slide |

Swipe works on touch screens. Each slide has its own URL, so `index.html#12` opens slide 12.

## Run of show

| Time | Lead | Segment |
| --- | --- | --- |
| 00–05 | Subramanya | Opening and the application story |
| 05–17 | Subramanya | AWS security foundations |
| 17–25 | Subramanya | API → document assistant → agent |
| 25–35 | Pradyoth | How AI applications fail |
| 35–48 | Pradyoth | Bedrock Guardrails demonstration |
| 48–58 | Pradyoth | RAG and tool authorization |
| 58–65 | Subramanya | Detection and response |
| 65–85 | Both | Participant exercise |
| 85–90 | Both | Debrief and questions |

Slides 36–39 are reference material on running the lab on AWS (architecture, cost, Free Tier, next builds); they can be skipped in the live talk.

## Repository

- `index.html`: the presentation
- `source/`: the original slide files (`deck.json`, `deck.css`, one HTML file per slide)

## Notes

- All records, identifiers, customer details and tool actions in the slides are synthetic.
- The AWS demos are a preparation plan, not a verified deployment.
- AWS documentation and pricing were checked on 29 October 2026; re-check before relying on them.
- IAM policies and resource names on the slides are illustrative placeholders.
