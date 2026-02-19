# T-BUG Memory System

A multi-layer memory system for AI agents, inspired by human memory architecture.

## Overview

This skill implements a memory system for AI agents with:
- **Episodic Memory** - Daily experiences and events
- **Semantic Memory** - Knowledge base and concepts
- **Procedural Memory** - Skills and workflows
- **Working Memory** - Current context and tasks

## Installation

Copy this folder to your agent's skills directory.

## Configuration

### File Locations (Customize)

```json
{
  "episodic": "memory/",
  "semantic": "~/Desktop/knowledge/",
  "procedural": "skills/",
  "working": "HEARTBEAT.md",
  "index": "MEMORY_INDEX.md"
}
```

## Memory Types

### 1. Episodic (Daily)
- Path: `memory/YYYY-MM-DD.md`
- Content: Raw session logs, events
- When: After significant interactions

### 2. Semantic (Knowledge)
- Path: `~/Desktop/knowledge/04_记忆库/`
- Content: Structured notes by topic
- When: After research or learning

### 3. Procedural (Skills)
- Path: `skills/` + `TOOLS.md`
- Content: Capabilities and how-tos
- When: Acquiring new skills

### 4. Working (Current)
- Path: `HEARTBEAT.md`
- Content: Active tasks, context
- When: Ongoing sessions

## Tools

### memory_search
Mandatory recall before answering questions about:
- Prior work
- Decisions
- Dates and events
- People and preferences
- Todos

Returns top snippets with path + lines.

### memory_get
Safe snippet read after memory_search.
- Optional `from` and `lines` params
- Keeps context small

## Usage

```python
# Before answering about past work
memory_search(query="what did we build")

# After finding relevant info
memory_get(path="memory/2026-02-15.md", from=10, lines=20)

# Save new learning
write(content="# New Learning\n...", 
      path="~/Desktop/knowledge/04_记忆库/topic.md")
```

## Retrieval Strategy

1. **Time Decay** - Newer = more relevant
2. **Importance Score**:
   - 10 = milestone
   - 7-9 = important
   - 4-6 = normal
   - 1-3 = temporary
3. **Tag Filtering** - Quick topic lookup
4. **Cross-Reference** - Connect related memories

## Best Practices

1. **Write immediately** - Don't trust mental notes
2. **Use meaningful names** - File names matter
3. **Cross-reference** - Link related info
4. **Periodic review** - Consolidate memories
5. **Keep updated** - Delete outdated info

## Key Principle

> "Memory isn't just storage - it's retrieval."
> 
> A million stored facts mean nothing if you can't find the right one.

## File Structure

```
memory-system/
├── SKILL.md           # This file
├── config.json        # Configuration
├── search.py          # Search logic
├── get.py            # Retrieval logic
├── write.py          # Storage logic
└── templates/        # Note templates
```

---

_Building an agent? Start with memory. Without it, every conversation starts from zero._
