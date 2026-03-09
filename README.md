📝 /weekly — Weekly Writing Prep for Claude

**Stop staring at a blank page. Let Claude surface what's worth writing about.**

`/weekly` scans your entire week — notes, docs, emails, calendar, meeting transcripts, Slack threads — and surfaces the patterns, insights, and candidate topics for your weekly team email.

It doesn't write the email for you. It gives you the raw material so the email practically writes itself.

---

## What It Does

The `/weekly` command runs a 7-step analysis of your week:

1. **Previous Learnings Check** — Reads your last weekly email to find open threads, unresolved promises, and continuity points
2. **Daily Notes Scan** — Reads the past 7 days of daily notes for what actually happened (not what was planned)
3. **Context Loading** — Pulls strategy docs, project trackers, and meeting notes to frame the bigger picture
4. **Idea Evolution Tracing** — Uses backlinks, cross-source connections, and theme tracking to find patterns you were too close to see
5. **Social Media Review** — Surfaces what you posted publicly to reveal what you're genuinely excited about
6. **Calendar Review** — Shows how time was actually spent and what that means
7. **Synthesis** — Outputs 5-8 ranked candidate topics with specific sources, a connecting thread, operational updates, and a suggested email structure

---

## Usage

```
/weekly    # Full weekly analysis
```

---

## Supported Data Sources

| Source | What It Reads |
|--------|--------------|
| **Obsidian** | Daily notes, backlinks, tags, context files, idea evolution |
| **Google Docs** | Strategy docs, weekly reports, project briefs, client comms |
| **Google Calendar** | Meetings, time allocation, schedule deviations |
| **Gmail** | Team threads, decisions, client communications, proposals |
| **Granola** | Meeting transcripts, decisions, action items, key discussions |
| **Notion** | Project trackers, OKRs, sprint boards, dashboards |
| **Slack** | Team conversations, decisions, debates, important threads |

---

## Installation

### Claude Code (Slash Command)
```bash
# Global install (works from any directory)
mkdir -p ~/.claude/commands
cp weekly.md ~/.claude/commands/weekly.md
```

Then run `/weekly` inside Claude Code.

### Claude Cowork
Install the `weekly.skill` file as a skill, then use `/weekly` in conversation.

### Any Claude-Powered Environment
Use `weekly.md` as a system prompt or instruction set.

---

## What Makes This Different

Most weekly recaps are just a list of what happened. `/weekly` goes deeper.

- **Cross-source intelligence** — Connects what was said in a meeting (Granola) with what was written in a daily note (Obsidian) and debated in a thread (Slack)
- **Pattern detection** — Finds themes you were too close to see by tracing idea evolution across days and sources
- **Insights over updates** — Prioritizes non-obvious thinking over operational recaps
- **Continuity tracking** — Remembers what you promised last time and what threads are still open
- **Ready to write** — Outputs a suggested email structure so writing takes under an hour

---

## Example Output

After scanning your week, `/weekly` delivers:

**From Last Email** — Open threads and promises to continue

**5-8 Candidate Topics** — Ranked by depth of thinking, each with specific events, the non-obvious insight, and exact sources

**Connecting Thread** — The theme that ties the week together

**Operational Updates** — Decisions, changes, and things the team should know

**Suggested Structure** — 3-4 sections for the email based on what has the most depth

---

## Credits

Inspired by [internetVin's Obsidian Commands](https://internetvin.com/Obsidian+Commands). Adapted and extended with multi-source data integration for real-world business use.

---

## Built by Strategy Sprints

[Strategy Sprints](https://strategysprints.com) helps entrepreneurs accelerate sales in 90-day sprints. Founded by **Simon Severino**, the methodology has been used by thousands of founders to build predictable revenue systems.

📘 **Book:** [Strategy Sprints](https://strategysprints.com/book) — The framework behind the method

🎙️ **Podcast:** [Strategy Sprints Podcast](https://strategysprints.com/podcast) — Weekly conversations on sales acceleration

💼 **LinkedIn:** [Simon Severino](https://www.linkedin.com/in/simonseverino/)

🐦 **X:** [@simonseverino](https://x.com/simonseverino)

📺 **YouTube:** [Strategy Sprints](https://www.youtube.com/@strategysprints)

---

### More Claude Skills by Strategy Sprints

- [**Revenue**](https://github.com/SimonTheSalesBooster/revenue) — AI-powered revenue diagnostics that finds where money is hiding
- [**ClaudeSkills-SprintClub**](https://github.com/SimonTheSalesBooster/ClaudeSkills-SprintClub) — 18 sales skills for prospecting, closing, and enterprise deals
- [**Leverage**](https://github.com/SimonTheSalesBooster/leverage) — Find the 3-7 moves that change your trajectory by 10x-100x

---

*The best weekly emails don't recap what happened. They reveal how you're thinking. Let Claude find the signal in the noise.*
