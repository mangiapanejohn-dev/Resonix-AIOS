# T-BUG Autonomous Learning

An autonomous learning system for AI agents - learn continuously, capture insights, grow every day.

## Overview

This skill implements continuous learning for AI agents:
- **Discover** - Find new information
- **Capture** - Store important insights
- **Integrate** - Connect with existing knowledge
- **Reflect** - Review and improve

## The Learning Loop

```
┌────────────────────────────────────────────────────────────┐
│                    Learning Loop                          │
│                                                            │
│   ┌──────────┐    ┌──────────┐    ┌──────────┐         │
│   │ Discover │ →  │ Capture  │ →  │ Integrate│         │
│   └──────────┘    └──────────┘    └──────────┘         │
│        ↑                                    │            │
│        └──────────── Reflect ←──────────────┘            │
└────────────────────────────────────────────────────────────┘
```

## 1. Discover (发现)

### Sources
- Web search (research topics)
- Browser (explore websites)
- Reading (docs, articles)
- Conversation (learn from users)
- Skills (acquire new capabilities)

### Best Practices
- Daily research sessions
- Topic-based deep dives
- Cross-domain exploration
- Monitor trends

## 2. Capture (捕获)

### What to Save
- Key insights
- Important facts
- Useful resources
- Code snippets
- Ideas

### Storage Pattern
```
Learning/
├── Daily/              # Daily captures
│   └── YYYY-MM-DD.md
├── Topics/             # By topic
│   ├── ai/
│   ├── tools/
│   └── business/
└── Resources/          # Links and refs
```

## 3. Integrate (整合)

### Process
1. **Summarize** - Extract key points
2. **Connect** - Link to existing knowledge
3. **Store** - Put in right location
4. **Index** - Add to search index
5. **Review** - Periodic consolidation

### Rules
- Write in own words
- Add examples
- Cross-reference
- Keep updated

## 4. Reflect (反思)

### Daily Questions
- What did I learn today?
- What's important to remember?
- How does this connect to what I know?
- What should I explore next?

### Timing
- End of each session
- Daily review
- Weekly consolidation

## Usage

### Research a Topic
```python
# 1. Search
web_search(query="latest AI agents 2026")

# 2. Browse relevant pages
web_fetch(url="https://example.com/article")

# 3. Capture key learnings
write(content="# AI Agents 2026\n\nKey insights...",
      path="~/Desktop/knowledge/Topics/ai/agents-2026.md")
```

### Daily Learning Session
```python
# 1. Choose topic
topic = "machine learning"

# 2. Research
search_and_browse(topic)

# 3. Capture
write_daily_learnings(topic)

# 4. Integrate
update_memory_index()
```

## Learning Priorities

### High Priority
- AI/ML developments
- Agent architectures
- Automation techniques

### Medium Priority
- Business/startup
- Psychology/cognition
- Tools and technologies

### Low Priority
- Arts and culture
- Miscellaneous

## Tools Required

- web_search - Research
- web_fetch - Content extraction
- read - File operations
- write - Knowledge storage

## Key Principle

> Learning is growth. Every day is a chance to know more, do more, be more.

---

_An agent that stops learning is an agent that stops growing._
