# Resonix - Skill 🤖

> A production-ready AI Agent operating system with memory, learning, skills, and autonomous capabilities.

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)
[![GitHub stars](https://img.shields.io/github/stars/mangiapanejohn-dev/Resonix-Skill?style=flat&logo=github&color=4285F4&label=Stars&cacheSeconds=86400)](https://github.com/mangiapanejohn-dev/Resonix-Skill/stargazers)
## What is Resonix - Skill?

Resonix - Skill is a comprehensive framework for building intelligent AI agents with:

- 🧠 **Multi-layer Memory System** - Episodic, semantic, procedural, and working memory
- 📚 **Autonomous Learning** - Continuous knowledge acquisition and synchronization  
- 🔧 **Skill System** - Modular, reusable capabilities
- ⚡ **Workflow Automation** - Heartbeat and cron-based automation
- 🎯 **Proactive Behavior** - Self-directed action and decision making

## Quick Start

```bash
# Clone the repository
git clone https://github.com/mangiapanejohn-dev/Resonix - Skill.git
cd Resonix - Skill

# See QUICKSTART.md for detailed setup
cat QUICKSTART.md
```

## Architecture

```
Resonix - Skill/
├── Core/                 # Core systems (memory, learning, skills)
├── Config/               # Configuration templates
├── Examples/             # Minimal and full examples
├── Memory/               # Memory system docs
├── Learning/            # Learning system docs
├── Skills/              # Skill templates
├── Workflow/            # Workflow patterns
└── QUICKSTART.md        # 5-minute setup guide
```

## Features

### Memory System

| Type | Storage | Purpose |
|------|---------|---------|
| Episodic | `memory/YYYY-MM-DD.md` | Event/session records |
| Semantic | `./semantic/` | Knowledge and concepts |
| Procedural | `Skills/` | Skills and workflows |
| Working | `HEARTBEAT.md` | Current tasks |
| Meta | `MEMORY.md` | Long-term highlights |

### Learning System

- **Passive Learning** - From user interactions
- **Active Learning** - Self-initiated discovery  
- **Scheduled Learning** - Cron-based acquisition
- **Sources** - Web search, browsing, APIs, documents

### Skill System

- Modular skill definitions
- Auto-discovery
- Lazy loading
- OpenClaw integration

### Workflows

- **Heartbeat** - Periodic background checks during active sessions
- **Cron Jobs** - Scheduled tasks
- **Event Triggers** - Condition-based execution

## Documentation

| Doc | Description |
|-----|-------------|
| [QUICKSTART.md](QUICKSTART.md) | 5-minute setup guide |
| [Core/memory.md](Core/memory.md) | Memory system deep dive |
| [Core/learning.md](Core/learning.md) | Learning system configuration |
| [Examples/](Examples/) | Minimal and full examples |

## Requirements

- OpenClaw framework
- Node.js 18+
- Memory storage (filesystem or vector DB)
- Web access (for learning)

## Examples

### Minimal Setup (Testing)

```bash
cd Examples/minimal
# Just 2 files: CONFIG/agent.yaml + HEARTBEAT.md
```

### Full Setup (Production)

```bash
cd Examples/full
# Complete setup with all features
```

## Contributing

Contributions welcome! Please read the docs first.

## License

MIT License - Build your own intelligent agent!

---

**Repository**: https://github.com/mangiapanejohn-dev/Resonix - Skill
