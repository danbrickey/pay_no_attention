# Student Manual: Getting Started with pay_no_attention

**Duration**: 120 minutes
**Your Learning Goals**: Set up AI executive assistant, complete 3 hands-on labs

---

## Welcome

Welcome to *pay_no_attention* - your personal AI executive assistant system! This isn't just another collection of ChatGPT prompts. It's a complete framework for offloading mental overhead to AI so you can focus on what matters.

The name comes from philosopher Alfred North Whitehead, who observed that **"Civilization advances by extending the number of important operations which we can perform without thinking about them."** That's exactly what we're building today - systems that handle complexity automatically so you can stop thinking about *how* to get things done and just *do* them.

---

## What You'll Learn

By the end of this session, you'll be able to:
1. ✅ Set up VS Code, GitHub, and your own copy of this project
2. ✅ Configure the AI with your personal context (career goals, preferences, background)
3. ✅ Use structured prompts to accomplish complex tasks
4. ✅ Create a comprehensive career CV and transition plan
5. ✅ Document equipment maintenance and generate automated schedules

---

## How to Use This Manual

- 📖 **During the session**: Follow along with demonstrations, refer to step-by-step instructions
- 🔍 **After the session**: Use as reference for completing exercises or revisiting concepts
- 🔗 **Links**: File paths and prompts to find in your repository
- ⚡ **Quick Reference**: Use the companion Quick Reference guide for day-to-day use

---

# Part 1: Understanding the System

## The Philosophy

### Why "pay_no_attention"?

Whitehead's insight was profound: the best systems are the ones you *don't have to think about*. You don't think about how to drive a car (once you've learned) - you just drive. You don't think about how to type - you just type.

This project applies that principle to knowledge work:
- ❌ **Before**: "How do I organize my career plan? What structure should I use? Where do I save it?"
- ✅ **After**: "AI, create my career plan" → Done, structured, saved in the right place

### AI as Executive Assistant vs. Chatbot

**Traditional AI chatbot use**:
- You ask a question
- AI answers
- Context forgotten
- Repeat tomorrow

**AI Executive Assistant** (this project):
- AI knows your goals, preferences, and context (stored in `.ai/instructions.md`)
- Structured prompts guide AI to produce *exactly* what you need
- Outputs saved in organized documentation system
- AI remembers past work and builds on it

**Example**:

*Chatbot approach*:
```
You: "Help me find a gift for my sister"
AI: "What does she like?"
You: "Yoga and wellness"
AI: [suggests generic gifts]
Next day: Same conversation from scratch
```

*Executive Assistant approach*:
```
You: @giftfinder Sarah
AI: [Loads Sarah's profile from docs/gift-profiles/family/Sarah-Martinez.md]
    - Knows: Vegan, small apartment, loves yoga, wellness focus
    - Remembers: Gave her yoga mat last year (won't duplicate)
    - Searches: Finds perfect space-saving meditation cushion
    - Updates: Adds to gift history automatically
```

---

## The 93-Prompt Library

You're getting access to **93 ready-to-use prompts + 3 reusable templates**, organized into:

### Meta & Navigation (10 prompts)
- **@bootstrap** 🚀: ONE-TIME setup wizard (we'll use today!)
- **@nav** 🧭: Routes you to the right prompt for any task
- **@discover** 🔍: Interactive exploration of what's available
- **@meta-librarian** ⭐: Create new custom prompts
- Quick Start Guide, patterns, agentic development resources

### Architecture Experts (6 ready + 3 templates)
- **@cloud**: AWS/Azure/GCP architecture
- **@api**: REST/GraphQL/gRPC design
- **@security**: Zero-trust, compliance, threat modeling
- **@architect**: Data architecture (Data Vault, dimensional modeling)
- **@drawio**: Create technical diagrams
- Templates for creating your own architecture experts

### Documentation (4 prompts)
- **@arcdoc**: Architecture documentation
- **@projdoc**: Project documentation
- **@bizrules**: Business rules extraction
- **@meeting**: Meeting notes → action items

### Career Development (60 prompts!)
- Career paths across 6 industries:
  - AI/Tech (16 paths): ML Engineer, Prompt Engineer, AI Product Manager...
  - Traditional Tech (8): Full Stack, DevOps, Cloud Architect...
  - Business (7): Product Manager, Business Analyst...
  - Creative (9): UX Designer, Content Writer, Video Editor...
  - Healthcare (4): Nurse Practitioner, Healthcare Admin...
  - Finance/Sales (5): Financial Analyst, Sales Engineer...
  - Vocational (11): Electrician, Help Desk, Paralegal...
- **@career-analyzer**: Gap analysis and roadmaps (using today!)
- **career-cv-interviewer**: Build comprehensive CV (using today!)
- Resume builder, job search strategist

### Workflows (5 multi-step processes)
- Slide deck creation (4-step)
- **Career transition** (4-step): Analysis → Assessment → Resume → Job Search
- More workflows to explore

### Specialized (2 prompts)
- **@tutor**: Personalized learning assistant
- **@coach**: Create training sessions (THIS session was created with it!)

### Development, Strategy, Utilities (11 prompts)
- Code assistance, vendor evaluation
- **@equipment-doc**: Document maintenance (using today!)
- **@maintenance-planner**: Master maintenance schedule (using today!)
- **@giftfinder**: Gift shopping system (optional exercise)
- Excel automation, productivity tools

---

## Directory Structure

Understanding where things live:

```
pay_no_attention/
│
├── .ai/                           ← YOUR PERSONAL CONFIGURATION
│   ├── instructions.md            ← AI reads this to know about YOU
│   ├── context.md                 ← Project-specific notes
│   └── instructions.TEMPLATE.md   ← Example to reference
│
├── ai-resources/
│   └── prompts/                   ← THE 93-PROMPT LIBRARY
│       ├── README.md              ← Master catalog (read this!)
│       ├── QUICK_START.md         ← Persona-based quick start
│       ├── meta/                  ← @bootstrap, @nav, @discover, etc.
│       ├── architecture/          ← Architecture experts + templates
│       ├── career/                ← 60 career path guides
│       ├── documentation/         ← Doc generation prompts
│       ├── workflows/             ← Multi-step processes
│       ├── specialized/           ← @tutor, @coach
│       └── utilities/             ← @equipment-doc, @giftfinder, etc.
│
└── docs/                          ← YOUR DOCUMENTATION
    ├── career/                    ← Career plans, CVs go here
    ├── maintenance/
    │   ├── vital_info/            ← Equipment docs go here
    │   ├── source_manuals/        ← PDF manuals storage
    │   └── master_file.md         ← Generated master schedule
    └── gift-profiles/             ← Gift recipient profiles
```

---

# Part 2: Foundation Setup (Module 1)

## What is VS Code?

**Visual Studio Code (VS Code)** is a code editor that AI assistants *love* because they can see your entire project at once. Think of it as Microsoft Word designed for code and structured documents.

**Why we use it**:
- AI can read/write/edit files across your whole project
- Built-in terminal for running commands
- Extensions for AI assistants (Claude Code, GitHub Copilot, etc.)
- Syntax highlighting makes markdown and code readable

## What is GitHub?

**GitHub** is version control and cloud storage for code/documents.

**Why we use it**:
- **Version control**: Every change tracked, can undo anything
- **Cloud backup**: Your work is safe even if laptop dies
- **Collaboration**: Share with others or keep private
- **History**: See what changed when and why

**Key concepts**:
- **Repository (repo)**: A project folder
- **Clone**: Copy a repo to your computer
- **Commit**: Save a checkpoint
- **Push**: Upload changes to cloud
- **Pull**: Download updates from cloud

---

## Step-by-Step Setup

### Step 1: Install VS Code

**Mac**:
1. Go to https://code.visualstudio.com
2. Click "Download for Mac"
3. Open downloaded file, drag VS Code to Applications
4. Launch VS Code from Applications

**Windows**:
1. Go to https://code.visualstudio.com
2. Click "Download for Windows"
3. Run installer (VSCodeSetup.exe)
4. Follow prompts, check "Add to PATH"
5. Launch VS Code from Start menu

**What success looks like**: VS Code opens, you see welcome screen

---

### Step 2: Create GitHub Account

1. Navigate to https://github.com
2. Click "Sign up"
3. Enter email, create password, choose username
4. Verify email address (check inbox)
5. Select "Free" plan
6. Complete quick survey (optional)

**What success looks like**: Logged into GitHub, see dashboard

---

### Step 3: Install Git (Command-Line Tool)

**Mac**:
1. Open Terminal (Applications → Utilities → Terminal)
2. Type: `git --version`
3. If not installed, Mac will prompt to install Xcode Command Line Tools
4. Click "Install" and wait

**Windows**:
1. Go to https://git-scm.com/download/win
2. Download and run installer
3. Use default settings (click "Next" through all)
4. Finish installation

**Verify**:
- Open VS Code
- Open Terminal: Menu → Terminal → New Terminal
- Type: `git --version`
- Should see version number (e.g., "git version 2.39.0")

---

### Step 4: Clone the Repository

**What you're doing**: Copying the pay_no_attention project to your computer

**Steps**:

1. **Open VS Code**

2. **Open Terminal** (Menu → Terminal → New Terminal)

3. **Navigate to where you want the project**:
   ```bash
   # Mac/Linux:
   cd ~/Documents

   # Windows:
   cd C:\Users\YourName\Documents
   ```

4. **Clone the repository**:
   ```bash
   git clone https://github.com/danbrickey/pay_no_attention.git
   ```

5. **Open the project folder**:
   - Menu → File → Open Folder
   - Navigate to `pay_no_attention` folder
   - Click "Open"

**What success looks like**:
- VS Code file explorer shows pay_no_attention folder structure
- You see: .ai/, ai-resources/, docs/ folders

---

### Step 5: Create Your Own Repository

**Why**: You want your own copy to customize and save your work

**Option A: Create New Repo (Recommended for this class)**

1. **On GitHub.com**:
   - Click green "New" button (or go to https://github.com/new)
   - Repository name: `my-ai-assistant` (or your choice)
   - Description: "My personal AI executive assistant"
   - Choose: **Private** (recommended)
   - Do NOT initialize with README
   - Click "Create repository"

2. **Copy files to your new repo**:
   ```bash
   # In terminal, navigate to your Documents folder
   cd ~/Documents  # or C:\Users\YourName\Documents on Windows

   # Create new folder for YOUR repo
   mkdir my-ai-assistant
   cd my-ai-assistant

   # Initialize git
   git init

   # Copy files from cloned repo (excluding .git folder)
   # Mac/Linux:
   cp -r ../pay_no_attention/* .
   cp -r ../pay_no_attention/.ai .

   # Windows (use File Explorer):
   # Copy everything from pay_no_attention folder EXCEPT .git folder
   # Paste into my-ai-assistant folder
   # Don't forget to copy .ai folder (it's hidden - enable "Show hidden files")

   # Add GitHub remote (use YOUR repository URL)
   git remote add origin https://github.com/YOUR-USERNAME/my-ai-assistant.git

   # Make first commit
   git add .
   git commit -m "Initial setup: Clone pay_no_attention project"
   git push -u origin main
   ```

**Option B: Fork (Alternative)**

1. Go to https://github.com/danbrickey/pay_no_attention
2. Click "Fork" button (top right)
3. Choose your account
4. Rename if desired
5. Click "Create fork"
6. Clone YOUR fork:
   ```bash
   git clone https://github.com/YOUR-USERNAME/pay_no_attention.git
   ```

**What success looks like**:
- You have a folder with all the files
- Running `git remote -v` shows YOUR GitHub repository
- Your repository appears on your GitHub profile

---

### Step 6: Install AI Assistant Extension

**For Claude Code** (if you have Claude Pro/API):
1. In VS Code, click Extensions icon (left sidebar, square icon)
2. Search "Claude Code"
3. Click "Install"
4. Follow prompts to authenticate

**For GitHub Copilot** (if you have GitHub Pro):
1. Extensions → Search "GitHub Copilot"
2. Install
3. Sign in with GitHub account

**For this class**: Instructor will specify which AI assistant to use

**What success looks like**: AI assistant icon appears in VS Code sidebar

---

## Practice Exercise

**Try this**:
1. In VS Code, navigate to `ai-resources/prompts/README.md`
2. Click to open the file
3. Read the first section
4. Find the mnemonic table
5. Click on a link (e.g., @bootstrap) - it should open that prompt file

**You're ready when**: You can navigate the folder structure and open files

---

# Part 3: Bootstrap Your Personal Assistant (Lab 1)

## What is Bootstrapping?

**Bootstrap** = The one-time setup wizard that customizes the entire system for YOU

**What it does**:
1. Interviews you about your background, goals, preferences
2. Creates personalized `.ai/instructions.md` file
3. Proposes documentation folder structure
4. Gives you a personalized tour of relevant prompts

**Think of it like**: Setting up a new phone - you only do it once, but it makes everything else work better

---

## Why This Matters

`.ai/instructions.md` is the persistent memory for ALL AI interactions in this project.

**Without it**:
```
You: "Help me with my career plan"
AI: "What's your background?"
You: [Explains everything from scratch]
```

**With it**:
```
You: "Help me with my career plan"
AI: [Reads .ai/instructions.md]
    "Given your 5 years as a Project Manager and your goal to transition
    to AI Product Management, let's focus on..."
```

---

## Step-by-Step: Bootstrap Interview

### Preparation

**Before starting**:
- Set aside 15-20 minutes uninterrupted
- Think about:
  - Your current role and experience
  - Your career goals (even if vague)
  - How you prefer to learn (hands-on, theory, visual, etc.)
  - What you want this AI assistant to help with

---

### Phase 1: Initiate Bootstrap

1. **Open AI Assistant** in VS Code (Claude Code, Copilot, etc.)

2. **Type**: `@bootstrap`

3. **AI welcomes you** and asks:
   - "Have you copied the `ai-resources/` folder into your project?"
   - Answer: **Yes** (you cloned the whole repo)

4. **AI asks**: "Are you setting up a brand new project or updating an existing one?"
   - Answer: **New**

5. **AI confirms** what it found and explains the process

---

### Phase 2: Personal Context Interview

The AI will ask you **7 groups of questions**. Answer honestly - you can update this anytime!

#### Group 1: Professional Identity

**Questions you'll get**:
1. What's your current role or title?
2. How many years of professional experience do you have?
3. What are your primary day-to-day responsibilities?
4. [Optional] What company or organization do you work for?

**Example answers**:
- Role: "Product Manager at a fintech startup"
- Experience: "5 years"
- Responsibilities: "Roadmap planning, user research, working with engineering teams"
- Company: "Skip" or "Acme Financial Services"

---

#### Group 2: Focus Areas

**Question**: Which domains are most relevant to your work?

**Checklist** (select all that apply):
- [ ] Software Development (Frontend, Backend, Full-stack)
- [ ] Data Engineering / Data Science / Analytics
- [ ] Cloud Architecture (AWS, Azure, GCP)
- [ ] DevOps / Site Reliability / Platform Engineering
- [ ] Product Management / Product Design
- [ ] Business Analysis / Strategy
- [ ] Project Management / Agile Coaching
- [ ] UI/UX Design
- [ ] Security / Compliance
- [ ] Marketing / Content Creation
- [ ] Career Development / Job Searching
- [ ] Teaching / Tutoring
- [ ] Other: ___________

**Example**: Check "Product Management" and "Career Development"

---

#### Group 3: Technical Stack

**If applicable**, list your tools:
- **Languages**: Python, JavaScript, SQL, etc.
- **Frameworks**: React, Django, etc.
- **Platforms**: AWS, Salesforce, etc.
- **Tools**: Git, Jira, Figma, etc.

**If not applicable**: Just say "N/A" or "Non-technical role"

**Example**:
- Languages: "SQL for data analysis, learning Python"
- Platforms: "Jira, Miro, Amplitude"
- Tools: "Figma, Notion, Google Analytics"

---

#### Group 4: Career Goals

**Questions**:
- Short-term (3-6 months): What do you want to accomplish?
- Medium-term (1-2 years): Where do you want to be?
- Long-term (3-5+ years): What's the vision?

**Example**:
- Short: "Get promoted to Senior PM, learn Python basics"
- Medium: "Transition to AI Product Management"
- Long: "Director of Product, leading AI product teams"

---

#### Group 5: How You'll Use This Library

**Select all that apply**:
- [ ] Career planning and job search
- [ ] Resume and cover letter writing
- [ ] Learning new technical skills
- [ ] Code reviews and programming help
- [ ] Architecture design and documentation
- [ ] Project planning and organization
- [ ] Personal productivity and time management
- [ ] Creative projects (presentations, content, gifts)
- [ ] Home/equipment maintenance tracking
- [ ] Other: ___________

**Example**: Check "Career planning," "Learning new skills," "Productivity"

---

#### Group 6: Preferences

**Communication style**: How should AI communicate with you?
- Direct and concise
- Detailed explanations
- Conversational
- Mix of all

**Learning style**: How do you learn best?
- Hands-on examples
- Theory first, then practice
- Visual diagrams
- Mix of all

**Documentation preference**: What format do you prefer?
- Detailed docs
- Quick reference
- Step-by-step tutorials
- Mix of all

**Example**: "Conversational," "Hands-on examples," "Quick reference with links to details"

---

#### Group 7: Industry Context (Optional)

**If applicable**:
- Industry: Healthcare, Finance, E-commerce, Education, etc.
- Compliance: HIPAA, GDPR, SOX, PCI-DSS, etc.
- Domain expertise: Clinical trials, Trading systems, etc.

**You can skip this** if not relevant

---

### Phase 3: Review Your Configuration

**AI generates your `.ai/instructions.md`** based on the interview.

**What it includes**:
```markdown
# Personal AI Assistant - Configuration

## Your Professional Context

### Current Role & Background
- **Your Role**: Product Manager
- **Years of Experience**: 5 years
- **Primary Responsibilities**: Roadmap planning, user research...

### Your Focus Areas
- [x] Product Management / Product Design
- [x] Career Development / Job Searching
- [ ] Software Development
...

### Your Career Goals
- Short-term (3-6 months): Get promoted to Senior PM, learn Python basics
- Medium-term (1-2 years): Transition to AI Product Management
- Long-term (3-5 years): Director of Product, leading AI teams

## How You Want to Use This AI Assistant

### Primary Use Cases
- [x] Career planning and job search
- [x] Learning new technical skills
- [x] Personal productivity and time management

### Your Preferences
- **Communication Style**: Conversational
- **Learning Style**: Hands-on examples
- **Documentation Preferences**: Quick reference with links to details

---

## Quick Start with Prompts

Top prompts based on your focus areas:
- **@career-analyzer** - Career path analysis and gap analysis
- **Career Transition Workflow** - 4-step process from analysis to job offer
- **@tutor** - Learn Python, product skills, or any topic
- **@cloud** - Learn cloud architecture (relevant for PM work)
- **@coach** - Create learning sessions for yourself or team

See full navigation:
- **@nav** - Intelligent routing to right prompts
- **@discover** - Interactive prompt exploration
```

**AI asks**: "Would you like me to save this to `.ai/instructions.md`?"

**You say**: "Yes!"

---

### Phase 4: Documentation Structure

**AI proposes** a folder structure based on your goals:

```
docs/
├── README.md
├── career/                   # Your career planning
│   ├── cv.json              # Comprehensive CV
│   └── career_plan.md       # Career roadmap
├── learning/                # Learning notes, courses
└── projects/                # Project documentation
```

**AI asks**: "Should I create this structure?"

**You can**:
- Say "Yes" (recommended)
- Say "Customize" and specify changes
- Say "No" (do it manually later)

---

### Completion

**AI provides**:
- ✅ Personalized tour of top 5 prompts for YOU
- ✅ Suggested first actions
- ✅ Quick reference card

**You now have**:
- ✅ `.ai/instructions.md` customized for you
- ✅ Folder structure for your work
- ✅ AI that knows your context for all future interactions

---

## Common Questions

**Q: Can I change my .ai/instructions.md later?**
A: Yes! Edit it anytime. The AI will use whatever is in the file.

**Q: What if I don't know the answer to a question?**
A: Say "I don't know" or "Skip" - the file can have gaps.

**Q: Should I be specific or general?**
A: More specific = better AI responses, but general works too. Start simple, add detail as you learn what's useful.

**Q: Is this information private?**
A: It stays on your computer and in your private repo (if you made it private). The AI reads it but doesn't share it.

---

# Part 4: Career Planning with AI (Lab 2)

## Overview

In this lab, you'll:
1. Create a comprehensive, structured CV
2. Analyze your career path and identify gaps
3. Generate a detailed career transition plan with specific steps

**Why structured CV?**: A rich, detailed CV can be transformed into ANY format (resume, LinkedIn, portfolio). You create it once, use it forever.

---

## Part A: Build Your CV (12 minutes)

### What is career-cv-interviewer.md?

This prompt conducts a systematic interview to extract your complete career history and creates a **JSON-formatted CV** optimized for AI processing.

**Output**: A comprehensive CV with:
- Professional identity & contact info
- Career history with detailed roles, projects, impacts
- Skills matrix (technical + soft skills with proficiency levels)
- Education & certifications
- AI readiness profile (for career transitions)

---

### Quick Path (If Pressed for Time)

**If you already have a resume**:

1. Open AI assistant in VS Code
2. Upload your existing resume
3. Say: "Use career-cv-interviewer.md to convert this to a structured CV"
4. AI will extract information and format as JSON
5. Review and fill in gaps
6. Save to `docs/career/cv.json`

**Estimated time**: 5-7 minutes

---

### Full Interview Path (For Complete CV)

**If you want a thorough CV or don't have a resume**:

1. **Open career-cv-interviewer.md**:
   - Navigate to `ai-resources/prompts/career/career-cv-interviewer.md`
   - Read the prompt (optional, to understand what's coming)

2. **Start the interview**:
   - In AI chat: Type or reference the career-cv-interviewer prompt
   - AI begins 6-phase systematic interview

3. **Phase 1: Story Opening** (2 min)
   - AI asks about your career arc
   - Share your narrative in your own words

4. **Phase 2: Role Deep Dive** (6-8 min)
   - For each significant role, AI asks:
     - Context & scope (what was your mandate?)
     - Technical environment (tools, stack)
     - Impact & outcomes (measurable results)
     - AI/ML connections (any exposure?)
   - Specific projects and achievements

5. **Phase 3: Skills Inventory** (3 min)
   - AI builds skills matrix collaboratively
   - Confirms proficiency levels
   - Captures soft skills with examples

6. **Phase 4: Education & Learning** (2 min)
   - Formal degrees
   - Certifications
   - Recent learning
   - Thought leadership

7. **Phase 5: AI Transition Vision** (2 min)
   - What AI capabilities do you want?
   - Target roles
   - Timeline

8. **Phase 6: Validation** (1 min)
   - AI summarizes key highlights
   - You fill in any gaps

9. **Save your CV**:
   - AI generates JSON-formatted CV
   - Copy to `docs/career/cv.json`
   - Or save as `docs/career/cv.md` if you prefer markdown

**Estimated time**: 15-20 minutes (can finish outside class if needed)

---

### Example CV Output (Excerpt)

```json
{
  "professional_identity": {
    "name": "Jane Smith",
    "professional_tagline": "Product Manager transitioning to AI/ML product leadership",
    "career_narrative_summary": "5 years building B2B SaaS products, passionate about leveraging AI to solve complex user problems. Seeking to combine product management expertise with AI/ML technical capabilities."
  },

  "ai_readiness_profile": {
    "transition_vision": "Become an AI Product Manager leading ML-powered features",
    "target_roles": ["AI Product Manager", "ML Product Lead"],
    "current_ai_capabilities": [
      {
        "capability": "Data analysis for product insights",
        "proficiency": "Intermediate",
        "evidence": "Used SQL and Python for user behavior analysis"
      }
    ],
    "identified_skill_gaps": [
      "ML fundamentals and algorithms",
      "Python for ML (pandas, scikit-learn)",
      "Model evaluation and metrics"
    ]
  },

  "career_history": [
    {
      "title": "Product Manager",
      "company": "Acme SaaS Inc.",
      "dates": {"start": "2020-01", "end": "present"},
      "quantifiable_impact": [
        {
          "metric": "User retention",
          "value": "Increased from 68% to 84%",
          "context": "Through data-driven feature prioritization"
        }
      ]
    }
  ],
  ...
}
```

---

## Part B: Career Analysis & Gap Analysis (15 minutes)

### What is career-analyzer.md?

This prompt takes your CV and:
- Scores your fit for target roles (with % match breakdown)
- Identifies specific skill/experience gaps
- Creates phased learning roadmap with exact courses, costs, timelines
- Recommends 2-3 AI career paths with detailed analysis
- Generates actionable career plan document

---

### Step-by-Step Process

**1. Load Career Analyzer** (1 min)

- Navigate to `ai-resources/prompts/career/career-analyzer.md`
- In AI chat: Reference or type `@career-analyzer`
- AI introduces itself and asks for your CV

**2. Provide Your CV** (1 min)

Option A: If you have cv.json file:
- Upload or reference: `docs/career/cv.json`

Option B: If you have existing resume:
- Upload your resume
- AI will work with that (less detailed analysis)

Option C: Verbal description:
- Describe your background briefly
- AI will ask clarifying questions

**3. Specify Your Target** (2 min)

Tell the AI what you're aiming for:

Option 1 - Specific transition:
- "I want to transition to AI Product Manager"
- "Analyze my fit for Machine Learning Engineer roles"

Option 2 - General exploration:
- "What AI career paths fit my background?"
- "I'm interested in AI but don't know which direction"

Option 3 - Specific job posting:
- Paste a job description you're interested in
- AI will analyze fit for THAT specific role

**4. Receive Comprehensive Analysis** (10 min)

AI generates detailed analysis including:

**Match Score Breakdown**:
```
Overall Fit: 72%
- Technical Skills: 65%
- Experience Level: 80%
- Education/Certifications: 70%
- Soft Skills/Leadership: 85%
- Domain Knowledge: 60%
```

**Gap Analysis** (for each gap):
```
Gap 1: Python for Machine Learning
- Importance: Critical
- Current Level: Beginner (basic Python only)
- Target Level: Proficient (pandas, scikit-learn, model evaluation)
- How to Close:
  • Course: "Python for Data Science" by IBM (Coursera)
    - Duration: 25 hours over 5 weeks
    - Cost: $49 (or free audit)
    - Timeline: Months 1-2
  • Project: Build 3 ML models for portfolio
    - Time: 30 hours
    - Timeline: Month 3
```

**Career Path Recommendations** (2-3 paths with full roadmaps):

Each path includes:
- Current fit assessment (X/100)
- Why this path matches your strengths
- Complete gap analysis
- **Phased timeline** with specific months/quarters:
  - Phase 1: Foundation (Months 1-3)
  - Phase 2: Skill Development (Months 4-6 or 4-9)
  - Phase 3: Job-Ready Preparation (Months 7-12)
- **Specific learning resources** (exact course names, links, costs)
- **Portfolio project ideas** (what to build)
- **Entry strategy** (how to get first role)
- **Market outlook & salary ranges**

**5. Save Your Career Plan** (1 min)

- AI generates complete career plan document
- Save to: `docs/career/career_plan.md`
- AI will format with proper versioning

---

### Example Career Plan Excerpt

```markdown
# AI Career Transition Plan - Jane Smith

**Date**: 2025-10-25
**Planning Horizon**: 12 months
**Target Career Path**: AI Product Manager
**Current Fit**: 72/100

---

## Executive Summary

You're well-positioned for AI Product Management with strong product fundamentals, data analysis experience, and stakeholder communication skills. Primary gaps are ML technical knowledge and hands-on AI project experience.

**Recommended Path**: AI Product Manager (72% fit)
**Timeline**: 6-9 months to job-ready
**Investment**: $200-400 + 10-15 hours/week

---

## Phase 1: Foundation (Months 1-3)

### Week 1-4: ML Fundamentals
- [ ] Course: "Machine Learning" by Andrew Ng (Coursera)
  - Time: 60 hours (5 hours/week for 12 weeks - start now)
  - Cost: $49/month or free audit
  - Focus: Understand ML concepts, algorithms, evaluation metrics

### Week 5-8: Python for ML
- [ ] Course: "Python for Data Science" (Coursera)
  - Time: 25 hours
  - Cost: $49
  - Master: pandas, numpy, scikit-learn basics

### Week 9-12: First AI Project
- [ ] Project: Customer Churn Prediction Model
  - Time: 20-30 hours
  - Tech: Python, pandas, scikit-learn, Jupyter
  - Outcome: End-to-end ML project for portfolio

**Phase 1 Totals**: 110-120 hours (10 hours/week), ~$100

---

## Phase 2: Skill Development (Months 4-6)

### Month 4-5: Advanced ML & AI Product Skills
- [ ] Course: "AI Product Management" (Product School)
  - Time: 30 hours
  - Cost: $299
  - Learn: AI feature design, model evaluation, ROI analysis

### Month 5-6: Second Portfolio Project
- [ ] Project: Recommendation System for E-commerce
  - More complex than Phase 1
  - Demonstrates product thinking + technical skill

...
```

---

### What to Do With This Plan

**Immediately**:
- Read through Phase 1 recommendations
- Bookmark or save the exact courses mentioned
- Add Phase 1 tasks to your calendar

**Ongoing**:
- Check off completed items
- Update the plan as you progress
- Use as reference during job interviews ("Here's my structured learning plan")

**In 3-6 months**:
- Revisit with AI for progress check
- Update with new skills gained
- Adjust timeline based on actual pace

---

## Common Questions

**Q: This seems like a lot - do I have to do everything?**
A: No! Focus on Phase 1 first. The plan is comprehensive so you have options. Prioritize what fits your timeline.

**Q: What if I can't afford the courses?**
A: Many are free to audit. AI will include free alternatives. You can also ask: "Show me free-only options"

**Q: Can I change target roles later?**
A: Yes! Run career-analyzer again anytime. Your CV is reusable for any analysis.

**Q: What if the timeline seems too long/short?**
A: The plan adapts to your pace. AI assumes part-time study while working. Adjust based on your availability.

---

# Part 5: Maintenance Documentation (Lab 3)

## Overview

In this lab, you'll:
1. Document 1-2 pieces of equipment (car, appliance, tool)
2. Generate maintenance schedules with climate-specific timing
3. (If time) Create master household maintenance plan

**The power**: Take a photo or upload a manual → Get complete maintenance guide with part numbers, costs, local service providers, and optimized calendar.

---

## Part A: Document Equipment (15 minutes)

### What is equipment-maintenance-documenter.md?

This prompt creates comprehensive maintenance documentation from:
- Photos of equipment (extracts brand/model from image)
- PDF manuals (mines for schedules and specs)
- Verbal descriptions ("I have a 2020 Honda Civic")

**Output**: Detailed maintenance guide with:
- Maintenance schedule (frequencies, seasonal timing)
- Step-by-step procedures
- Exact part numbers and materials specs
- Local service providers (if you provide location)
- Climate-specific adjustments (if you provide location)

---

### Choose Your Equipment

**For this lab, pick 1-2 items**:

**Easy (Recommended)**:
- ✅ Your car/vehicle (well-documented, everyone has one)
- ✅ HVAC system (check thermostat or furnace)
- ✅ Refrigerator or other appliance

**Medium**:
- Lawn mower, snow blower
- Water heater
- Washer/dryer

**Advanced**:
- Power tools (chainsaw, drill, etc.)
- Specialized equipment
- Vintage/rare items

**Have ready**:
- Photos showing brand/model (take now if needed)
- OR manual PDF (check manufacturer website if you don't have)
- OR just description and we'll research

---

### Step-by-Step Process

**1. Load Equipment Documenter** (1 min)

- Navigate to: `ai-resources/prompts/utilities/equipment-maintenance-documenter.md`
- In AI chat: Type `@equipment-doc` or reference the prompt

**2. Provide Equipment Information** (3 min)

**Option A - Photo**:
- Take/upload photo showing model plate or identifying features
- AI will analyze and extract brand, model, specs

**Option B - PDF Manual**:
- Upload equipment manual PDF
- AI will mine for maintenance schedules, part numbers, procedures

**Option C - Description**:
- Describe: "2020 Honda Civic, 45,000 miles"
- AI will ask clarifying questions and research

**3. Answer Context Questions** (2 min)

AI will ask:

**Location** (optional but valuable):
- City, State or ZIP code
- Why: AI adjusts maintenance timing for YOUR climate
- Example: "Chicago, IL" → AI knows harsh winters affect car maintenance

**Ownership Status**:
- Owner, Renter, Property Manager
- Why: Affects responsibilities (renters don't service HVAC compressor)
- Example: "Renter" → AI marks what's landlord's job vs. yours

**4. Receive Documentation** (5 min)

AI generates comprehensive guide, for example:

```markdown
# Equipment Documentation: 2020 Honda Civic

## Equipment Overview
- **Category**: Vehicle
- **Brand**: Honda
- **Model**: Civic (10th Gen, LX trim)
- **Year**: 2020
- **Identified From**: User description + online research
- **Key Features**: 2.0L 4-cylinder, CVT transmission, 158 HP
- **Ownership Context**: Owner

---

## Documentation Resources
- **Official Manual**: [Honda Civic 2020 Owner's Manual PDF](https://owners.honda.com/)
- **Customer Support**: 1-800-999-1009
- **Warranty**: 3yr/36,000mi basic, 5yr/60,000mi powertrain (check if still covered)
- **Maintenance Schedule**: [Honda Maintenance Minder](https://owners.honda.com/servicemaintenance/minder)

---

## Location Analysis
- **Location**: Chicago, IL 60601
- **Climate Zone**: USDA Zone 6a, Humid Continental
- **Temperature Range**: -5°F winter to 90°F summer
- **Seasonal Factors**: Harsh winters with road salt, humid summers
- **Regional Considerations**:
  - Road salt = rust prevention critical
  - Cold starts = battery health important
  - Potholes = suspension/tire monitoring

**Maintenance Impact**:
- Oil changes: Synthetic oil recommended for winter cold starts
- Undercarriage wash: Critical after winter road salt exposure
- Tire pressure: Check weekly in winter (pressure drops in cold)
- Battery: Test before winter; cold reduces capacity

---

## Maintenance Schedule

| Task | Frequency | Best Timing | Climate Notes | Cost |
|------|-----------|-------------|---------------|------|
| Oil change | Every 5,000 mi | Any season | Synthetic 0W-20 for Chicago winters | $45-70 |
| Tire rotation | Every 7,500 mi | Spring & Fall | Check pressure weekly in winter | $25-40 |
| Cabin air filter | Annually | Spring | High pollen area - may need 2x/year | $15-25 (DIY) |
| Engine air filter | Every 30,000 mi | Spring or Fall | More frequent if dusty environment | $20-35 (DIY) |
| Brake inspection | Every 10,000 mi | Any season | Salt exposure = corrosion risk | $Free (with oil change) |
| Battery test | Annually | October | Cold kills weak batteries | Free (at parts store) |
| Undercarriage wash | Weekly in winter | Jan-Mar | Remove road salt ASAP | $10-15/wash |
| Coolant flush | Every 60,000 mi | Fall | Prevent freezing damage | $100-150 |

---

## Detailed Procedures

### Oil Change (DIY or Professional)

**Frequency**: Every 5,000 miles or 6 months
**Best Time**: Any season (watch for extreme cold - harder DIY)
**Duration**: 30 min (DIY), 45 min (shop wait)
**Difficulty**: Easy (if you have tools), or Professional
**Responsibility**: Owner

**Climate Considerations**:
- Chicago winters: Use 0W-20 synthetic (better cold flow than conventional)
- Don't drain oil when engine is cold - harder to drain fully

**Materials Needed**:
- Oil: 3.7 quarts 0W-20 synthetic
  - **Recommended**: Honda Genuine 0W-20 (Part #08798-9036)
  - **Alternatives**: Mobil 1 0W-20, Castrol Edge 0W-20
  - **Cost**: $25-35 for full amount
- Oil filter: Honda Part #15400-PLM-A02
  - **Cost**: $8-12
  - **Where to buy**: AutoZone, O'Reilly, Amazon

**DIY Steps**:
1. Warm engine (5 min drive) - do NOT skip, helps oil drain completely
2. Jack up car, secure with stands (NEVER work under car on jack alone!)
3. Locate drain plug (17mm socket) and oil filter
4. Place drain pan under plug, remove plug, drain oil (10 min)
5. Replace crush washer on drain plug (Part #94109-14000, $1 each)
6. Remove old filter (may need filter wrench), install new
7. Lower car, add 3.7 quarts new oil via filler cap
8. Start engine, check for leaks, shut off
9. Check dipstick - should be between MIN and MAX marks
10. Reset Maintenance Minder on dashboard

**Safety Warnings**:
- Hot oil can burn - let cool slightly before draining
- Never work under car supported only by jack
- Dispose of old oil properly (take to AutoZone/O'Reilly for free recycling)

**Professional Option**:
- **Cost**: $45-70 at quick lube, $60-90 at dealer
- **Tip**: Ask for Honda filter (not generic)

---

### Tire Rotation

[Similar detailed format for every maintenance task...]

---

## Materials & Specifications

| Material/Part | Specification | OEM Part # | Alternatives | Cost | Where to Buy |
|---------------|---------------|------------|--------------|------|--------------|
| Engine Oil | 0W-20 Synthetic | 08798-9036 | Mobil 1 0W-20 | $25-35 | AutoZone, Amazon |
| Oil Filter | — | 15400-PLM-A02 | Fram XG7317 | $8-12 | AutoZone, Amazon |
| Cabin Air Filter | — | 80292-TBA-A11 | FRAM CF12157 | $12-18 | AutoZone, Amazon |
| Engine Air Filter | — | 17220-5AA-A00 | K&N 33-5075 | $15-30 | AutoZone, Amazon |

---

## When to DIY vs. Call a Professional

**Renter Guidance**: N/A (you own your vehicle)

**Owner Guidance**:
- **DIY-Friendly**:
  - Oil changes (if you have tools and space)
  - Air filter replacements
  - Tire pressure checks and top-offs
  - Cabin air filter replacement
  - Windshield wiper replacement
  - Battery terminal cleaning

- **Professional-Required**:
  - Transmission service (CVT fluid change requires dealer equipment)
  - Brake system work (safety-critical)
  - Timing belt replacement (if needed - interference engine)
  - Suspension/steering work
  - Anything triggering check engine light

**Warning Signs Requiring Professional**:
- Check engine light on
- Strange noises (grinding, squealing, knocking)
- Vibrations or pulling while driving
- Fluid leaks under car
- Smoke from engine or exhaust

**Service Providers** (Chicago, IL area):
- **Honda Dealer**: McGrath Honda (downtown) - 3.2 mi
  - Phone: (773) 248-8000
  - Service: Full service, genuine parts, warranty work
  - Cost: Higher ($60-90 oil change) but thorough

- **Independent Mechanics**:
  - Windy City Automotive (Lincoln Park) - 2.5 mi
    - Rating: 4.8/5 stars (Google)
    - Cost: Moderate ($50-70 oil change)

- **Quick Lube Chains**:
  - Jiffy Lube (various locations)
  - Cost: Low ($45-60) but verify Honda filter used

---

## Troubleshooting & Common Issues

### Maintenance Minder System Won't Reset
**Symptoms**: After oil change, "Maint. Req'd" light stays on
**Likely Causes**: Incorrect reset procedure
**DIY Fix**:
1. Turn ignition to ON (don't start engine)
2. Press and hold SELECT/RESET button until oil life % appears
3. Hold SELECT/RESET for 10+ seconds until indicator blinks
4. Release, press briefly again to confirm
**Prevention**: Follow procedure immediately after service

[More common issues...]

---

*Equipment maintenance documentation generated: 2025-10-25*
*For: 2020 Honda Civic, Chicago IL*
*File: docs/maintenance/vital_info/vehicle_sedan_honda_civic_2020.md*
```

**5. Save Documentation** (1 min)

- **Filename**: `vehicle_sedan_honda_civic_2020.md`
- **Location**: `docs/maintenance/vital_info/`
- **Why this matters**: Maintenance planner will scan this folder

---

### Try It Yourself

**Now create your documentation**:

1. Choose your equipment
2. Gather photo/manual/description
3. Use @equipment-doc prompt
4. Answer questions (location helps!)
5. Save to `docs/maintenance/vital_info/`

**Estimated time**: 10-15 minutes per item

---

## Part B: Create Master Maintenance Plan (10 minutes)

### What is household-maintenance-planner.md?

This prompt scans ALL your equipment files and creates:
- **Monthly calendar** with all maintenance tasks
- **Seasonal summaries** with grouped tasks
- **Annual budget** (DIY vs. professional cost estimates)
- **Task grouping recommendations** (do related tasks together)
- **Bulk purchase opportunities** (buy filters in bulk, save money)
- **Service provider directory** (if location provided)

**Think of it as**: Your household maintenance command center

---

### Step-by-Step Process

**1. Load Maintenance Planner** (1 min)

- Navigate to: `ai-resources/prompts/utilities/household-maintenance-planner.md`
- In AI chat: Type `@maintenance-planner` or reference prompt

**2. AI Scans Your Equipment** (automatic, 2 min)

- AI reads all files in `docs/maintenance/vital_info/`
- Extracts: tasks, frequencies, costs, materials, service providers
- Analyzes: overlap, grouping opportunities, seasonal distribution

**3. AI Generates Master Schedule** (5 min)

Creates comprehensive document with:

**Monthly Calendar**:
```markdown
### January

| Date | Task | Equipment | Duration | Cost | Priority | Status |
|------|------|-----------|----------|------|----------|--------|
| Early Jan | Check tire pressure | Honda Civic | 5 min | $0 | High | [ ] |
| Mid Jan | Replace HVAC filter | Home HVAC | 10 min | $15 | High | [ ] |
| Late Jan | Oil change | Honda Civic | 30 min | $60 | Medium | [ ] |

**January Totals**: 3 tasks, 45 minutes, $75

**January Purchase List**:
- [ ] HVAC filter 16x20x1 MERV 11 - Qty: 1 - $15 - Buy at: Home Depot
- [ ] Synthetic oil 0W-20 - Qty: 1 - $30 - Buy at: AutoZone

**January Notes**:
- Best time: Mid-month for HVAC (before Feb cold snap)
- Oil change: Can wait until late Jan or early Feb
```

**Task Grouping Recommendations**:
```markdown
### Recommended Task Groupings

**Group 1: Indoor Filter Changes** (Same day - 25 min total)
- [ ] HVAC filter - 10 min - $15
- [ ] Furnace filter - 5 min - $12
- [ ] Vacuum cleaner filter - 5 min - $8
- [ ] Range hood filter - 5 min - $10

**Best Timing**: Every 3 months (Jan, Apr, Jul, Oct)
**Bulk Purchase**: Buy all 4 filters together quarterly - Save $12/year vs. buying individually
```

**Annual Budget Summary**:
```markdown
## Annual Cost Summary

**Total Annual Maintenance**: $1,200 - $1,800

By Category:
- Vehicle: $450-650 (oil changes, tires, inspections)
- HVAC: $200-400 (filters, annual service)
- Appliances: $150-250 (filters, cleaning)
- Home Systems: $100-200 (gutters, misc)

**Optimization Opportunities**:
1. DIY oil changes: Save $180/year (vs. dealer pricing)
2. Buy filters in bulk: Save $45/year
3. Bundle HVAC service with AC tuneup: Save $75 (one service call)

**Potential Total Savings**: $300/year
```

**4. Save Master File** (1 min)

- Save to: `docs/maintenance/master_file.md`
- This becomes your household maintenance command center

**5. Use Ongoing**

- **Weekly**: Check what's due
- **Monthly**: Review upcoming month, buy materials
- **Quarterly**: Update with actual costs, mark completed tasks

---

## Why This Matters

**Before this system**:
- Forget oil changes until car light comes on
- Don't know when you last changed HVAC filter
- Emergency repair because you missed maintenance
- Buy materials last-minute at high prices

**After this system**:
- See all maintenance in one calendar
- Get reminders for each task
- Group related tasks for efficiency
- Buy materials in bulk, save money
- Prevent emergencies with proactive maintenance

**The Whitehead quote applies**: You no longer think about "when was that last serviced?" - the system handles it. Pay no attention.

---

# Part 6: Wrap-Up & Next Steps

## What You've Built Today

In 2 hours, you've:
1. ✅ Set up VS Code, GitHub, and cloned the repository
2. ✅ Created personalized `.ai/instructions.md` - AI knows your context
3. ✅ Built comprehensive CV (structured JSON or from resume)
4. ✅ Generated career transition plan with specific roadmap
5. ✅ Documented equipment with detailed maintenance guides
6. ✅ (Optionally) Created master household maintenance schedule

**More importantly**: You understand HOW to work with structured prompts and persistent context. This isn't just about the 3 labs we did - it's a new way of working with AI.

---

## The Power of Persistent Context

**Traditional AI use**:
```
Day 1: "Help me with career planning" → [AI helps, forgets]
Day 5: "Help me with career planning" → [Start from scratch]
Day 10: "Help me with career planning" → [Same questions again]
```

**AI Executive Assistant** (what you built):
```
Day 1: "Help me with career planning"
        → AI reads .ai/instructions.md
        → Knows your role, goals, preferences
        → Creates personalized plan, saves to docs/career/

Day 5: "Update my career plan with new certification"
        → AI reads existing plan from docs/career/career_plan.md
        → Knows your context from .ai/instructions.md
        → Updates plan, preserves history

Day 10: "How am I tracking on my career plan?"
         → AI compares plan vs. current date
         → Provides progress report
         → Suggests next steps
```

**The AI remembers and builds on past work**. That's the power.

---

## Your System Overview

### Where Things Live

```
my-ai-assistant/                 ← Your repository
│
├── .ai/
│   └── instructions.md          ← AI reads this EVERY interaction
│
├── ai-resources/
│   └── prompts/                 ← 93 prompts you can use
│
└── docs/                        ← YOUR work
    ├── career/
    │   ├── cv.json              ← Your comprehensive CV
    │   └── career_plan.md       ← Your career roadmap
    │
    └── maintenance/
        ├── vital_info/          ← Equipment documentation
        │   └── vehicle_sedan_honda_civic_2020.md
        └── master_file.md       ← Master maintenance schedule
```

### Your Quick Reference Mnemonics

**Setup & Navigation**:
- `@bootstrap` - ONE-TIME setup (you did this!)
- `@nav` - "Route me to the right prompt for [task]"
- `@discover` - "What prompts are available for [topic]?"

**Career**:
- `career-cv-interviewer.md` - Build comprehensive CV (you did this!)
- `@career-analyzer` - Gap analysis and roadmap (you did this!)
- `career transition workflow` - 4-step process (analysis → assessment → resume → job search)

**Maintenance**:
- `@equipment-doc` - Document equipment (you did this!)
- `@maintenance-planner` - Master schedule (you did this!)

**Next to Try**:
- `@giftfinder` - Gift shopping system (optional exercise)
- `@tutor` - Learn any topic with personalized lessons
- `@coach` - Create training sessions
- `@meta-librarian` - Build custom prompts

---

## Optional Exercises (Independent Projects)

### 1. Gift Management System

**Use**: `@giftfinder` prompt

**What you'll build**:
- Recipient profiles in `docs/gift-profiles/`
- Gift history tracking (never give same gift twice)
- AI-powered gift search with web integration

**Try this**:
1. Navigate to `utilities/giftfinder-shopping-assistant.md`
2. Create profile for 1-2 gift recipients
3. Search for gifts using AI web search
4. See how AI prevents duplicate gifts

**Time**: 30-45 minutes

---

### 2. Braindump Structuring Prompts

**Use**: `@meta-librarian` to create custom prompts

**What you'll learn**: How to transform stream-of-consciousness notes into structured documents

**Example prompts to build**:
- Meeting notes → Action items + decisions + follow-ups
- Journal entries → Insights + patterns + themes
- Random ideas → Organized project plan
- Voice memos → Structured documentation

**Try this**:
1. Think of something you frequently capture in messy notes
2. Use `@meta-librarian` prompt
3. Describe what you want: Input (messy notes) → Output (structured doc)
4. AI creates custom prompt for you
5. Test it with your actual notes

**Time**: 45-60 minutes

---

### 3. Explore More Prompts

**Architecture Experts** (if you're technical):
- `@cloud` - AWS/Azure/GCP architecture guidance
- `@api` - REST/GraphQL/gRPC design
- `@security` - Zero-trust, compliance, threat modeling

**Workflows**:
- Career Transition Workflow (`workflows/career-transition/`)
  - 4-step process: Analysis → Qualification Assessment → Resume → Job Search
  - Builds on the career work you did today!
- Slide Deck Workflow (`workflows/slide_deck_workflow/`)
  - Extract corporate style → Apply to content → Architect deck → Assemble

**Utilities**:
- `@tutor` - Learn any topic with personalized curriculum
- Excel automation prompts
- More maintenance and productivity tools

---

## Community & Support

### GitHub Repository
- **URL**: https://github.com/danbrickey/pay_no_attention
- **Use for**:
  - Questions and discussions
  - Reporting issues or bugs
  - Seeing updates and new prompts
  - Sharing your custom prompts (if you build any)

### Updating Your Repository
When new prompts are released:
```bash
# In your repo folder, add original repo as "upstream"
git remote add upstream https://github.com/danbrickey/pay_no_attention.git

# Fetch updates
git fetch upstream

# Merge updates (careful - review changes first!)
git merge upstream/main
```

### Keep Learning
- Read the full library: `ai-resources/prompts/README.md`
- Explore prompt categories
- Try @discover for interactive exploration
- Update `.ai/instructions.md` as you learn more about yourself

---

## Tips for Success

### 1. Update Your Configuration Regularly
As you learn what's useful, edit `.ai/instructions.md`:
- Add new career goals
- Update skills you've learned
- Refine your communication preferences

### 2. Use the Navigation Tools
Don't try to remember all 93 prompts:
- **@nav** when you know what you need: "I need help with X"
- **@discover** when browsing: "Show me prompts for Y"
- **README** for comprehensive catalog

### 3. Start with Your Actual Needs
Don't try to use every prompt:
- Focus on prompts that solve YOUR problems
- Build up your docs/ folder with YOUR work
- Customize over time

### 4. Trust the Structure
The prompts are designed to:
- Ask the right questions
- Produce the right format
- Save to the right location

Let them guide you - they've been engineered for this.

### 5. Remember the Philosophy
**"Civilization advances by extending the number of important operations which we can perform without thinking about them."**

The goal isn't to learn all the prompts. The goal is to *stop thinking about* career planning, maintenance tracking, gift shopping, etc., because the system handles it.

**Pay no attention** - because the system is working.

---

## Quick Reference Card

### Essential Commands (Git)
```bash
git add .                    # Stage all changes
git commit -m "message"      # Save checkpoint
git push                     # Backup to cloud
git pull                     # Download updates
git status                   # See what changed
```

### Essential File Locations
- **Your config**: `.ai/instructions.md`
- **Prompt library**: `ai-resources/prompts/`
- **Your work**: `docs/`
- **Career stuff**: `docs/career/`
- **Maintenance**: `docs/maintenance/`

### Essential Prompts (Mnemonics)
- **@bootstrap** - Setup (one-time)
- **@nav** - Navigation
- **@discover** - Exploration
- **@career-analyzer** - Career planning
- **@equipment-doc** - Maintenance docs
- **@giftfinder** - Gift shopping
- **@tutor** - Learning
- **@meta-librarian** - Create prompts

### Getting Help
1. Use **@nav**: "Help me with [problem]"
2. Read **README**: `ai-resources/prompts/README.md`
3. Ask instructor or GitHub discussions

---

## Congratulations!

You've transformed how you work with AI. You're no longer chatting with a bot - you're directing an executive assistant that knows your context, maintains your knowledge, and delivers structured outputs.

Now go build something amazing. And pay no attention to all the complexity this system is handling for you - that's the point. 🚀

---

*Student Manual v1.0*
*Created: 2025-10-25*
*For: Getting Started with pay_no_attention (120-minute session)*
