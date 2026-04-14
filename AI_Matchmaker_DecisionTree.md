# AI Assistant Matchmaker — Decision Tree Reference

This document maps every node, branching path, and result screen in the AI Assistant Matchmaker app. Use it as the source of truth when building slides or UI screens.

---

## How to Read This Document

- **Question nodes** are numbered screens with a question and two or more answer paths.
- **Result screens** are final destination screens. Each includes ready-to-use copy for the app.
- Arrows show where each answer leads.

---

## Question Nodes

---

### Node 1 — Start Screen
**"What are you trying to do?"**

| Answer | Goes to |
|---|---|
| Research / Web Browsing | Node 3 |
| Creative writing / Coding | Node 2 |

---

### Node 2
**"Do you need the AI to handle huge documents, like an entire codebase or a full book?"**

| Answer | Goes to |
|---|---|
| Yes | Node 4 |
| No | Node 5 |

---

### Node 3
**"Do you need strict, sourced citations, like you'd expect in an academic paper?"**

| Answer | Goes to |
|---|---|
| Yes | Node 6 |
| No | Node 7 |

---

### Node 4
**"What's the main focus of those large documents?"**

| Answer | Goes to |
|---|---|
| Deep writing and analysis | Node 8 |
| Advanced data crunching or code execution | Node 9 |

---

### Node 5
**"Do you prefer working with an open-source model?"**

| Answer | Goes to |
|---|---|
| Yes | Node 10 |
| No | Node 11 |

---

### Node 6
**"Are you already working inside Google Workspace?"**

| Answer | Goes to |
|---|---|
| Yes | → **Result: Gemini** |
| No | → **Result: Perplexity** |

---

### Node 7
**"Are you looking for something built directly into Microsoft Office and Windows?"**

| Answer | Goes to |
|---|---|
| Yes | → **Result: Copilot** |
| No | Node 12 |

---

### Node 8
**"Is data privacy and keeping your documents off corporate servers a concern?"**

| Answer | Goes to |
|---|---|
| Yes | → **Result: Mistral** |
| No | → **Result: Claude** |

---

### Node 9
**"What's the main focus of those large documents?"**

| Answer | Goes to |
|---|---|
| Yes (data crunching / code execution confirmed) | → **Result: ChatGPT Plus** |
| No | Node 13 |

---

### Node 10
**"Which open-source community fits your workflow better?"**

| Answer | Goes to |
|---|---|
| Meta's Llama ecosystem | → **Result: Llama** |
| A leaner, European-built model | → **Result: Mistral** |
| A developer-focused, high-reasoning model | → **Result: DeepSeek** |

---

### Node 11
**"Are you looking for an AI with a distinct conversational personality, not just a generic assistant?"**

| Answer | Goes to |
|---|---|
| Yes | Node 14 |
| No, just clean, reliable output | → **Result: Claude** |

---

### Node 12
**"Are you more interested in real-time social trends, or personal coaching and emotional support?"**

| Answer | Goes to |
|---|---|
| Real-time social trends | Node 15 |
| Personal coaching / emotional support | → **Result: Pi** |

---

### Node 13
**"Are you looking for a free or low-cost option?"**

| Answer | Goes to |
|---|---|
| Paid is fine | → **Result: ChatGPT Plus** |
| Free tier | → **Result: Gemini** |

---

### Node 14
**"What kind of personality are you looking for?"**

| Answer | Goes to |
|---|---|
| Warm, empathetic, and focused on personal growth | → **Result: Pi** |
| Unfiltered, fast, and plugged into social media | → **Result: Grok** |

---

### Node 15
**"Do you want the AI to pull from live social media feeds and real-time posts?"**

| Answer | Goes to |
|---|---|
| Yes | → **Result: Grok** |
| No, general up-to-date web info is fine | → **Result: Gemini** |

---

---

## Result Screens — Full Copy

Each result screen includes: a headline, a one-sentence description of the tool, and a short "why it's your match" explanation based on the path the user took.

---

### Result: ChatGPT Plus
**Your match: ChatGPT Plus**

*ChatGPT Plus is OpenAI's premium AI assistant, built for serious, high-output work across writing, analysis, coding, and data tasks.*

**Why it's your match:**
You're working with large, data-heavy documents and need an AI that can actually process, analyze, and run code on them. ChatGPT Plus gives you Code Interpreter, file uploads, and one of the most capable reasoning engines available — all in one place. If your workflow involves spreadsheets, datasets, or running real computations, this is where you want to be.

---

### Result: Claude
*(Path A — Deep writing, large documents, no privacy concern)*
**Your match: Claude**

*Claude is Anthropic's AI assistant, known for handling long, complex documents with careful, nuanced analysis.*

**Why it's your match:**
You're dealing with large documents and your priority is depth of writing and analysis — not running code. Claude has one of the longest context windows of any AI, meaning it can hold an entire book or codebase in memory and reason through it thoughtfully. It's especially strong at summarizing, editing, and drawing careful conclusions from dense material.

---

*(Path B — Creative writing/coding, no large docs, no distinct personality needed)*
**Your match: Claude**

*Claude is Anthropic's AI assistant, designed for thoughtful, high-quality writing and coding without the noise.*

**Why it's your match:**
You want a clean, reliable AI that does the work without performing a personality. Claude is consistently praised for the quality of its writing, its careful reasoning, and its ability to follow nuanced instructions. Whether you're drafting, editing, or building something, you'll get clear, useful output without a lot of fuss.

---

### Result: Gemini
*(Path A — Research, citations needed, already in Google Workspace)*
**Your match: Gemini**

*Gemini is Google's AI assistant, built directly into Google Docs, Gmail, Drive, and the rest of the Google Workspace ecosystem.*

**Why it's your match:**
You already live inside Google Workspace, and Gemini is the only AI that's actually embedded there. Instead of copying and pasting between tools, you can use AI directly inside the documents and emails you're already working with. It's the most frictionless choice for anyone deep in the Google ecosystem.

---

*(Path B — Research, no strict citations, not Microsoft-focused, interested in real-time social trends, no live social feeds needed)*
**Your match: Gemini**

*Gemini is Google's AI assistant, with strong web access and real-time search built in.*

**Why it's your match:**
You want to stay on top of what's happening in the world without needing direct social media integration. Gemini is connected to Google Search and surfaces current, relevant information quickly. It's a dependable everyday assistant for research, summarization, and staying informed — without the social media noise.

---

*(Path C — Large documents for data crunching, free tier preferred)*
**Your match: Gemini**

*Gemini is Google's AI assistant, and its free tier is one of the most capable available without a subscription.*

**Why it's your match:**
You need help with large, data-heavy documents but you're not ready to pay for a subscription. Gemini's free tier gives you access to strong AI capabilities backed by Google's infrastructure — including solid reasoning, web access, and support for long documents — at no cost.

---

### Result: Copilot
**Your match: Microsoft Copilot**

*Microsoft Copilot is Microsoft's AI assistant, built directly into Word, Excel, Outlook, Teams, and Windows.*

**Why it's your match:**
You're already in the Microsoft ecosystem and want an AI that works where you already are — not a separate app you have to switch to. Copilot is embedded right inside the tools you use every day. Ask it to summarize a document in Word, generate a formula in Excel, or draft a reply in Outlook, all without leaving your workflow.

---

### Result: Perplexity
**Your match: Perplexity**

*Perplexity is an AI-powered search engine that gives you direct, sourced answers with citations you can actually verify.*

**Why it's your match:**
You need your information to be backed up with sources — not just a confident-sounding answer. Perplexity pulls from the web in real time and cites every claim, so you can trace exactly where the information came from. It's the closest thing to having a research assistant who shows their work.

---

### Result: Llama
**Your match: Llama**

*Llama is Meta's open-source AI model, freely available for anyone to download, run, and modify.*

**Why it's your match:**
You want an open-source model and you're comfortable in the Meta ecosystem — the most widely adopted open-source AI community in the world. Llama gives you the flexibility to run the model locally, fine-tune it for specific tasks, and build on top of it however you need. It's the go-to choice for developers and researchers who want full control without vendor lock-in.

---

### Result: Mistral
*(Path A — Open-source, European-built model preferred)*
**Your match: Mistral**

*Mistral is a French AI company building lean, efficient open-source models with a focus on performance and privacy.*

**Why it's your match:**
You want open-source, but you're drawn to a model that's a bit more compact and purpose-built — not a massive ecosystem play. Mistral's models are fast, efficient, and developed by a team with a strong commitment to European data standards. If you care about where your AI comes from and want something that punches above its size, Mistral is a smart pick.

---

*(Path B — Large documents, deep writing, privacy is a concern)*
**Your match: Mistral**

*Mistral is a French AI company building efficient, privacy-respecting AI models that can be run on your own infrastructure.*

**Why it's your match:**
You're working with sensitive documents and you're not comfortable sending them to a major corporate AI provider. Mistral lets you self-host, meaning your data stays on your own servers and never passes through someone else's system. For legal documents, confidential reports, or anything that needs to stay private, that's not a nice-to-have — it's the whole point.

---

### Result: Pi
*(Path A — Distinct personality, warm and focused on personal growth)*
**Your match: Pi**

*Pi is a personal AI designed around emotional intelligence, active listening, and genuine conversation.*

**Why it's your match:**
You're not looking for a task-completion machine. You want an AI that actually engages with you — asks follow-up questions, remembers context, and responds with warmth. Pi is built specifically for that kind of interaction. Think of it less like a search engine and more like a thoughtful conversation partner who's always available and never in a rush.

---

*(Path B — Research, no strict citations, not Microsoft-focused, personal coaching and emotional support)*
**Your match: Pi**

*Pi is a personal AI designed around emotional intelligence, active listening, and genuine conversation.*

**Why it's your match:**
You're less interested in finding facts and more interested in working things through — making decisions, reflecting on goals, or just having a conversation with something that listens. Pi specializes in that. It's calm, curious, and personal in a way most AI tools aren't. If you want support rather than just answers, Pi fits better than anything else on this list.

---

### Result: Grok
*(Path A — Distinct personality, unfiltered and plugged into social media)*
**Your match: Grok**

*Grok is xAI's AI assistant, built with a direct personality and real-time access to posts and trends on X (formerly Twitter).*

**Why it's your match:**
You want an AI with an actual edge to it — not one that hedges everything and plays it safe. Grok is faster, more willing to engage with edgy or unconventional questions, and plugged directly into what's trending on social media right now. If you want an AI that keeps up with the internet in real time and doesn't feel like a corporate product, Grok is your match.

---

*(Path B — Real-time social trends, wants live social media feeds)*
**Your match: Grok**

*Grok is xAI's AI assistant with native real-time access to X (formerly Twitter), including live posts, trending topics, and social media conversations.*

**Why it's your match:**
You specifically want an AI that's tapped into what people are actually saying on social media right now — not just what Google has indexed. Grok reads live posts from X, tracks trending conversations, and can summarize what the internet is talking about in real time. No other AI on this list does that.

---

### Result: DeepSeek
**Your match: DeepSeek**

*DeepSeek is a Chinese AI lab's open-source model that has gained attention for its strong performance on complex reasoning and coding tasks.*

**Why it's your match:**
You want open-source, and you need something that goes deep on technical problems. DeepSeek has made waves for matching or exceeding much larger models on coding and math benchmarks — while still being fully open and free to use. If your work is heavy on logic, code, or structured reasoning, DeepSeek is worth putting at the top of your list.

---

---

## Full Path Summary Table

| Path | Nodes Traveled | Result |
|---|---|---|
| Research → Citations needed → In Google Workspace | 1 → 3 → 6 (Yes) | Gemini |
| Research → Citations needed → Not in Google Workspace | 1 → 3 → 6 (No) | Perplexity |
| Research → No strict citations → Microsoft Office | 1 → 3 → 7 (Yes) | Copilot |
| Research → No strict citations → Not Microsoft → Social trends → Live feeds | 1 → 3 → 7 (No) → 12 → 15 (Yes) | Grok |
| Research → No strict citations → Not Microsoft → Social trends → No live feeds | 1 → 3 → 7 (No) → 12 → 15 (No) | Gemini |
| Research → No strict citations → Not Microsoft → Personal coaching | 1 → 3 → 7 (No) → 12 (coaching) | Pi |
| Creative/Coding → Large docs → Deep writing → Privacy concern | 1 → 2 → 4 → 8 (Yes) | Mistral |
| Creative/Coding → Large docs → Deep writing → No privacy concern | 1 → 2 → 4 → 8 (No) | Claude |
| Creative/Coding → Large docs → Data/code → Paid is fine | 1 → 2 → 4 → 9 (Yes) | ChatGPT Plus |
| Creative/Coding → Large docs → Data/code → Free tier | 1 → 2 → 4 → 9 (No) → 13 (free) | Gemini |
| Creative/Coding → No large docs → Open source → Llama ecosystem | 1 → 2 → 5 → 10 (Llama) | Llama |
| Creative/Coding → No large docs → Open source → European model | 1 → 2 → 5 → 10 (Mistral) | Mistral |
| Creative/Coding → No large docs → Open source → High-reasoning model | 1 → 2 → 5 → 10 (DeepSeek) | DeepSeek |
| Creative/Coding → No large docs → Not open source → No distinct personality | 1 → 2 → 5 → 11 (No) | Claude |
| Creative/Coding → No large docs → Not open source → Warm personality | 1 → 2 → 5 → 11 → 14 (warm) | Pi |
| Creative/Coding → No large docs → Not open source → Unfiltered personality | 1 → 2 → 5 → 11 → 14 (unfiltered) | Grok |
