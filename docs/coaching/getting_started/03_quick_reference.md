---
title: "Getting Started with pay_no_attention - Quick Reference"
author: "Dan Brickey"
version: "1.0.0"
last_updated: "2025-10-25"
category: "coaching"
tags: ["quick-reference", "cheat-sheet", "getting-started"]
status: "active"
---

# Quick Reference: pay_no_attention Project

**Print this page and keep it handy!**

---

## Essential Git Commands

| Command | What It Does | When to Use |
|---------|--------------|-------------|
| `git status` | Shows what's changed | Before committing |
| `git add .` | Stages all changes | Before committing |
| `git commit -m "message"` | Saves changes locally | After making changes |
| `git push` | Backs up to GitHub | After committing |
| `git pull` | Gets latest from GitHub | Before starting work |

**Memory Aid**: **C**lone → **A**dd → **C**ommit → **P**ush (CACP)

📖 [Detailed Git Instructions → Student Manual Part 2](02_student_manual.md#part-2-foundation-setup-git-github-vs-code)

---

## Key Folder Locations

```
pay_no_attention/
├── .ai/instructions.md          ← Your personal AI config
├── ai-resources/prompts/        ← The 93-prompt library
│   ├── meta/                    ← @bootstrap, @nav, @discover
│   ├── career/                  ← Career paths
│   └── utilities/               ← Maintenance, gifts, etc.
└── docs/                        ← Your documents go here
```

📖 [Directory Structure Details → Student Manual Part 1](02_student_manual.md#understanding-the-directory-structure)

---

## The Core Workflow

### 1. Setup (One Time)
```bash
# Clone repo
git clone https://github.com/danbrickey/pay_no_attention.git

# Create YOUR repo
mkdir my-ai-assistant
cd my-ai-assistant
git init
```

### 2. Personalize (First Use)
```
@bootstrap
```
Answer 7 questions → AI creates your `.ai/instructions.md`

### 3. Daily Use
```
@nav              # Find prompts
@discover         # Search by topic
@[prompt-name]    # Use any prompt
```

📖 [Complete Setup Instructions → Student Manual Part 2](02_student_manual.md#setting-up-vs-code-github-and-git)

---

## Common Tasks

| I Want To... | Use This Prompt | Where It Lives |
|-------------|-----------------|----------------|
| Find prompts by topic | `@discover [topic]` | `prompts/meta/discover-prompt-finder.md` |
| Browse all prompts | `@nav` | `prompts/meta/nav-resource-navigator.md` |
| Change career | `@career-analyzer` | `prompts/career/career-analyzer.md` |
| Build my CV | `@career-cv` | `prompts/career/career-cv-interviewer.md` |
| Document equipment | `@equipment-doc` | `prompts/utilities/equipment-maintenance-documenter.md` |
| Plan maintenance | `@maintenance-planner` | `prompts/utilities/household-maintenance-planner.md` |
| Find gifts | `@giftfinder` | `prompts/utilities/giftfinder-shopping-assistant.md` |

📖 [Full Prompt Library → Student Manual Part 1](02_student_manual.md#the-prompt-library-93-ready-to-use-prompts)

---

## Career Planning Quick Path

```
Step 1: Build your CV
@career-cv

Step 2: Analyze career options
@career-analyzer

Step 3: Compare 2-5 paths
Get qualification tiers + roadmaps

Step 4: Pick your target
Follow 30-day sprint plan
```

📖 [Detailed Career Lab → Student Manual Part 4](02_student_manual.md#part-4-lab-2---career-planning-with-ai-30-minutes)

---

## Maintenance Documentation Quick Path

```
Step 1: Document each item
@equipment-doc
- Take 5-10 photos
- Upload manual if available
- Answer questions

Step 2: Create master schedule
@maintenance-planner
- AI reads all your equipment docs
- Generates unified calendar
- Adjusts for your climate
```

📖 [Detailed Maintenance Lab → Student Manual Part 5](02_student_manual.md#part-5-lab-3---maintenance-documentation-25-minutes)

---

## Troubleshooting

| Problem | Solution | More Info |
|---------|----------|-----------|
| Can't find a prompt | Use `@nav` or `@discover [keyword]` | [Student Manual Part 1](02_student_manual.md#how-to-find-prompts) |
| Git says "not a repository" | Run `git init` in your folder | [Student Manual Part 2](02_student_manual.md#troubleshooting) |
| AI doesn't remember me | Check `.ai/instructions.md` exists | [Student Manual Part 3](02_student_manual.md#troubleshooting-1) |
| Push failed | Run `git pull` first, then `git push` | [Student Manual Part 2](02_student_manual.md#common-git-problems) |
| Career path not listed | Use `@career-analyzer` with custom role | [Student Manual Part 4](02_student_manual.md#troubleshooting-2) |
| Maintenance schedule wrong | Edit climate in `@maintenance-planner` | [Student Manual Part 5](02_student_manual.md#troubleshooting-3) |

📖 [Complete Troubleshooting Guide → Student Manual](02_student_manual.md)

---

## Key Principles (Remember These!)

### 1. Context Is King
The AI remembers what's in `.ai/instructions.md` - keep it updated!

### 2. Prompts Are Tools
Don't just chat - use the specialized prompts for structured workflows

### 3. Save Everything
Commit → Push to GitHub regularly (your future self will thank you)

### 4. Experiment Safely
Git makes it safe to try things - you can always undo

### 5. Build Incrementally
Start simple (one document) → Expand (more areas) → Refine (better prompts)

📖 [Philosophy & Best Practices → Student Manual Part 1](02_student_manual.md#the-pay-no-attention-philosophy)

---

## Quick Decision Trees

### "Which Career Prompt Should I Use?"

```
Do you have a CV/resume already?
├─ Yes → Use @career-analyzer to compare paths
└─ No → Use @career-cv first, THEN @career-analyzer

Know your target role?
├─ Yes → Browse career/[industry]_career_paths/
└─ No → Use @career-analyzer to explore options
```

### "Which Maintenance Prompt First?"

```
Have equipment docs already?
├─ Yes → Use @maintenance-planner to create schedule
└─ No → Use @equipment-doc for each item first

One item or many?
├─ One item → @equipment-doc
└─ Multiple items → @equipment-doc each, THEN @maintenance-planner
```

📖 [Detailed Workflows → Student Manual Parts 4-5](02_student_manual.md#part-4-lab-2---career-planning-with-ai-30-minutes)

---

## File Naming Conventions

**Good Examples**:
```
docs/career/cv_john_smith_2025.md
docs/maintenance/2015_honda_civic_maintenance.md
docs/maintenance/master_schedule_2025.md
```

**Why This Matters**:
- Consistent naming → Easier for AI to find files
- Date stamps → Track versions over time
- Descriptive names → Know what's inside without opening

📖 [Best Practices → Student Manual Part 6](02_student_manual.md#best-practices)

---

## Emergency Commands

**Undo Last Commit** (before pushing):
```bash
git reset --soft HEAD~1
```

**Discard All Changes** (nuclear option):
```bash
git checkout .
```

**See What Changed**:
```bash
git diff
```

**Check Remote Connection**:
```bash
git remote -v
```

📖 [Git Emergency Guide → Student Manual Part 2](02_student_manual.md#git-emergency-commands)

---

## Next Steps After This Session

### Week 1: Consolidate
- [ ] Complete any unfinished labs
- [ ] Set up `.ai/instructions.md` fully
- [ ] Make 1 commit per day (build the habit)

### Week 2-4: Expand
- [ ] If Career Planning: Work through 30-day sprint
- [ ] If Maintenance: Document all major equipment
- [ ] Explore 3-5 new prompts from the library

### Month 2-3: Customize
- [ ] Create your first custom prompt (braindump structuring?)
- [ ] Build a workflow that combines 2-3 prompts
- [ ] Share what you've built (GitHub, blog, friends)

📖 [Long-Term Development → Student Manual Part 6](02_student_manual.md#continuing-your-journey)

---

## Community & Support

**Official Resources**:
- Project Repo: https://github.com/danbrickey/pay_no_attention
- Issue Tracker: https://github.com/danbrickey/pay_no_attention/issues

**Get Help**:
1. Check [Student Manual](02_student_manual.md) troubleshooting sections
2. Check [Instructor Guide](01_instructor_guide.md) for common pitfalls
3. Search existing GitHub issues
4. Open new issue with details

**Share Your Success**:
- Created something cool? Open a discussion!
- Found a bug? Report it!
- Improved a prompt? Submit a pull request!

📖 [Additional Resources → Student Manual Part 6](02_student_manual.md#additional-resources)

---

## Mnemonics & Memory Aids

**CACP** - Git Workflow
- **C**lone → **A**dd → **C**ommit → **P**ush

**3 M's** - Maintenance Workflow
- **M**anual/Photos → **M**aintenance Doc → **M**aster Schedule

**DISC** - Finding Prompts
- **D**iscover (search) → **I**nspect (read) → **S**elect (choose) → **C**all (@prompt)

**CVARS** - Career Planning
- **C**V first → **V**alidate current skills → **A**nalyze paths → **R**oadmap → **S**print

---

## Print & Laminate This Section

### Daily Workflow Card

**Morning** (Start of Work):
```bash
git pull              # Get latest
git status            # Check state
```

**During Work**:
- Use `@nav` or `@discover` to find prompts
- Create documents in `docs/` folder
- Use specialized prompts for structured work

**Evening** (End of Work):
```bash
git status            # See what changed
git add .             # Stage changes
git commit -m "What I did today"
git push              # Backup to GitHub
```

**Weekly**:
- Review `.ai/instructions.md` - still accurate?
- Explore 1-2 new prompts
- Clean up `docs/` folder (organize)

---

**Last Updated**: 2025-10-25
**Version**: 1.0.0
**Full Manual**: [02_student_manual.md](02_student_manual.md)
**Instructor Guide**: [01_instructor_guide.md](01_instructor_guide.md)
