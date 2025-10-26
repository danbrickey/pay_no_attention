# Instructor's Guide: Getting Started with pay_no_attention

**Duration**: 120 minutes
**Audience**: Tech-fluent adults (20s-30s), no formal technical training required
**Session Goals**: Set up environment, bootstrap personal config, complete 3 hands-on labs

---

## Pre-Session Preparation

### Materials Needed
- Projector/screen for demonstrations
- Student Manual (provided) - one per participant or digital access
- Quick Reference Guide (provided) - one per participant
- Backup USB drives with VS Code installer (in case of internet issues)
- Sample equipment photo/manual (for demonstration)

### Technology Setup
- Verify projector works with your laptop
- Test GitHub access (ensure not blocked by venue network)
- Have VS Code pre-installed on your machine for demos
- Clone pay_no_attention repo in advance to show working example
- Prepare Claude Code or similar AI coding assistant for live demos

### Pre-Reading (Optional for Participants)
- Send repository link 24 hours before: https://github.com/[your-username]/pay_no_attention
- Quick Start Guide: `ai-resources/prompts/QUICK_START.md`
- README overview: `ai-resources/prompts/README.md`

---

## Session Outline & Timing

### Opening (5 minutes)
**Goal**: Set context, establish rapport, preview journey

**Key Points**:
- Welcome and icebreaker: "Who here has used ChatGPT or Claude for work?"
- Introduce the Whitehead quote and project philosophy
- Set expectations: Hands-on, safe environment to ask questions

**What to Say**:
> "Welcome! Today we're going to transform how you work with AI. Instead of chatting with AI like a search engine, you're going to build a personal executive assistant that knows your context, manages your knowledge, and helps you accomplish complex tasks. The name 'pay_no_attention' comes from philosopher Alfred North Whitehead, who said 'Civilization advances by extending the number of important operations which we can perform without thinking about them.' That's exactly what we're building - systems that handle the mental overhead so you can focus on what matters."

**Gauge Understanding**:
- "Has anyone used structured prompts before? What was your experience?"
- "What tasks do you find yourself doing repeatedly that you wish were automated?"

---

### Module 1: Foundation Setup (30 minutes)
**Goal**: Everyone has working development environment

**Teaching Points**:

- **Why VS Code + GitHub?**
  - Why this matters: VS Code gives AI assistants full context of your files; GitHub preserves your work
  - Common misconception: "I need to be a programmer to use these tools"
  - Key phrase to use: "Think of VS Code as Microsoft Word for code and documents, and GitHub as Google Drive with superpowers"

- **The Git Workflow (Simplified)**
  - Why this matters: You can safely experiment without breaking things
  - Common misconception: "Git is too complex for me"
  - Key phrase to use: "Clone means copy, commit means save a checkpoint, push means backup to cloud"

**Socratic Moments**:
🤔 **Question**: "Why might we want our AI assistant to have access to all our documents in one place instead of asking it questions one at a time?"
- **What you're looking for**: Realization that context persistence enables smarter assistance
- **If they struggle**: "Think about working with a human assistant - would they be more helpful if they remembered your past projects and preferences?"
- **A-ha moment**: "Oh! The AI can connect information across different areas of my life because it sees everything together!"

**Example/Demo**:
1. Show VS Code interface (5 min)
   - File explorer panel
   - Editor area
   - Terminal/command palette
   - Extensions marketplace

2. GitHub account creation walkthrough (5 min)
   - Navigate to github.com
   - Sign up process
   - Email verification

3. Clone repository demonstration (10 min)
   ```bash
   # Show this command and explain each part:
   git clone https://github.com/danbrickey/pay_no_attention.git
   # git = version control tool
   # clone = make a copy
   # URL = where to copy from
   # Result: folder on your computer
   ```

4. Create personal repository (10 min)
   - Fork vs. new repo explanation
   - For this class: Creating NEW repo recommended
   - Copy files from cloned repo
   - First commit and push

**Practice (if time permits)**:
- Have participants open VS Code and explore the file structure
- Find specific files: `.ai/instructions.md`, `ai-resources/prompts/README.md`

**Transition**:
> "Now that everyone has the code on their machine, let's understand what we just downloaded and why it's powerful."

---

### Module 2: Project Philosophy & Navigation (15 minutes)
**Goal**: Participants understand the 'why' and can navigate the library

**Teaching Points**:

- **The Whitehead Philosophy**:
  - Why this matters: Understanding the philosophy helps you see applications everywhere
  - Common misconception: "This is just a collection of prompts"
  - Key phrase to use: "Every prompt is designed to remove mental overhead from a specific task"

- **AI Executive Assistant vs. Chatbot**:
  - Why this matters: Changes how you interact with AI
  - Common misconception: "I just ask the AI what to do"
  - Key phrase to use: "Executive assistants anticipate needs, maintain context, and deliver structured outputs"

- **The 93-Prompt Library Structure**:
  - Why this matters: Knowing what's available multiplies your effectiveness
  - Key phrase to use: "10 meta prompts for setup and creation, 6 architecture experts, 60 career paths, 5 workflows, and more"

**Socratic Moments**:
🤔 **Question**: "If you had a human executive assistant, what would you want them to remember about you and your work?"
- **What you're looking for**: Recognition of need for persistent context
- **If they struggle**: "Would you want to re-explain your career goals every time you met with them?"
- **A-ha moment**: "That's what .ai/instructions.md does - it gives the AI persistent memory of who I am!"

**Example/Demo**:
Walk through the directory structure on screen:
```
pay_no_attention/
├── .ai/                          ← Your personal configuration
│   ├── instructions.md           ← AI knows your context
│   └── context.md                ← Project-specific notes
├── ai-resources/
│   └── prompts/                  ← 93 ready-to-use prompts
│       ├── meta/                 ← @bootstrap, @nav, @discover
│       ├── architecture/         ← @cloud, @api, @security
│       ├── career/               ← 60 career path guides
│       ├── workflows/            ← Multi-step processes
│       └── utilities/            ← Practical tools
└── docs/                         ← Your documentation
```

Show live navigation:
1. Open README.md in VS Code
2. Show mnemonic table: @bootstrap, @nav, @discover
3. Demonstrate clicking through to a prompt file
4. Explain how AI uses these prompts

**Transition**:
> "Let's put this into practice. Your first lab will customize this entire system for YOUR life and YOUR goals."

---

### Module 3: Lab 1 - Bootstrap Your Personal Assistant (25 minutes)
**Goal**: Personalized `.ai/instructions.md` created and understood

**Teaching Points**:

- **The Bootstrap Interview Process**
  - Why this matters: Quality input = quality assistance
  - Common pitfall: Being too vague ("I like tech stuff")
  - Key phrase to use: "The AI can't read your mind, but it can remember everything you tell it"

- **What Goes in instructions.md**
  - Why this matters: This is the persistent context for ALL AI interactions in this project
  - Common misconception: "I have to fill out every field"
  - Key phrase to use: "Start with basics, add more as you learn what's useful"

**Socratic Moments**:
🤔 **Question**: "Why might it be valuable to tell the AI about your learning style (hands-on vs. theory-first)?"
- **What you're looking for**: Recognition that AI adapts its responses
- **If they struggle**: "If you learn best by doing, should the AI give you 10 pages of theory or a quick example and a task?"
- **A-ha moment**: "The AI will customize HOW it teaches me, not just WHAT it teaches!"

**Lab Setup (5 minutes)**:
1. Everyone open VS Code to the pay_no_attention folder
2. Navigate to `ai-resources/prompts/meta/bootstrap-setup.md`
3. Open Claude Code (or similar AI coding assistant)
4. Type: `@bootstrap`

**Lab Instructions (15 minutes)**:

Provide printed/displayed step-by-step:

1. **Initiate Bootstrap** (1 min)
   - In AI chat: Type `@bootstrap` and press enter
   - AI will ask if you've copied ai-resources folder (say yes - you cloned it)

2. **Phase 1: Verification** (2 min)
   - AI confirms what's installed
   - Answer questions about new vs. update (answer: new)

3. **Phase 2: Interview** (10 min)
   - Answer the 7 question groups honestly
   - Don't worry about being perfect - you can update later
   - **Instructor tip**: Walk around and help if anyone gets stuck

   Example responses to share:
   - Role: "Software Project Manager"
   - Experience: "5 years"
   - Focus: Check "Product Management" and "Career Development"
   - Goals: "Get promoted to Senior PM in 6 months"

4. **Phase 3 & 4: Review Output** (2 min)
   - AI generates your instructions.md
   - Review what it created
   - Copy content to `.ai/instructions.md` file

**Debrief (5 minutes)**:
- "What surprised you about the interview?"
- "Look at someone else's instructions.md - how is it different from yours?"
- "This file will now influence EVERY interaction with AI in this project"

**Common Issues**:
- **"I don't know my technical stack"**: That's fine! Say "N/A" or leave blank
- **"What if I want to change this later?"**: You can edit `.ai/instructions.md` anytime
- **"Do I have to share personal info?"**: No! Only include what you're comfortable with

**Transition**:
> "Great! Now the AI knows who you are. Let's put it to work on something practical: your career."

---

### Break (10 minutes)

**During break:**
- Ensure everyone's `.ai/instructions.md` is saved
- Help anyone who fell behind catch up
- Verify AI assistants are connected and working

---

### Module 4: Lab 2 - Career Planning with AI (30 minutes)
**Goal**: Comprehensive CV created and career plan generated

**Teaching Points**:

- **Structured CV vs. Resume**
  - Why this matters: Machines can process structured data; humans need narrative
  - Common misconception: "A CV is just a long resume"
  - Key phrase to use: "This CV is a rich database about your career that can be transformed into any format"

- **Career Gap Analysis**
  - Why this matters: Shows exactly what stands between you and your goals
  - Common pitfall: Vague goals like "work in AI"
  - Key phrase to use: "The AI will quantify your fit and create a specific roadmap"

- **Versioned Career Plans**
  - Why this matters: Your plan will evolve; you want history
  - Key phrase to use: "Think of it like Track Changes for your life strategy"

**Socratic Moments**:
🤔 **Question**: "Why might a structured, detailed CV be more valuable than a polished one-page resume?"
- **What you're looking for**: Understanding of adaptability and AI processing
- **If they struggle**: "Which can you more easily customize: a template with structured data or a PDF paragraph?"
- **A-ha moment**: "I can generate MANY targeted resumes from ONE detailed CV!"

**Lab Setup (3 minutes)**:
1. Decide: Full CV interview OR use existing resume
   - **Recommended for class**: Abbreviated version (save time)
   - **For thorough result**: Full interview (can finish later)
2. Navigate to `ai-resources/prompts/career/career-cv-interviewer.md`
3. Have recent resume handy (if you have one)

**Lab Part A: Build CV (12 minutes)**:

**Quick Path** (if pressed for time):
1. Upload existing resume to AI
2. Ask AI to convert to structured CV using career-cv-interviewer format
3. Review and fill in gaps

**Interview Path** (fuller experience):
1. Use career-cv-interviewer.md prompt
2. AI conducts 6-phase interview
3. Answer questions about work history, skills, education
4. AI generates JSON-formatted CV
5. Save to `docs/career/cv.json`

**Instructor demonstration** (show on screen):
```
Me: I'd like to create a comprehensive CV
AI: [Runs career-cv-interviewer questions]
Me: [Answers about professional background]
AI: [Generates structured CV with metadata]
```

**Lab Part B: Career Analysis (15 minutes)**:

1. **Load Career Analyzer** (2 min)
   - Navigate to `career-analyzer.md`
   - In AI: `@career-analyzer`
   - Provide your CV (from Part A)

2. **Specify Target** (2 min)
   - Option 1: "Analyze for AI Product Manager transition"
   - Option 2: "What career paths fit my background?"
   - Option 3: Provide specific job description

3. **Receive Analysis** (10 min)
   - AI provides:
     - Match scores
     - Gap analysis with specific courses, certs, timeline
     - 2-3 AI career path recommendations
     - Detailed roadmap (Phase 1, 2, 3)
     - Cost and time estimates

4. **Save Career Plan** (1 min)
   - AI generates career_plan.md
   - Save to `docs/career/career_plan.md`

**Example to show**:
```markdown
## Career Path 1: AI Product Manager

Current Fit: 72/100

**Transferable Skills**:
- Product management experience → AI product lifecycle
- Stakeholder communication → Technical/business bridge
- Roadmap planning → AI feature prioritization

**Gap Analysis**:
- **Python basics**: Currently none → Need proficient
  - Course: "Python for Product Managers" (Coursera, 20 hrs, $49)
  - Timeline: Month 1-2

...
```

**Common Issues**:
- **"My CV isn't detailed enough"**: That's fine! The AI will work with what you provide
- **"I don't know what AI career I want"**: Ask AI to recommend paths based on CV
- **"This analysis is overwhelming"**: Focus on Phase 1 recommendations first

**Transition**:
> "You now have a career roadmap with specific steps. Let's shift gears to something completely different: managing physical stuff in your life."

---

### Module 5: Lab 3 - Maintenance Documentation (25 minutes)
**Goal**: 1-2 equipment items documented, master schedule generated

**Teaching Points**:

- **Proactive vs. Reactive Maintenance**
  - Why this matters: Prevents expensive emergencies
  - Common misconception: "I'll just fix things when they break"
  - Key phrase to use: "An ounce of prevention is worth a pound of cure - and this makes prevention effortless"

- **AI Understanding Physical Equipment**
  - Why this matters: AI can read manuals, extract specs, research best practices
  - Common misconception: "I need to type everything manually"
  - Key phrase to use: "Take a photo, upload a manual, or just describe it - AI does the research"

- **Climate-Aware Scheduling**
  - Why this matters: Maintenance timing varies by location
  - Key phrase to use: "Your maintenance schedule is customized for YOUR climate, not generic advice"

**Socratic Moments**:
🤔 **Question**: "Why might it be useful to have all your maintenance tasks in one master calendar instead of scattered in different manuals?"
- **What you're looking for**: Recognition of efficiency and preventing forgotten tasks
- **If they struggle**: "Have you ever forgotten to change an air filter or service something until it became a problem?"
- **A-ha moment**: "I can see ALL my maintenance in one place and group related tasks together!"

**Lab Part A: Document Equipment (15 minutes)**:

**Setup** (3 min):
- Choose 1-2 items to document:
  - **Easy**: Car (most people have one, well-documented)
  - **Medium**: Home appliance (HVAC, refrigerator, washer)
  - **Advanced**: Power tool, equipment
- Have photos or manual PDFs ready

**Process** (12 min):

1. **Load Equipment Documenter** (1 min)
   - Navigate to `utilities/equipment-maintenance-documenter.md`
   - In AI: `@equipment-doc`

2. **Provide Information** (3 min)
   - Upload photo of equipment (model plate visible)
   - OR upload manual PDF
   - OR describe: "2020 Honda Civic, 45,000 miles, Chicago IL"

3. **Answer Context Questions** (2 min)
   - Location (for climate-specific guidance)
   - Owner or renter? (affects responsibilities)

4. **Receive Documentation** (5 min)
   - AI generates comprehensive maintenance guide:
     - Equipment specs
     - Maintenance schedule (with climate adjustments)
     - Detailed procedures
     - Materials needed with part numbers
     - Service provider recommendations (if location given)

5. **Save File** (1 min)
   - Save to `docs/maintenance/vital_info/`
   - Filename: `vehicle_sedan_honda_civic_2020.md`

**Example to show on screen**:

Upload photo of car → AI response:
```markdown
## Equipment Overview
- **Category**: Vehicle
- **Brand**: Honda
- **Model**: Civic (10th generation)
- **Year**: 2020
- **Ownership**: Owner

## Maintenance Schedule

| Task | Frequency | Best Timing | Climate Notes |
|------|-----------|-------------|---------------|
| Oil change | Every 5K miles | Any season | Synthetic recommended for Chicago winters |
| Tire rotation | Every 7.5K miles | Spring & Fall | Check pressure weekly in winter |
| Cabin air filter | Annually | Spring | High pollen area - may need 2x/year |

...
```

**Lab Part B: Create Master Plan (10 minutes)** *(if time allows)*:

1. **Load Maintenance Planner** (1 min)
   - Navigate to `utilities/household-maintenance-planner.md`
   - In AI: `@maintenance-planner`

2. **Scan and Synthesize** (8 min)
   - AI scans all files in `docs/maintenance/vital_info/`
   - Generates master schedule:
     - Monthly calendar view
     - Seasonal task summary
     - Annual budget estimates
     - Task grouping recommendations
     - Bulk purchase opportunities

3. **Save Master File** (1 min)
   - Save to `docs/maintenance/master_file.md`

**Example output**:
```markdown
## January

| Date | Task | Equipment | Duration | Cost |
|------|------|-----------|----------|------|
| Early Jan | Check tire pressure | Honda Civic | 5 min | $0 |
| Mid Jan | Replace HVAC filter | Home HVAC | 10 min | $15 |

**January Purchase List**:
- [ ] HVAC filter 16x20x1 MERV 11 - $15 - Buy at: Home Depot

**January Totals**: 2 tasks, 15 minutes, $15
```

**Common Issues**:
- **"I don't have photos/manuals handy"**: Use generic descriptions - AI will research
- **"AI can't identify my equipment from photo"**: Provide brand/model manually
- **"I'm a renter, not owner"**: Perfect! AI marks landlord vs. your responsibilities

**Transition**:
> "You've now set up three major systems: career planning, and maintenance tracking. Let's wrap up and talk about where to go from here."

---

### Module 6: Wrap-up & Next Steps (15 minutes)
**Goal**: Solidify learning, provide ongoing resources, energize for continued use

**Key Points**:
- Recap what was built today
- Highlight the power of persistent context
- Provide roadmap for continued exploration

**What to Say**:
> "In two hours, you've built a personalized AI executive assistant that knows your career goals, tracks your maintenance needs, and can help with dozens of other tasks. More importantly, you understand HOW to work with structured prompts and persistent context. This isn't just about the prompts we used today - it's about a new way of working with AI."

**Activity: Quick Review Game** (5 min)
Ask rapid-fire questions, hands up to answer:
- "Where is your personal context stored?" (.ai/instructions.md)
- "How many ready prompts are in this library?" (93)
- "Which prompt helps you find other prompts?" (@nav or @discover)
- "What's the mnemonic for setting up the system?" (@bootstrap)
- "Can you edit .ai/instructions.md anytime?" (Yes!)

**Present Optional Exercises** (3 min):

1. **Gift Management System**
   - Use @giftfinder to create recipient profiles
   - Never forget what you've given someone
   - Search for perfect gifts with AI web search
   - Located: `utilities/giftfinder-shopping-assistant.md`

2. **Braindump Structuring**
   - Create custom prompts that transform messy notes into structured documents
   - Use @meta-librarian to build your own prompts
   - Examples: Meeting notes → action items, journal entries → insights
   - Located: `meta/meta-librarian-architect.md`

3. **Explore More Workflows**
   - Career Transition Workflow (4-step process)
   - Slide Deck Creation Workflow
   - Located: `workflows/` directory

**Provide Quick Reference Cards** (2 min):
- Hand out or display Quick Reference (see 03_quick_reference.md)
- Bookmark key locations
- Mnemonic cheat sheet

**Community & Support** (2 min):
- GitHub repository: https://github.com/danbrickey/pay_no_attention
- Issues/discussions for questions
- Future session announcements
- Share your success stories

**Q&A** (3 min):
Open floor for questions

**Closing** (1 min):
> "The name 'pay_no_attention' reminds us that the best systems are the ones you don't have to think about. You've built the foundation today. As you use these prompts, update your .ai/instructions.md, and add your own documentation, this system will become second nature. You won't think about HOW to get career advice or manage maintenance - you'll just DO it, effortlessly. That's the power of good automation. Now go build amazing things!"

---

## Facilitation Tips

### Pacing
- ⏱️ **If running behind**:
  - Skip Lab 3 Part B (master planner) - can do independently
  - Shorten Module 2 philosophy discussion to 10 minutes
  - Have participants finish CV interview as homework

- ⏱️ **If ahead of schedule**:
  - Do longer equipment documentation (2-3 items instead of 1)
  - Show additional prompts (@coach, @tutor, architecture experts)
  - Deeper dive into Git workflow
  - Start optional exercise (gift finder demo)

### Energy Management
- **High energy needed**: Module 1 (setup can be tedious), starts of labs
- **Reflective moments**: Module 2 philosophy, between labs when reviewing outputs
- **Break points**: Scheduled break after Lab 1; offer quick stretch at 75-minute mark

### Reading the Room
- **Signs of confusion**: Lots of hands up, people stuck on same step, blank stares
  - **Response**: Pause for group Q&A, show on screen, walk through together

- **Signs of boredom**: People on phones, side conversations, rushing ahead
  - **Response**: Speed up exposition, get to hands-on faster, offer advanced challenges

- **Signs of engagement**: Questions, "aha" moments, helping neighbors, excited comments
  - **Response**: Encourage questions, celebrate discoveries, let them explore

### Common Pitfalls

1. **GitHub authentication issues**
   - **How to avoid**: Have participants set up personal access tokens in advance
   - **How to handle**: Have alternative: use GitHub Desktop GUI instead of command line

2. **AI assistant not connected/working**
   - **How to avoid**: Test before session, have backup accounts
   - **How to handle**: Pair up participants, demonstrate on your screen

3. **Information overload**
   - **How to avoid**: Focus on "why" not just "what," relate to their experience
   - **How to handle**: Remind them they have the manual, focus on core concepts

4. **Participants with very different skill levels**
   - **How to avoid**: Set clear expectations in session description
   - **How to handle**: Pair advanced with beginners, offer extension activities

---

## Socratic Question Bank

Use these strategically to prompt discovery:

**For Module 1** (Setup):
- "Why might a developer use version control? What problem does it solve?"
- "What's the advantage of having your files in the cloud versus only on your laptop?"
- "If two people edit the same file, how might Git help them merge their changes?"

**For Module 2** (Philosophy):
- "What's the difference between asking ChatGPT one question vs. building a system with persistent context?"
- "If the AI remembers your career goals, how might that change the quality of its advice?"
- "Why might we organize 93 prompts into categories instead of one giant prompt file?"

**For Module 3** (Bootstrap):
- "Should you tell the AI your communication preference (concise vs. detailed)? Why?"
- "What happens if your career goals change in 6 months? Can you update your config?"
- "Why might it be useful for the AI to know your learning style?"

**For Module 4** (Career):
- "Why might a gap analysis be more valuable than just 'learn AI stuff'?"
- "What's the benefit of having specific course names vs. 'take some online classes'?"
- "If you had a career coach, would you want them to remember past conversations? How is this similar?"

**For Module 5** (Maintenance):
- "Why might maintenance timing differ between Miami and Minnesota?"
- "What's the advantage of grouping similar tasks (all filter changes) on the same day?"
- "How does this prevent the 'I forgot to service it' problem?"

---

## Success Indicators

You'll know the session worked if:
- ✅ 80%+ of participants have working repos by Module 1 end
- ✅ Everyone completes at least 2 of 3 labs
- ✅ Participants articulate the "persistent context" concept
- ✅ At least 3 "aha moment" visible reactions during Socratic questions
- ✅ Questions shift from "how do I..." to "can I use this for..."
- ✅ People stay engaged through all 120 minutes (not checked out)
- ✅ Post-session: Participants report using prompts independently

---

## Post-Session

### Follow-Up
- Send link to repository (if not already shared)
- Share digital copies of Student Manual and Quick Reference
- Provide list of next learning resources:
  - Full prompt library README
  - Community forum/Discord
  - Office hours schedule (if offering)

### Self-Reflection
- What went well?
  - [Which labs generated most engagement?]
  - [Which explanations landed best?]
  - [Timing accuracy?]

- What would you adjust?
  - [Any modules too long/short?]
  - [Technical issues to solve?]
  - [Examples to improve?]

- What surprised you?
  - [Unexpected questions?]
  - [Different use cases discovered?]
  - [Participant backgrounds different than expected?]

---

*Instructor Guide v1.0*
*Created: 2025-10-25*
*For: Getting Started with pay_no_attention (120-minute session)*
