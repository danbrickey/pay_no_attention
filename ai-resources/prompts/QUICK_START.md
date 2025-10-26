---
title: "AI Prompts Library - Quick Start Guide"
author: "Dan Brickey"
last_updated: "2025-10-25"
version: "1.0.0"
category: "getting-started"
tags: ["quick-start", "onboarding", "top-picks", "persona-based"]
status: "active"
purpose: "Fast onboarding guide - top prompts by persona and common workflows"
---

# AI Prompts Library - Quick Start Guide

Welcome! This library has **88 ready-to-use prompts + 3 templates**. Here's how to get started fast.

## 🚀 First-Time Users: Start Here

### Step 1: Navigation Tools (Pick One)

**New to the library?** Start with one of these:

1. **[@nav](meta/nav-resource-navigator.md)** 🧭 - Navigation Assistant
   - Use when: You know what you want but not which prompt
   - Type: `@nav I need help with [your task]`
   - Example: `@nav I need to design a REST API`

2. **[@discover](meta/discover-prompt-finder.md)** 🔍 - Interactive Prompt Finder
   - Use when: Browsing or exploring what's available
   - Type: `@discover` then answer questions
   - Perfect for: First-time exploration

3. **Browse by persona** (this guide) - See top picks below

### Step 2: Find Your Persona

Jump to the section that matches you:
- [Software Engineer / Developer](#software-engineer--developer)
- [Architect / Technical Lead](#architect--technical-lead)
- [Product Manager / Business Analyst](#product-manager--business-analyst)
- [Career Changer / Job Seeker](#career-changer--job-seeker)
- [Documentation Writer / Technical Writer](#documentation-writer--technical-writer)
- [Startup Founder / Solo Builder](#startup-founder--solo-builder)
- [Student / Learner](#student--learner)

---

## 👥 Top Prompts by Persona

### Software Engineer / Developer

**Your Top 5 Prompts**:

1. **[@api](architecture/api-architect.md)** - API Architecture Expert
   - Design REST/GraphQL/gRPC APIs
   - Microservices communication patterns
   - Authentication, versioning, developer experience

2. **[@cloud](architecture/cloud-architect.md)** - Cloud Architecture Expert
   - AWS, Azure, GCP design
   - Serverless vs. containers vs. VMs
   - Cost optimization, scalability

3. **[@security](architecture/security-architect.md)** - Security Architecture Expert
   - Zero-trust architecture
   - OWASP Top 10 mitigation
   - Compliance (GDPR, HIPAA, SOC2)

4. **[Vibe Coding](development/vibe-coding/)** - Developer Experience Assistant
   - Clean code practices
   - Iterative development
   - Code reviews

5. **[@drawio](architecture/drawio-diagram-specialist.md)** - Architecture Diagrams
   - System architecture diagrams
   - C4 model visualizations
   - Technical documentation

**Common Workflows**:
- API Design: @api → @security → @drawio → @arcdoc
- Cloud Migration: @cloud → @security → @arcdoc
- New Feature: @api → vibe-coding → @arcdoc

---

### Architect / Technical Lead

**Your Top 5 Prompts**:

1. **[@cloud](architecture/cloud-architect.md)** - Cloud Architecture Expert
   - Multi-cloud strategies
   - Well-Architected Framework
   - Infrastructure decisions

2. **[@api](architecture/api-architect.md)** - API Architecture Expert
   - API strategy and governance
   - Microservices architecture
   - API gateway patterns

3. **[@security](architecture/security-architect.md)** - Security Architecture Expert
   - Threat modeling (STRIDE)
   - Defense-in-depth
   - Compliance frameworks

4. **[@architect](architecture/architect-data-vault.md)** - Data Architecture Expert
   - Data Vault 2.0 modeling
   - Dimensional modeling (Kimball)
   - Snowflake optimization

5. **[@arcdoc](documentation/arcdoc-documentation-architect.md)** - Architecture Documentation
   - Multi-audience docs (exec → technical)
   - Interview mode for requirements
   - Braindump processing

**Common Workflows**:
- System Design: @cloud + @api + @security → @drawio → @arcdoc
- Data Platform: @architect → @cloud → @arcdoc
- Architecture Review: @security (threat model) → @arcdoc

**Pro Tip**: Use architecture templates to create custom experts for your specific domain (network, software, platform).

---

### Product Manager / Business Analyst

**Your Top 5 Prompts**:

1. **[Technical Requirements](architecture/technical-requirements/)** - Requirements Elicitation
   - Define technical requirements
   - Gap analysis
   - Validation frameworks

2. **[@projdoc](documentation/projdoc-expert.md)** - Project Documentation
   - PRDs, specs, roadmaps
   - Stakeholder communication
   - Project structure

3. **[@meeting](documentation/meeting-notes-summarizer.md)** - Meeting Notes Summarizer
   - Convert notes to action items
   - Track decisions and owners
   - Follow-up reminders

4. **[AI Vendor Evaluation](strategy/ai-vendor-evaluation/)** - Strategic Assessment
   - Vendor comparison frameworks
   - Build vs. buy decisions
   - Risk assessment

5. **[@arcdoc](documentation/arcdoc-documentation-architect.md)** - Technical Documentation
   - Business-friendly architecture docs
   - Executive summaries
   - Cross-functional communication

**Common Workflows**:
- New Feature: Technical Requirements → @projdoc → @meeting
- Vendor Selection: AI Vendor Evaluation → @projdoc
- Roadmap Planning: @projdoc → @meeting → @arcdoc

---

### Career Changer / Job Seeker

**Your Top 5 Prompts**:

1. **[Career Analyzer](career/career-analyzer.md)** - Multi-Domain Career Analysis
   - Compare roles across industries
   - Identify skill gaps
   - Create development plans

2. **Career Path Prompts** (60 role-specific prompts)
   - Pick your target role from:
     - [AI/ML Careers](career/ai_career_paths/) (16 roles)
     - [Tech Careers](career/tech_career_paths/) (8 roles)
     - [Business Careers](career/business_career_paths/) (7 roles)
     - [Creative Careers](career/creative_career_paths/) (9 roles)
     - [Healthcare Careers](career/healthcare_career_paths/) (4 roles)
     - [Finance/Sales Careers](career/finance_sales_career_paths/) (5 roles)
     - [Vocational/Entry-Level](career/vocational_career_paths/) (11 roles)

3. **[Resume Builder](career/resume-builder/)** - Professional Resume Creation
   - ATS-optimized resumes
   - Industry-specific guidance
   - Multiple resume formats

4. **[Job Search Strategist](career/job-search-strategist/)** - Strategic Job Search
   - Job posting analysis
   - Application strategy
   - Networking guidance

5. **[@tutor](specialized/tutor-learning-assistant.md)** - Learning Assistant
   - Skill development plans
   - Personalized learning paths
   - Practice exercises

**Common Workflow** (Career Transition):
1. Career Analyzer → identify target role
2. Specific Career Path (e.g., Full Stack Engineer) → assess qualification
3. Follow roadmap from career path
4. Resume Builder → create tailored resume
5. Job Search Strategist → apply strategically

---

### Documentation Writer / Technical Writer

**Your Top 5 Prompts**:

1. **[@arcdoc](documentation/arcdoc-documentation-architect.md)** - Architecture Documentation
   - 4 modes: Interview, Braindump, Discovery, Organization
   - Multi-audience layering
   - Technical + business documentation

2. **[@projdoc](documentation/projdoc-expert.md)** - Project Documentation
   - README files, setup guides
   - User documentation
   - Internal wikis

3. **[@bizrules](documentation/bizrules-documenter.md)** - Business Rules Documentation
   - Extract rules from code
   - Document domain logic
   - Compliance documentation

4. **[@drawio](architecture/drawio-diagram-specialist.md)** - Technical Diagrams
   - Architecture diagrams
   - Data flow diagrams
   - System context diagrams

5. **[@meeting](documentation/meeting-notes-summarizer.md)** - Meeting Summarizer
   - Action items extraction
   - Decision documentation
   - Follow-up tracking

**Common Workflows**:
- New Documentation: @arcdoc (interview) → @drawio → @projdoc
- Code → Docs: @bizrules → @arcdoc → @drawio
- Meeting → Actions: @meeting → @projdoc

---

### Startup Founder / Solo Builder

**Your Top 5 Prompts**:

1. **[@cloud](architecture/cloud-architect.md)** - Cloud Architecture
   - Startup-friendly cloud selection
   - Cost optimization for early stage
   - Serverless-first recommendations

2. **[@api](architecture/api-architect.md)** - API Design
   - MVP API design
   - Mobile backend patterns
   - Scaling strategies

3. **[@security](architecture/security-architect.md)** - Security Basics
   - Essential security for startups
   - SOC2 preparation
   - Cost-effective security

4. **[AI Vendor Evaluation](strategy/ai-vendor-evaluation/)** - Build vs. Buy
   - Tool selection framework
   - Vendor comparison
   - Cost-benefit analysis

5. **[@projdoc](documentation/projdoc-expert.md)** - Documentation
   - README for open source
   - API documentation
   - Investor/stakeholder docs

**Common Workflows**:
- MVP Design: @cloud → @api → @security → @projdoc
- Fundraising: @arcdoc → @drawio → @projdoc
- Hiring: Career paths → @projdoc (job descriptions)

**Pro Tip**: Focus on managed services (@cloud recommends serverless) to minimize operational overhead.

---

### Student / Learner

**Your Top 5 Prompts**:

1. **[@tutor](specialized/tutor-learning-assistant.md)** - Personalized Learning
   - Custom learning paths
   - Skill development plans
   - Practice exercises

2. **Career Path Exploration** (60 career prompts)
   - Explore career options by industry
   - Understand qualification requirements
   - Build skill roadmaps

3. **[@api](architecture/api-architect.md)** or **[@cloud](architecture/cloud-architect.md)**
   - Learn architecture patterns
   - Understand best practices
   - Real-world examples

4. **[@projdoc](documentation/projdoc-expert.md)** - Documentation Skills
   - Learn documentation practices
   - Portfolio project documentation
   - Technical writing

5. **[@meta](meta/meta-prompt-engineer.md)** - Learn Prompt Engineering
   - Understand prompt patterns
   - Build custom prompts
   - AI interaction skills

**Learning Paths**:
- **Backend Development**: @tutor → @api → @cloud → @security
- **Career Exploration**: Career Analyzer → Specific Career Path → @tutor
- **Technical Writing**: @projdoc → @arcdoc → @bizrules

---

## 🔥 Most Popular Prompts (All Personas)

1. **[@cloud](architecture/cloud-architect.md)** - Cloud Architecture (AWS/Azure/GCP)
2. **[@api](architecture/api-architect.md)** - API Design (REST/GraphQL/gRPC)
3. **[@security](architecture/security-architect.md)** - Security & Compliance
4. **[Career Paths](career/)** - 60 role-specific career guides
5. **[@arcdoc](documentation/arcdoc-documentation-architect.md)** - Architecture Documentation
6. **[@drawio](architecture/drawio-diagram-specialist.md)** - Architecture Diagrams
7. **[@architect](architecture/architect-data-vault.md)** - Data Architecture
8. **[@meta-librarian](meta/meta-librarian-architect.md)** - Create Custom Prompts
9. **[@projdoc](documentation/projdoc-expert.md)** - Project Documentation
10. **[@tutor](specialized/tutor-learning-assistant.md)** - Learning Assistant

---

## 🎯 Common Use Cases & Recommended Prompts

| Use Case | Recommended Prompts | Workflow |
|----------|---------------------|----------|
| **Design a cloud system** | @cloud, @security, @drawio | @cloud → @security → @drawio → @arcdoc |
| **Build an API** | @api, @security, @arcdoc | @api → @security → @arcdoc |
| **Change careers** | Career Analyzer, Career Paths, Resume Builder | Career Analyzer → Specific Path → Resume → Job Search |
| **Write technical docs** | @arcdoc, @projdoc, @drawio | @arcdoc (interview/braindump) → @drawio → @projdoc |
| **Learn a new skill** | @tutor, Career Paths | @tutor → Practice → Career Path (for job) |
| **Evaluate vendors/tools** | AI Vendor Evaluation | Evaluation → @projdoc (document decision) |
| **Create diagrams** | @drawio | @drawio (or use templates for other tools) |
| **Document meetings** | @meeting | @meeting → @projdoc (if follow-up needed) |
| **Build a prompt** | @meta-librarian | @meta-librarian → Test → Iterate |
| **Design data architecture** | @architect, @cloud | @architect → @cloud (infrastructure) → @arcdoc |

---

## 🛠️ Advanced Features

### Templates for Custom Prompts

If you need a prompt for a domain we don't cover:

1. **[General Architecture Expert Template](architecture/templates/general-architecture-expert.md)**
   - Create experts for: Network, Software, Platform, etc.
   - 30-60 min customization time

2. **[Technical Documentation Architect Template](architecture/templates/technical-documentation-architect.md)**
   - Create documentation systems for specific projects
   - 60-90 min customization time

3. **[Visual Architecture Specialist Template](architecture/templates/visual-architecture-specialist.md)**
   - Create diagram specialists for: Mermaid, PlantUML, etc.
   - 45-75 min customization time

**When to use templates**:
- Need similar functionality in different domain
- Organization-specific requirements
- Building a prompt family

**When to use @meta-librarian**:
- Completely new prompt type
- Uncertain about approach
- Want systematic evaluation of options

---

## 📚 Learn More

### Core Documentation
- **[Main README](README.md)** - Full library catalog with all 88 prompts
- **[Architecture Templates](architecture/templates/README.md)** - Template usage guide
- **[Prompting Pattern Library](meta/prompting-pattern-library/)** - Advanced techniques
- **[Agentic Development](meta/agentic-development/)** - Build with subagents

### Navigation Tools
- **[@nav](meta/nav-resource-navigator.md)** - Intelligent routing assistant
- **[@discover](meta/discover-prompt-finder.md)** - Interactive discovery
- **This guide** - Persona-based quick start

### Getting Help
- **[@nav](meta/nav-resource-navigator.md)** - "I need help with [task]"
- **[@discover](meta/discover-prompt-finder.md)** - Browse interactively
- **Main README** - Search by tag or category

---

## 💡 Pro Tips

1. **Use mnemonics**: Type `@cloud` instead of long file paths
2. **Combine prompts**: Many tasks need 2-3 prompts in sequence
3. **Check templates**: Before creating from scratch, see if template exists
4. **Start with @nav**: When unsure, ask Navigator for guidance
5. **Explore careers**: 60 career paths cover most industries
6. **Workflow thinking**: Complex tasks often need multiple phases
7. **Custom is OK**: Use @meta-librarian to create exactly what you need
8. **Documentation matters**: @arcdoc has 4 modes for different doc tasks
9. **Security first**: Always include @security in architecture workflows
10. **Learn continuously**: @tutor creates personalized learning paths

---

## 🚦 Next Steps

**New User Path**:
1. ✅ Read this guide
2. ✅ Pick your persona section above
3. ✅ Try your #1 recommended prompt
4. ✅ Explore related prompts
5. ✅ Combine prompts in workflows

**Returning User Path**:
1. Use mnemonic (@cloud, @api, etc.) for quick access
2. Check [Main README](README.md) for new prompts
3. Create custom prompts with @meta-librarian
4. Build workflows combining multiple prompts

**Power User Path**:
1. Customize templates for your organization
2. Build multi-prompt workflows
3. Create domain-specific prompt families
4. Contribute improvements back

---

**Welcome to the AI Prompts Library! Start with your persona's top picks above, and let @nav or @discover guide you from there.**

*Last Updated: 2025-10-25 | Version: 1.0.0*
