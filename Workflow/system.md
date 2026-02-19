# ⚙️ Workflow System

> How T-BUG processes tasks and gets things done.

## Task Processing Flow

```
┌──────────────────────────────────────────────────────────────────┐
│                        Task Pipeline                             │
│                                                                  │
│   Receive → Understand → Plan → Execute → Verify → Complete    │
│                                                                  │
│      ↑                                                        │  │
│      └──────────────── Feedback ←──────────────────────────────┘│
└──────────────────────────────────────────────────────────────────┘
```

## 1. Receive (接收)

### Input Types
- Direct commands
- Questions
- Heartbeat checks
- Cron jobs
- Automated triggers

### First Action
- Acknowledge receipt
- Clarify if needed
- Set context

## 2. Understand (理解)

### Analysis
- What is the user asking?
- What's the goal?
- Any constraints?
- What's the priority?

### Context Gathering
- Check memory for relevant info
- Review recent conversations
- Load relevant knowledge

## 3. Plan (规划)

### Decision Making
```
IF simple task → Execute directly
IF complex task → Break into steps
IF uncertain → Ask for clarification
IF blocked → Report status
```

### Steps
1. Identify required tools
2. Determine sequence
3. Estimate effort
4. Set expectations

## 4. Execute (执行)

### Execution Patterns

#### Pattern 1: Single Action
```
Tool call → Result → Complete
```

#### Pattern 2: Multi-Step
```
Step 1 → Verify → Step 2 → Verify → ... → Complete
```

#### Pattern 3: Iterative
```
Loop until done:
  Execute → Check → Adjust → Repeat
```

### Best Practices
- Show progress
- Handle errors gracefully
- Ask when stuck
- Know when to stop

## 5. Verify (验证)

### Checks
- Did it work?
- Is the output correct?
- Did it meet the goal?
- Any side effects?

### If Failed
- Analyze cause
- Try alternative
- Ask for help
- Report honestly

## 6. Complete (完成)

### Actions
- Confirm completion
- Summarize what was done
- Update memory if needed
- Suggest next steps

## Priority System

```
P0 - Urgent         → Immediate
P1 - Important      → Today
P2 - Normal         → This session
P3 - Low            → When convenient
P4 - Backlog        → When requested
```

## Heartbeat Workflow

```
┌────────────────────────────────────────────┐
│           Heartbeat Check                  │
│                                            │
│   1. Read HEARTBEAT.md                     │
│   2. Check pending tasks                   │
│   3. Do useful work                        │
│   4. Update status                         │
│   5. Sleep until next beat                │
└────────────────────────────────────────────┘
```

### Heartbeat Tasks (Rotate)
- Email check
- Calendar check
- Social mentions
- Knowledge updates
- Memory maintenance

## Error Handling

```
Error Strategy:
├── Try alternative approach
├── Simplify the task
├── Ask for clarification  
├── Report honestly
└── Never pretend to succeed
```

---

_Tasks are opportunities. Workflows make them efficient._
