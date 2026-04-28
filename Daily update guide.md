# 📋 README Daily Update Cheatsheet

Quick reference — every time you sit down to work, spend 2 minutes updating.

---

## ✅ What to Update & Where

### After every work session (5 min max)

| What happened | Where to update | Example |
|---|---|---|
| Learned something | `## What I Learned` in relevant project README | `- [2025-01-15] auditd rules are syscall-level, not process-level` |
| Finished a task | GitHub Issues → close the issue | Commit message: `closes #5` |
| Crossed a milestone | `## Project Progress` table | Change `⬜` to `✅` |
| Started something new | Open a new GitHub Issue | Title: "Parse Zeek conn.log format" + label: "in progress" |
| Got blocked | GitHub Issue → add "blocked" label + comment why | — |

### Once a week (Sunday, 5 min)

| What | Where |
|---|---|
| Update "Currently Learning" | Profile README → `## Currently Learning` |
| Add a row to Journey Log | Profile README → `## Journey Log` |
| Update project status badge | Profile README → project table (⬜ → 🟡 → ✅) |

---

## 🏷️ GitHub Issue Workflow

```
1. Before starting any task → Open an Issue
   Title: what you're building ("Add Zeek parser module")
   Label: "in progress"

2. While working → commit with issue reference
   git commit -m "feat: parse conn.log fields — refs #7"

3. When done → close with commit
   git commit -m "feat: zeek parser complete — closes #7"
   Label: "done"

4. If stuck → add "blocked" label + comment explaining why
```

---

## 📝 "What I Learned" Entry Format

```markdown
- [YYYY-MM-DD] One sentence. Concrete. Specific. Not "learned about X" but
  "X works this way because Y, which means Z in practice."
```

**Good:** `- [2025-01-15] Sysmon Event ID 1 logs process creation including parent PID, which is how you detect LOLBas chains`  
**Bad:** `- [2025-01-15] Learned about Sysmon`

---

## 🖼️ Architecture Diagram Workflow

1. Go to [draw.io](https://draw.io) (free, no account needed)
2. Draw your diagram (boxes + arrows, simple is fine)
3. Export: **File → Export As → PNG** → save as `docs/architecture.png`
4. Also save the source: **File → Save** → `docs/architecture.drawio`
5. Commit both files
6. In README, replace the placeholder with: `![Architecture](./docs/architecture.png)`

---

## 🔄 Status Badge Reference

In project READMEs, update the status badge as you progress:

```markdown
<!-- Not started -->
![Status](https://img.shields.io/badge/status-planned-lightgrey)

<!-- Active work -->
![Status](https://img.shields.io/badge/status-in_progress-yellow)

<!-- Done -->
![Status](https://img.shields.io/badge/status-complete-brightgreen)
```

---

## 📸 Screenshot Workflow

When something works visually (dashboard, terminal output):
1. Take screenshot → save to `docs/screenshots/FEATURE-NAME.png`
2. Add to Usage Examples section: `![Dashboard](./docs/screenshots/dashboard.png)`
3. Commit with message: `docs: add dashboard screenshot`

---

## 🔗 Quick Links

- [Home SOC Lab Issues](https://github.com/USERNAME/home-soc-lab/issues)
- [Log Parser CLI Issues](https://github.com/USERNAME/log-parser-cli/issues)
- [SOC Triage Agent Issues](https://github.com/USERNAME/soc-triage-agent/issues)
- [Draw.io](https://draw.io)
- [Shields.io badge generator](https://shields.io)