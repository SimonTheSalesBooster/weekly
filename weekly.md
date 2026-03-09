# Weekly Learnings — Writing Prep

Help figure out what to write about in a weekly team email. Surface patterns, insights, and candidate topics from the week. Output everything to terminal. Do NOT create any files.

---

## Data Source Access

This command reads from multiple sources. Use all available tools to gather context before analysis.

### Obsidian Vault
If the Obsidian CLI is available, use it for all vault reads and searches. It's significantly faster than filesystem tools and gives the agent direct access to backlinks, tags, search, and file metadata in real time. All Obsidian commands below assume the CLI. If it's not available, fall back to reading files directly from the vault directory.

### Google Docs
Search Google Drive for relevant documents: strategy updates, weekly reports, project briefs, team updates, client communications, and any reflective or strategic writing from the past week.

### Google Calendar
Review the past 7 days of calendar events for: key meetings, external calls, team syncs, how time was actually spent vs. intended, and any deviation from the normal structure.

### Gmail
Search recent emails (past 7 days) for: important team conversations, client communications, decisions made via email, things that came up worth reflecting on, and any threads that signal shifting priorities.

### Granola (Meeting Notes)
Query Granola for the past 7 days of meeting notes to extract: key decisions, insights from conversations, things that shifted thinking, action items, and discussions worth surfacing to the team.

### Notion
Search Notion for: project updates, team dashboards, sprint progress, OKR tracking, and any operational data that reveals what actually happened this week vs. what was planned.

### Slack
Search Slack for: important team conversations from the past 7 days, decisions made in channels, topics with energy or debate, things that came up worth reflecting on, and any threads that signal what the team is thinking about.

---

## Step 1: Read Previous Weekly Learnings (Continuity)

Search across all data sources for the two most recent weekly learnings or weekly update emails:

```
Obsidian search query="Weekly Learnings"
Obsidian read file="<most recent weekly learnings>"
```

Also search Gmail for recent sent emails with weekly updates, and Google Docs for any weekly learnings drafts.

Extract:
- What was written about last time (so we don't repeat without development)
- Threads that were opened but not resolved
- Things promised ("I'll write more about this soon")
- The tone and style (first person, reflective, connects specific events to broader ideas)

---

## Step 2: Read Daily Notes (Past 7 Days)

Use the Obsidian CLI to read all daily notes from the past 7 days:

```
Obsidian daily:read
Obsidian read path="Daily Notes/YYYY-MM-DD.md"   # for each of the past 6 days
```

Extract:
- What was actually worked on this week (not what was planned, what happened)
- Conversations and meetings that shifted thinking
- Ideas that emerged (especially ones with energy behind them)
- Decisions made or direction changes
- Problems encountered and how they were handled
- People mentioned and what the interactions were about
- Frustrations, breakthroughs, and realizations
- Anything that was surprising

---

## Step 3: Load Context Files

Use the Obsidian CLI to read context files for current state and priorities:

```
Obsidian read file="<Company-Context>"
Obsidian read file="<Project-Context>"
Obsidian read file="Personal Workflow Context"
```

Also pull context from:
- **Google Docs**: Strategy documents, quarterly plans, or project briefs that frame the bigger picture
- **Notion**: Active project trackers, OKRs, sprint boards, or dashboards that show current priorities
- **Granola**: Meeting notes from strategic conversations this week

Use these to understand which events from the week connect to bigger strategic questions. The weekly learnings work best when specific things that happened reveal something about the larger direction.

---

## Step 3.5: Trace Idea Evolution

Use the Obsidian CLI to explore how this week's thinking connects across notes and to the broader vault:

```
Obsidian backlinks file="<key notes referenced this week>"
Obsidian search:context query="<recurring theme from daily notes>"
Obsidian tags counts sort=count   # what themes dominated this week
Obsidian links file="<daily note>"  # for each day, see what it connects to
```

Also trace idea evolution across other sources:
- **Slack**: Threads where ideas were debated or refined during the week
- **Granola**: Meeting conversations where thinking evolved or shifted
- **Gmail**: Email threads where a topic developed over multiple exchanges

Look for:
- Ideas that appeared on multiple days this week (evolving thinking worth highlighting)
- Backlink chains showing how a conversation or meeting rippled into later thinking
- Themes from daily notes that connect to open questions in context files
- Notes from previous weeks that this week's thinking builds on or contradicts

The best weekly learnings come from noticing patterns the writer was too close to see. Use the graph structure and cross-source connections to find these.

---

## Step 4: Review Social Media Activity

Review recent posts (past 7 days).

Look for:
- Topics posted about publicly (these are things on your mind)
- Posts with high engagement (ideas that resonated)
- Threads or longer posts (these often contain the week's deepest thinking)
- Things shared about the company, projects, or events

These often reveal what you're genuinely excited about vs. what's just operational.

---

## Step 5: Review Calendar (Past 7 Days)

Pull the past week's calendar using Google Calendar.

Look for:
- Key meetings that happened (especially external ones, recordings, team syncs)
- How time was actually spent
- Any deviation from the intended structure (and what that means)

Cross-reference with Granola meeting notes for the actual substance of what was discussed.

---

## Step 6: Review Messages

Scan recent messages across all channels:

- **Slack**: Important team conversations, decisions made, topics with energy
- **Gmail**: Key threads, decisions, things worth reflecting on
- **Granola**: Meeting discussions that surfaced important thinking

Look for:
- Important team conversations
- Decisions made
- Things that came up worth reflecting on for the team

---

## Step 7: Synthesize — Output to Terminal

Print everything below directly to the terminal. Do NOT create any files.

### Output Format:

```
WEEKLY LEARNINGS PREP -- Week [number], [year]

FROM LAST EMAIL (threads to continue or resolve):
- [Thread from previous email that developed further this week]
- [Promise made that can now be addressed]

CANDIDATE TOPICS (ranked by depth of thinking + relevance to team):

[#]. [Topic name] -- [Project area]
    What happened: [Specific events, conversations, or decisions]
    The insight: [The non-obvious thing worth sharing]
    Source: [Which daily notes, meetings, Slack threads, or posts contain the raw thinking]

List 5-8 candidates.

CONNECTING THREAD:
If there's a theme that ties multiple things together this week, name it. The best emails connect specifics to a bigger idea.

OPERATIONAL UPDATES (not learnings, but the team should know):
- [Decisions, schedule changes, deals closed, etc.]

SUGGESTED STRUCTURE:
Recommend 3-4 sections for the email based on what has the most depth. The email should take no more than an hour to write.
```

---

## Output Guidelines

- Print everything to terminal. No file creation.
- Be specific: cite which daily note, which meeting, which Slack thread, which email, which post.
- Prioritize insights over updates. The team doesn't need a recap. They need to understand how you're thinking.
- Match existing tone: first person, reflective, connects specific events to broader ideas.
- Cross-reference sources: the best insights often come from connecting something said in a meeting (Granola) with something written in a daily note (Obsidian) or debated in a thread (Slack).
