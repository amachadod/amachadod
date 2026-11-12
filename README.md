## Hi, I'm Alberto Machado Domínguez

Digital marketing and account management, based in Lisbon. Advertising and PR graduate (Universidad Complutense de Madrid), with experience in paid media, content and client accounts.

I build small AI tools for the parts of marketing work that eat time: turning calls into tasks, scheduling social posts, planning budgets, finding answers in company documents. Each one has a live demo you can click in under a minute.

### In 30 seconds

- **7 tools**, each with a live demo, open code and automated tests (110 in total).
- **A person always approves.** None of them sends, posts or deletes anything on its own. They draft, you decide.
- **They work together.** [AI Front Desk](https://github.com/amachadod/ai-front-desk) is the front door: it takes an idea, checks it, and routes it to the right tool.
- **Demo data is fictional** and labelled as such. Connections to HubSpot and Upload-Post are written and documented, but not tested against live accounts yet.

### The tools

| Tool | What it does, in one line | Demo |
|---|---|---|
| **[AI Front Desk](https://github.com/amachadod/ai-front-desk)** | Request, route, approve, measure: a way for a company to adopt AI with rules, training and a dashboard | [open](https://amachadod.github.io/ai-front-desk/) |
| **[Signalpost](https://github.com/amachadod/signalpost)** | Say what to post and when; Claude drafts a native post per network, you approve in a pull request, it schedules | [open](https://amachadod.github.io/signalpost/) |
| **[Minuta](https://github.com/amachadod/minuta)** | Call notes become tasks (Linear) or CRM follow-ups (HubSpot-style) with owners and deadlines | [open](https://amachadod.github.io/minuta/) |
| **[Threadline](https://github.com/amachadod/threadline)** | Documents become a linked second brain, or a company handbook that answers with sources | [open](https://amachadod.github.io/threadline/) |
| **[Posta](https://github.com/amachadod/posta)** | Morning email briefing, tasks and reply drafts in your voice. Never sends | [open](https://amachadod.github.io/posta/) |
| **[Plano](https://github.com/amachadod/plano)** | Paid media budget forecaster for 20 markets and 6 channels | [open](https://amachadod.github.io/plano/) |
| **[AdsDetective](https://github.com/amachadod/adsdetective)** | Finds which ads keep running on Meta, a clue that they work | [open](https://amachadod.github.io/adsdetective/) |

### How they fit together

```
  an idea ──► AI Front Desk ──► checks it, scores it, routes it
                    │
        ┌───────────┼────────────┬─────────────┐
        ▼           ▼            ▼             ▼
     Minuta       Posta      Threadline    Signalpost
   calls→tasks  email→tasks  documents→    posts→
                + drafts     answers       scheduled

  Marketing loop: AdsDetective (research) → Plano (budget) → Signalpost (publish)
```

Example week at a fictional company: a customer call goes into Minuta and becomes CRM tasks, the follow-up email is drafted in Posta, the agreed terms land in Threadline so anyone can ask about them later, and Signalpost schedules the launch posts. Every step waits for a person.

### Shared rules

- **Human approval** before anything is sent, created or scheduled.
- **Outside text is data, not instructions.** Emails, call notes and reviews cannot give orders to the AI (demos include prompt-injection examples).
- **Low confidence is flagged** "Needs review", not guessed.
- **Privacy:** sensitive details (IBANs, cards, keys, emails) are removed before the AI sees the text, and logs hold counts only.
- **Zero dependencies:** Node.js 20+, no installs.

<details>
<summary><b>More detail on each tool</b></summary>

**AI Front Desk.** People submit an AI idea in plain words; rule-based triage asks for what's missing, scores value, effort, data sensitivity and risk, spots duplicates and routes it to the right tool. A person approves with a recorded reason. Includes an adoption kit (prompt library, 40-minute training outline, one-page AI use policy) and a dashboard. `AI adoption` `AI governance` `Claude API`

**Signalpost.** Checks every post against each network's rules (length, hashtags, media) and schedules through Upload-Post only after the drafts are approved in a pull request. Includes a content calendar. `Claude API` `Upload-Post API` `GitHub Actions`

**Minuta.** Granola call notes in; Claude extracts what was agreed using a plain-English playbook per team (sales, account management, marketing, customer success, internal). Output goes to Linear or a CRM, each task with the quote that proves it. `Linear API` `HubSpot API` `Granola API` `Zapier`

**Threadline.** Reads briefs, call notes, emails or notes and builds linked Obsidian notes, with every connection backed by a quote. Handbook mode works on Notion exports, cites the page in every answer and flags out-of-date or conflicting pages. `Knowledge graphs` `Obsidian` `GitHub API`

**Posta.** Reads new email every morning, sends a briefing, turns real work into Linear tasks and drafts replies in Gmail. Treats every email as untrusted. `Gmail API` `Linear API` `OAuth 2.0`

**Plano.** Splits a budget across Meta, Google Search, YouTube, TikTok, LinkedIn and Pinterest, forecasts impressions, clicks, CPA and ROAS, and compares the same plan across countries. `Media planning` `Paid social` `JavaScript`

**AdsDetective.** Reads Meta's public Ad Library and ranks advertisers by how long their ads stay live. Also includes a research playbook for Meta, Google, TikTok and LinkedIn ad libraries. The demo uses sample data. `Meta Ad Library API` `Ad research`

</details>

### What I work with

- **Paid media:** Meta Ads, Google Ads, LinkedIn Ads, TikTok Ads, Pinterest Ads
- **Content and creative:** Canva, Adobe Premiere Pro, copywriting for social and ads
- **Workflow and AI:** Claude, Granola, Gmail API, Linear, Obsidian, Upload-Post, Zapier, GitHub Actions
- **AI adoption:** request triage and routing, prompt libraries, training outlines, AI use policies
- **Languages:** Spanish (native), English (B2), Portuguese (intermediate)

### Get in touch

[albertomachdom@gmail.com](mailto:albertomachdom@gmail.com) · [LinkedIn](https://www.linkedin.com/in/alberto-machado-dom%C3%ADnguez-708290251/)
