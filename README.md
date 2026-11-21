# From IAM to Prompt Injection

An interactive lecture for second- and third-year students at AWS Student Community Day Mysuru 2026.

Subramanya Navada KR opens with application and cloud security foundations. Pradyoth Prashanth leads AI foundations, prompt injection, the Jack & Jill research case, Bedrock Guardrails, retrieval authorization and agent tool security. Subramanya closes with detection and incident response.

## Open the presentation

Open `index.html` in a browser. No server, AWS account or API key is required. Fonts load from Google Fonts when available, with local fallbacks.

| Key | Action |
| --- | --- |
| Right / Space / click background | Next reveal or slide |
| Left / click left background | Previous reveal or slide |
| F | Fullscreen |
| Home / End | First / last slide |

Buttons and selectors run the on-screen examples. Click the background after using a form control to resume keyboard navigation. URL fragments such as `index.html#17` select a slide.

## Lecture flow

| Slides | Content |
| --- | --- |
| 1–4 | Opening challenge, five questions and the two sides of AI security |
| 5–19 | Application and cloud foundations, recent attack cases, identities, IAM, encryption, secrets and cost |
| 20–23 | LLM context, trust boundaries and direct / indirect prompt injection |
| 24–27 | Pradyoth’s Jack & Jill resume case, AWS design and execution evidence |
| 28–33 | Guardrails, false positives, hallucinations, grounding and persistent memory poisoning |
| 34–45 | Guardrail integration, document / tool permissions, Cline incident and AWS pipeline controls |
| 46–50 | GuardDuty AI Protection, logs, alert routing and incident response |

A 45-minute interactive lecture for second- and third-year students. Subramanya opens with cloud foundations and AI-assisted attack cases. Pradyoth leads AI application security and the research cases. Subramanya closes with detection and response. The slides contain worked examples and audience questions, with no participant exercises, speaker notes, setup runbooks or reference appendices.

## Motion and diagrams

Every slide carries an animated diagram of its idea: request flows, attack chains, timelines, meters and gauges. The flows on the example slides react to the on-screen controls. A drifting network background, staggered entrances and slide transitions run throughout, and the closing slide fires confetti.

Slide 21 is an AWS trace lab that follows the poisoned-file lab: drag the same resume through S3, a Lambda extractor, `ApplyGuardrail`, a Bedrock model, an AgentCore Gateway policy and the offer-email tool. Two switches turn the Guardrail check and the tool-gate approval on or off, and a side panel lists what CloudTrail, CloudWatch and the Guardrail trace would hold at each stage. Its values are illustrative, like the other examples.

All of it is inline SVG, CSS and a small script at the end of `index.html` (the `FX layer` block in the styles, and the last `<script>`). Nothing new is loaded from the network. With the operating system's reduce-motion setting on, every animation is switched off and each diagram shows its finished state.

## Example boundaries

Interactive examples run deterministic JavaScript locally. They do not invoke a model, call AWS, reproduce the Bedrock classifiers or implement the complete IAM policy engine. All support records, refunds and finding fixtures are synthetic. Labels distinguish illustrative results from real evidence.

The Jack & Jill material comes from Pradyoth’s published research at https://ppradyoth.com/research/. The resume result and the separate chat-and-email test are identified separately. Delivered email does not establish a valid job offer. The AWS architecture is a proposed defense for the failure pattern, not a claim about the researched service’s hosting stack.

## Recent cases

The lecture uses four primary-source 2026 reports. Case slides link to the original report and distinguish the incident date from the publication date. AWS defense mappings are proposed designs, not claims about the affected service’s hosting stack.

| Case | Primary source |
| --- | --- |
| FortiGate campaign | [Amazon Threat Intelligence, 20 Feb 2026](https://aws.amazon.com/blogs/security/ai-augmented-threat-actor-accesses-fortigate-devices-at-scale/) |
| AI-assisted exposed-secret abuse | [Microsoft Threat Intelligence, 5 Nov 2026](https://www.microsoft.com/en-us/security/blog/2026/11/05/threat-actors-use-agentic-ai-tooling-to-find-and-abuse-exposed-secrets/) |
| AI recommendation poisoning attempts | [Microsoft Defender Security Research, 10 Feb 2026](https://www.microsoft.com/en-us/security/blog/2026/02/10/ai-recommendation-poisoning/) |
| Unauthorized Cline CLI release | [Cline maintainer post-mortem, 24 Feb 2026](https://cline.bot/blog/post-mortem-unauthorized-cline-cli-npm) |

## Editing

`index.html` is the complete runnable presentation, including the additional concept and research slides. Existing root HTML fragments mirror their corresponding slides. `deck.css` holds the shared slide styling, also embedded in `index.html`. Keep corresponding content and styles synchronized when editing.
