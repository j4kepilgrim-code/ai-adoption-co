# AI Adoption Co. — Training Programme

**Level 0 to Level 5 — Model Agnostic**

Works with Claude · ChatGPT · or any AI tool your team uses.

> You bought the licences. Here is what happens next.

---

## Overview

Most companies buy AI licences and then stall. The tool exists, the logins are issued, and almost nothing changes. This programme fixes that.

It is not tied to any single AI product. Whether your team uses Claude, ChatGPT, or a mix of both — the method is the same. The chain is the same. The only difference is which buttons you click.

**The promise:** By the end of this programme your team will have a shared mental model, a set of repeatable labs they can run on any task, and at least one working workflow they built themselves.

---

## The Levels

| Level | Name | What it looks like |
|-------|------|--------------------|
| **0** | Passenger | Has the licence. Has the login. Not sure what to do with it. |
| **1** | Driver | Gets useful outputs regularly. Understands why quality varies. Iterates rather than gives up. |
| **2** | Builder | Sets up persistent workspaces. Brings documents and examples in. Builds repeatable things. |
| **3** | Connector | Connects the model to tools and data sources. Thinks of it as a layer, not a chat window. |
| **4** | Architect | Designs workflows others use. Thinks about inputs, outputs, owners, hand-offs, quality. |
| **5** | Champion | Coaches peers. Spots opportunities. Maintains quality over time. The internal AI lead. |

---

## The Chain

The framework behind every lab. The fish you take home.

> **Goal → Model → Context → Reasoning → Tool → Hand-off**

Works across Claude, ChatGPT, or any AI tool your team uses.

---

## Data Safety and Privacy

Before your team uses any AI tool for work, there are things every person in the organisation needs to understand. This is not optional reading. Getting this wrong can expose confidential information, client data, or trade secrets.

The good news: with the right plan type and the right habits, both Claude and ChatGPT can be used safely for business. The bad news: the default settings on consumer plans are not safe for business use.

### The single most important rule

**Never put sensitive data into a consumer or free plan.** Free, Plus, and Pro tiers (for both Claude and ChatGPT) may use your conversations to train their models by default. This means confidential client information, financial data, internal strategy, or personal details could be retained and potentially influence future model responses. Business, Team, and Enterprise plans are different — your data is excluded from training by default. If your organisation is using personal or free accounts for work, stop. Get the right plan first.

### How Claude handles your data

| Claude plan | Trains on your data? | Data retention | Safe for business use? |
|-------------|---------------------|----------------|------------------------|
| Free / consumer plan | Yes — by default unless opted out | 30 days (no training) or 5 years (if training on) | No |
| Claude Pro (individual) | Yes — by default unless opted out | 30 days or 5 years if training enabled | No |
| Claude for Work / Team / Enterprise | No — excluded by default | 30 days, deletable | Yes |
| Claude API | No — never used for training | 7 days, then deleted | Yes |

### How ChatGPT handles your data

| ChatGPT plan | Trains on your data? | Data retention | Safe for business use? |
|--------------|---------------------|----------------|------------------------|
| Free / Plus / Pro (individual) | Yes — by default unless opted out | Retained until deleted or 30 days after | No |
| ChatGPT Team | No — excluded by default | Until manually deleted | Yes |
| ChatGPT Enterprise | No — excluded by default | Admin controlled | Yes |
| OpenAI API | No — not used for training | 30 days for safety, then deleted | Yes |

### What your organisation should do right now

**Step 1 — Check which plan everyone is on.** The biggest risk is shadow AI — employees using personal free or Pro accounts for work without realising what happens to that data. Before Training Day, the organisation should know which plan every employee is using. If anyone is on a free or individual paid plan for work, that needs to change before they put anything confidential into it.

**Step 2 — Get the right plan.**
- For Claude: Claude for Work (Team or Enterprise) ensures your data is excluded from training. Contact Anthropic at anthropic.com/team.
- For ChatGPT: ChatGPT Team or Enterprise ensures your data is excluded from training. Contact OpenAI at openai.com/chatgpt/team.
- If you are using both: ensure the business plan covers all employees on both tools.

**Step 3 — Set a company AI use policy.** Even on a business plan, your team needs to understand what is and is not appropriate to put into an AI tool. A simple one-page policy is enough at this stage. It should cover:
- What categories of data must never go into an AI tool — client personal data, financial records, passwords, unreleased product information, legally privileged communications.
- What is acceptable — internal drafting, summarising non-sensitive documents, brainstorming, formatting, research on public information.
- Which plan the company uses and why personal accounts must not be used for work.
- Who to ask if unsure.

**Step 4 — Check your data is encrypted in transit.** Both Claude for Work and ChatGPT Team and Enterprise encrypt data in transit (TLS) and at rest (AES-256). This is standard and you do not need to do anything special — but it is worth knowing so you can communicate it to your team.

### What the model does and does not do with your data

**The model does not remember between sessions.** This is one of the most important things to understand. Both Claude and ChatGPT on business plans do not retain memory of your conversations between sessions. Each new conversation starts fresh. The model does not know what you said yesterday. This is why context — uploading documents, setting up workspaces — is the skill at the heart of this programme. The model has no persistent memory of your organisation. You have to bring it each time.

**Watch for jurisdictional considerations.** Both Anthropic and OpenAI are US companies. This means data is subject to US law including the CLOUD Act, which allows US authorities to request data from US companies even if that data is stored outside the US. For most SMBs this is not a practical concern, but organisations handling highly sensitive data should be aware of it and seek legal advice if required. Australia's Privacy Act 1988 and the Australian Privacy Principles (APPs) also apply to how your organisation handles personal data — including data you process using third-party AI tools.

### The three things to tell your team on Training Day

| | |
|--|--|
| **1** | Check your plan. Free plans are not for work. Business plans are. |
| **2** | Never paste sensitive client data, passwords, or confidential financials into any AI tool. |
| **3** | The model does not remember you. Each session is fresh. That is why context skills matter. |

---

## The One Idea That Changes Everything

**The model is stateless.**

Every time you open it — Claude, ChatGPT, or any other tool — it is day one. It has no memory of you, your company, your clients, or your last conversation. A brilliant, well-read colleague who walks into the room with zero context every single time. What you bring to it determines everything about what comes out.

### What you can bring to a stateless model

| 1. Yourself | 2. Your documents | 3. Tools and skills |
|-------------|-------------------|---------------------|
| Your words, instructions, prompts, roles. Level 0 to 1. | Files, examples, reference material. The bridge to Level 2. | Connections to other systems. Level 3 and beyond. |

---

## L0 → L1 — Passenger to Driver

**Format:** Training Day · Half day · Whole team

### Free pre-reading

Before Training Day, point participants at their AI provider's free foundational course.

- **Claude users:** AI Fluency for Small Businesses — [anthropic.skilljar.com](https://anthropic.skilljar.com)
- **ChatGPT users:** AI Foundations — [academy.openai.com](https://academy.openai.com)
- **Both:** AI Capabilities and Limitations (Anthropic) covers fundamentals applicable to any model.

### Lab 1 — The Context Lab

- **Mode:** Conversation
- **Time:** 25 min
- **Works with:** Claude · ChatGPT

Same task, three levels of context. Compare outputs. The gap between Run 1 and Run 3 is the lesson.

- Run 1: write a follow-up email after a meeting. No context.
- Run 2: add who you are, who it goes to, what the meeting covered.
- Run 3: add what was decided, next steps, tone, and paste in one example of a good email you have actually sent.

What did you have to give it to get something genuinely useful? That list is your context checklist for this task, forever.

### Lab 2 — The Role Lab

- **Mode:** Conversation
- **Time:** 25 min
- **Works with:** Claude · ChatGPT

Task: we are thinking about hiring a part-time social media manager. What should we consider?

- Run 1: no role, no instruction on how to think.
- Run 2: you are an experienced operations manager. Think through this carefully before answering.
- Run 3: you are a cautious CFO. List the risks before the benefits.

Same question, three lenses. The model mirrors whatever role you give it. What lens would be most useful for the decisions you make regularly?

### Lab 3 — The Iteration Lab

- **Mode:** Conversation
- **Time:** 25 min
- **Works with:** Claude · ChatGPT

Pick something you actually need to write this week.

- Step 1: deliberately vague prompt. See what comes back.
- Step 2: diagnose what is wrong. Be specific.
- Step 3: fix in three moves — tell it what is wrong, add a constraint, ask it to critique itself and fix it.

A bad output is almost always a bad prompt. The skill is knowing how to close the gap.

---

## L1 → L2 — Driver to Builder

**Format:** Training Day · Half day · Small groups of 2–3

**The core shift:** A one-off conversation is a task. A persistent workspace is a system. The difference is whether you did the setup work once and stored it, or whether you are re-explaining everything every single time.

### Lab 4 — The Documentation Lab

- **Mode:** Conversation
- **Time:** 25 min
- **Works with:** Claude · ChatGPT

Part A: upload a real document you use. Ask questions, summarise, reformat, find problems.

Part B: upload an example of your best work and say — use this as a reference for quality and style. Watch the output jump.

### Lab 5 — The Persistent Workspace Lab

- **Mode:** Workspace
- **Time:** 30 min
- **Works with:** Claude Projects · ChatGPT Custom GPTs

Pick a recurring task. Set up a workspace with three things:

1. A system instruction: who you are, what the workspace is for, what good output looks like.
2. A reference document: one example of a good output you have produced before.
3. A trigger: the shortest prompt that kicks it into action.

Run it on real data. Compare to a blank conversation. How long did setup take? How much time does it save per use?

### Lab 6 — The Output Lab

- **Mode:** Artifact
- **Time:** 25 min
- **Works with:** Claude · ChatGPT

Pick a structured output your team produces regularly. Give the model the raw ingredients and ask it to produce the formatted document. Then ask: who receives this? What review step sits between the model and the recipient? The output is 60% of the job. The hand-off is the other 40%.

---

## L2 → L3 — Builder to Connector

**Format:** Full day · 4–6 people · Include whoever manages your tech stack

**The core shift:** The model alone is limited by what you manually bring to it. Tools and skills extend it — connecting it to your data sources, documents, and other systems. It stops being a chat window and starts being part of how the business runs.

### Pre-reading

- **Claude users:** Introduction to Model Context Protocol — [anthropic.skilljar.com](https://anthropic.skilljar.com)
- **ChatGPT users:** OpenAI Actions and GPT connectors — [platform.openai.com/docs](https://platform.openai.com/docs)

### Lab 7 — The Connector Lab

- **Mode:** Connected tool
- **Time:** 45 min
- **Works with:** Claude MCP · ChatGPT Connectors

Pick one integration relevant to the business — search, a document library, a CRM. Set up the connection. Run a task that would have been impossible without it. Compare before and after.

### Lab 8 — The Skills Lab

- **Mode:** Custom skill
- **Time:** 45 min
- **Works with:** Claude Skills · ChatGPT Custom GPTs

Show one working skill. Break down what is inside it — the instructions, the examples, the rules. Scope out one skill the team would benefit from. Write the brief together. If time allows, start building it.

---

## L3 → L4 — Connector to Architect

**Format:** Full day · Core operations team

**The core shift:** At Level 3 you are connecting things. At Level 4 you are designing the whole system. Not a single connection point — the entire flow. What triggers it, what goes in, what comes out, who checks it, where it goes, what happens when it breaks.

### Workflow design workshop

Pick two or three candidate workflows. Map each one using the chain. For each workflow answer six questions:

1. What triggers it?
2. What data and context does it need, and where does that come from?
3. What does the model do?
4. What does a human check before the output goes anywhere?
5. Where does the output go, and who receives it?
6. Who owns it, and what does failure look like?

**The Chain:** Goal → Model → Context → Reasoning → Tool → Hand-off

Then build one end-to-end in the room. Not a prototype — a working thing with an owner, a trigger, a review step, and a home.

### Quality and evaluation

How do you know a workflow is still working in 30 days? Build a review mechanism in from the start. What does a good output look like? What does a drifted output look like? Who checks, and when? A monthly 10-minute review of active workflows is enough to catch drift before it causes problems.

---

## L4 → L5 — Architect to Champion

**Format:** Ongoing role · Named individuals · Champions session + monthly calls

**The champion's job:** Not to be the most advanced user. To raise the floor for everyone else. Teacher, troubleshooter, and early warning system — spotting where things are drifting, where new capabilities could help, and where the team needs support.

### How to identify them

They self-select during Training Day. The Level 4 and 5 people are obvious — they have already tried more, ask better questions, and help their neighbours without being asked. Name them publicly. Give them a role.

### Champions session

**How to coach without taking over** — The difference between doing it for someone and teaching them to do it. How to run a context lab informally with a colleague. How to diagnose a bad output and explain what went wrong without making the person feel stupid.

**How to maintain quality over time** — A monthly review rhythm — which workspaces are running, which have drifted, which should be retired, which new ones to build. How to keep a shared library of what works.

**How to stay current** — Both Anthropic Academy and OpenAI Academy keep adding courses. Models keep improving. New tools keep shipping. The champion's job is to know what is new and translate it into whether it matters for this business.

### Champion engagement model

| Champions session | Monthly call | After 3 months |
|-------------------|--------------|----------------|
| 2–3 hours, once | 60 min, 3 months | Self-sufficient or re-engage |

---

## Closing principle

> The model is stateless.
>
> *It will always be stateless.*
>
> **But now you know what to bring.**

---

## Appendix — Course Map and Links

Both Anthropic and OpenAI offer free foundational training that maps directly to the levels in this programme. These courses are the homework layer — self-paced, free, and certified. The programme above is the implementation layer: the diagnostic, the labs, the workshop, and the hands-on build sessions that turn course knowledge into working practice.

Courses are listed in order of relevance to each level transition. All links were verified May 2026.

| Course | Provider | Level | Link |
|--------|----------|-------|------|
| AI Fluency for Small Businesses | Anthropic Academy | 0 → 1 | [anthropic.skilljar.com](https://anthropic.skilljar.com) |
| AI Capabilities and Limitations | Anthropic Academy | 0 → 1 | [anthropic.skilljar.com](https://anthropic.skilljar.com) |
| Claude 101 | Anthropic Academy | 0 → 1 | [anthropic.skilljar.com](https://anthropic.skilljar.com) |
| AI Foundations | OpenAI Academy | 0 → 1 | [academy.openai.com](https://academy.openai.com) |
| AI Fluency: Framework & Foundations | Anthropic Academy | 1 → 2 | [anthropic.skilljar.com](https://anthropic.skilljar.com) |
| ChatGPT for Excel / Skill Labs | OpenAI Academy | 1 → 2 | [academy.openai.com](https://academy.openai.com) |
| Intro to Claude Cowork | Anthropic Academy | 1 → 2 | [anthropic.skilljar.com](https://anthropic.skilljar.com) |
| Introduction to Model Context Protocol | Anthropic Academy | 2 → 3 | [anthropic.skilljar.com](https://anthropic.skilljar.com) |
| Introduction to Agent Skills | Anthropic Academy | 3 → 4 | [anthropic.skilljar.com](https://anthropic.skilljar.com) |
| Introduction to Subagents | Anthropic Academy | 3 → 4 | [anthropic.skilljar.com](https://anthropic.skilljar.com) |
| Building with the Claude API | Anthropic Academy | 4 → 5 | [anthropic.skilljar.com](https://anthropic.skilljar.com) |
| OpenAI Certifications (in pilot) | OpenAI / Coursera | 4 → 5 | [openai.com/index/openai-certificate-courses](https://openai.com/index/openai-certificate-courses) |

### Provider notes

**Anthropic Academy** — [anthropic.skilljar.com](https://anthropic.skilljar.com)
Launched March 2026. 13+ self-paced courses, all free, all with completion certificates. Three tracks: AI Fluency (for everyone), Product Training (for workflow professionals), and Developer Deep-Dives (for technical users). Directly relevant to Levels 0 through 4.

**OpenAI Academy** — [academy.openai.com](https://academy.openai.com)
Launched 2026. Mix of live workshops, virtual events, and digital content. AI Foundations course is currently in pilot with large employers and rolling out more broadly. Certification programme launching through 2026. Directly relevant to Levels 0 and 1. Technical courses on [platform.openai.com](https://platform.openai.com) for Level 3 and above.

### Data privacy quick reference links

- Anthropic privacy centre: [privacy.claude.com](https://privacy.claude.com)
- Anthropic Claude for Work / Team: [anthropic.com/team](https://anthropic.com/team)
- OpenAI enterprise privacy: [openai.com/enterprise-privacy](https://openai.com/enterprise-privacy)
- OpenAI business data policy: [openai.com/business-data](https://openai.com/business-data)
- Australian Privacy Act and AI guidance: [oaic.gov.au](https://oaic.gov.au)

---

*AI Adoption Co. — we help your team actually use AI.*
