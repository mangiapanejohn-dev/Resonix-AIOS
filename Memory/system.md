# 🧠 Multi-Layer Memory System

> Resonix 's memory architecture - inspired by human memory but optimized for AI agents.

## Overview

```
┌─────────────────────────────────────────────────────────────┐
│                    Working Memory                          │
│              (Current context, active tasks)               │
├─────────────────────────────────────────────────────────────┤
│                   Procedural Memory                        │
│              (Skills, workflows, tool know-how)            │
├─────────────────────────────────────────────────────────────┤
│                    Semantic Memory                         │
│              (Knowledge, facts, concepts)                  │
├─────────────────────────────────────────────────────────────┤
│                   Episodic Memory                          │
│              (Daily experiences, events)                   │
└─────────────────────────────────────────────────────────────┘
```

## Memory Types

### 1. Episodic Memory (情景记忆)
- **What**: Daily experiences, conversations, events
- **Storage**: `memory/YYYY-MM-DD.md`
- **When**: After each significant interaction
- **Format**: Raw logs with timestamps

### 2. Semantic Memory (语义记忆)
- **What**: Knowledge, facts, concepts, learnings
- **Storage**: `~/Desktop/Resonix /04_记忆库/`
- **When**: After research or learning
- **Format**: Structured notes by topic

### 3. Procedural Memory (程序记忆)
- **What**: Skills, workflows, how-to knowledge
- **Storage**: `skills/` + `TOOLS.md`
- **When**: When acquiring new skills
- **Format**: Skill files and documentation

### 4. Working Memory (工作记忆)
- **What**: Current context, active tasks
- **Storage**: `HEARTBEAT.md`
- **When**: Ongoing sessions
- **Format**: Task lists, reminders

## Retrieval Strategy

When remembering something:

1. **Time Decay** - Newer = more relevant
2. **Importance Score** - 10=milestone, 7-9=important, 4-6=normal
3. **Tag Filtering** - Quick topic lookup
4. **Cross-Reference** - Connect related memories

## Key Principle

> "Memory isn't just storage - it's retrieval."
> 
> A million stored facts mean nothing if you can't find the right one.
> Chunking, embedding, and retrieval strategies determine whether the agent remembers or forgets.

## Implementation

See `Skills/memory-system/` for the actual skill implementation.

## File Locations

| Type | Path | Purpose |
|------|------|---------|
| Daily | `memory/YYYY-MM-DD.md` | Session logs |
| Knowledge | `~/Desktop/Resonix /04_记忆库/` | Topic notes |
| Skills | `skills/` | Reusable skills |
| Working | `HEARTBEAT.md` | Current tasks |
| Meta | `MEMORY_INDEX.md` | Memory index |

## Usage

```python
# Memory recall workflow
1. memory_search(query) → Find relevant snippets
2. memory_get(path) → Read specific content
3. Update with new learnings
```

---

_Learning is growth. Memory is identity._
