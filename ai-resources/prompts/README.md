---
title: "AI Prompts Library - Master Catalog"
author: "Dan Brickey"
last_updated: "2025-10-25"
version: "3.2.0"
category: "prompts-index"
tags: ["prompts", "AI-templates", "code-generation", "documentation", "architecture", "career", "templates", "cloud", "api", "security", "navigation", "discovery"]
status: "current"
contents: ["architecture", "documentation", "meta", "career", "workflows", "specialized", "development", "strategy", "utilities", "templates", "navigation"]
usage: "Centralized library of reusable prompt templates for consistent AI assistance across all domains"
---

# AI Prompts Library - Master Catalog

Welcome to the AI Prompts Library - a comprehensive collection of reusable prompt templates for AI assistance across career development, technical work, documentation, and personal productivity.

## 🚀 New to the Library? Start Here!

**Choose your path**:

1. **[@nav](meta/nav-resource-navigator.md) 🧭 Navigator** - Know what you need but not which prompt?
   - Type: `@nav I need help with [your task]`
   - Intelligent routing with decision trees

2. **[@discover](meta/discover-prompt-finder.md) 🔍 Discovery Assistant** - Want to explore what's available?
   - Type: `@discover` then answer questions
   - Interactive prompt exploration

3. **[Quick Start Guide](QUICK_START.md) 📖** - Find top prompts by persona
   - Software Engineer, Architect, Product Manager, Career Changer, etc.
   - Common workflows and use cases

## 🔍 Mnemonic Quick Reference

Type `@` + mnemonic for fast autocomplete in Claude Code:

| Mnemonic | Prompt | Purpose |
|----------|--------|---------|
| **@bootstrap** 🚀 | [Bootstrap Setup](meta/bootstrap-setup.md) | **ONE-TIME**: First-time library setup & customization |
| **@nav** 🧭 | [Navigator](meta/nav-resource-navigator.md) | Intelligent routing to right prompts/docs/workflows |
| **@discover** 🔍 | [Discovery Assistant](meta/discover-prompt-finder.md) | Interactive prompt exploration and finding |
| **@meta-librarian** ⭐ | [Meta-Librarian Architect](meta/meta-librarian-architect.md) | **UNIFIED** (recommended): Create + assess + organize |
| **@meta** | [Meta-Prompt Engineer](meta/meta-prompt-engineer.md) | Prompt engineering only (focused) |
| **@librarian** | [Prompt Librarian](meta/librarian-prompt-management.md) | Library management only (focused) |
| **@architect** | [Data Architect](architecture/architect-data-vault.md) | Data architecture & modeling expert (Data Vault 2.0) |
| **@cloud** | [Cloud Architect](architecture/cloud-architect.md) | Cloud architecture expert (AWS, Azure, GCP) |
| **@api** | [API Architect](architecture/api-architect.md) | API architecture expert (REST, GraphQL, gRPC) |
| **@security** | [Security Architect](architecture/security-architect.md) | Security architecture expert (zero-trust, compliance) |
| **@arcdoc** | [Architecture Docs](documentation/arcdoc-documentation-architect.md) | Architecture documentation with business rules |
| **@bizrules** | [Business Rules](documentation/bizrules-documenter.md) | Document business rules from code |
| **@projdoc** | [Project Docs](documentation/projdoc-expert.md) | Create project documentation |
| **@meeting** | [Meeting Notes](documentation/meeting-notes-summarizer.md) | Summarize meetings to action items |
| **@drawio** | [Drawio Specialist](architecture/drawio-diagram-specialist.md) | Create/edit Draw.io diagrams |
| **@tutor** | [AI Tutor](specialized/tutor-learning-assistant.md) | Personalized learning & skill development |
| **@coach** | [Coaching Session Builder](specialized/coaching-session-builder.md) | Create structured coaching sessions (instructor guide + student manual + quick reference) |
| **@equipment-doc** | [Equipment Maintenance Documenter](utilities/equipment-maintenance-documenter.md) | Create maintenance docs for equipment/tools/vehicles |
| **@maintenance-planner** | [Household Maintenance Planner](utilities/household-maintenance-planner.md) | Master schedule with optimization & budgeting |
| **@giftfinder** | [Gift Finder](utilities/giftfinder-shopping-assistant.md) | Gift shopping with recipient profiling & web search |

---

## 📂 Directory Structure

```
ai-resources/prompts/
├── architecture/          ← Architecture & technical design prompts
├── documentation/         ← Documentation generation & management prompts
├── meta/                  ← Prompt engineering & meta-prompts
├── career/                ← Career development & analysis prompts
├── workflows/             ← Multi-step workflow prompts
├── specialized/           ← Domain-specific utility prompts
├── development/           ← Software development & coding prompts
├── strategy/              ← Strategic planning & evaluation prompts
└── utilities/             ← Productivity & automation utilities
```

---

## 🏗️ Architecture Prompts

**Location**: [architecture/](architecture/)

Expert prompts for data architecture, technical design, and diagramming:

### Ready-to-Use Architecture Experts
- **[@architect](architecture/architect-data-vault.md)** - Data architecture expert for Data Vault 2.0, dimensional modeling, and Snowflake platform design.
- **[@cloud](architecture/cloud-architect.md)** - Cloud architecture expert for AWS, Azure, and GCP. Covers cloud-native patterns, Well-Architected Framework, multi-cloud strategies, and cost optimization.
- **[@api](architecture/api-architect.md)** - API architecture expert for REST, GraphQL, and gRPC. Specializes in microservices communication, API gateways, security, and developer experience.
- **[@security](architecture/security-architect.md)** - Security architecture expert for zero-trust, threat modeling, compliance (GDPR, HIPAA, PCI-DSS, SOC2), and defense-in-depth strategies.
- **[@drawio](architecture/drawio-diagram-specialist.md)** - Specialist for creating and editing Draw.io diagrams for architecture documentation.
- **[technical-requirements/](architecture/technical-requirements/)** - Systematic approach to defining, documenting, and validating technical requirements for software projects.

### Architecture Prompt Templates
**Location**: [architecture/templates/](architecture/templates/)

Reusable templates for creating domain-specific architecture prompts:

- **[General Architecture Expert](architecture/templates/general-architecture-expert.md)** - Template for creating architecture experts in any domain (software, cloud, enterprise, security, etc.). Customize to create specialists for your specific architecture needs.
- **[Technical Documentation Architect](architecture/templates/technical-documentation-architect.md)** - Template for creating documentation management systems for technical projects. Includes multi-audience layering, interview mode, braindump processing, and documentation discovery.
- **[Visual Architecture Specialist](architecture/templates/visual-architecture-specialist.md)** - Template for creating diagram specialists for any tool (Draw.io, Mermaid, PlantUML, Excalidraw). Supports multi-tool diagram generation with domain customization.

**What are templates?** These are generalized patterns extracted from successful specialized prompts. Use them to create new prompts for different domains, technologies, or projects. See [templates/README.md](architecture/templates/README.md) for detailed usage guidance.

---

## 📝 Documentation Prompts

**Location**: [documentation/](documentation/)

Prompts for generating and managing various types of documentation:

- **[@arcdoc](documentation/arcdoc-documentation-architect.md)** - Architecture documentation assistant with business rules integration. Interviews for missing details, processes braindumps, organizes documentation with multi-audience layering.
- **[@projdoc](documentation/projdoc-expert.md)** - Expert for creating comprehensive project documentation with proper structure and formatting.
- **[@bizrules](documentation/bizrules-documenter.md)** - Specialist for documenting business rules and domain logic in accessible formats.
- **[@meeting](documentation/meeting-notes-summarizer.md)** - Assistant for summarizing meeting notes into actionable items and key decisions.

---

## 🧠 Meta / Prompt Engineering

**Location**: [meta/](meta/)

Tools for creating and improving prompts themselves:

> 💡 **New to the library?** Start with `@nav` or `@discover` for finding prompts, or use `@meta-librarian` to create new ones.

### First-Time Setup
- **[@bootstrap](meta/bootstrap-setup.md)** 🚀 - **One-Time Setup Assistant**: Guides you through initial library setup when copying into a new project. Customizes `.ai/instructions.md` through a structured interview, establishes documentation structure, and provides a personalized tour. **Use once when installing the library.**

### Navigation & Discovery (START HERE)
- **[@nav](meta/nav-resource-navigator.md)** 🧭 - **Intelligent Router**: Knows the entire AI resources ecosystem. Directs you to the right prompts, docs, or workflows with decision trees and confidence-based routing. **Use when you know what you need but not which prompt.**

- **[@discover](meta/discover-prompt-finder.md)** 🔍 - **Interactive Discovery**: Conversational prompt exploration through questions and guided navigation. **Use when browsing or exploring what's available.**

- **[Quick Start Guide](QUICK_START.md)** 📖 - **Persona-Based Quick Start**: Top prompts by persona (Software Engineer, Architect, PM, Career Changer, etc.) with common workflows. **Use when first learning the library.**

### Prompt Creation (Recommended)
- **[@meta-librarian](meta/meta-librarian-architect.md)** ⭐ - **UNIFIED SYSTEM**: Combines prompt engineering (systematic evaluation with 3 candidates), agentic workflow assessment (when to use subagents), and library management (organization & discovery). **Most users want this.**

### Focused Tools
- **[@meta](meta/meta-prompt-engineer.md)** - Prompt engineering only: Creates high-quality prompts using systematic evaluation methodology with rubric scoring and evidence-based selection.
- **[@librarian](meta/librarian-prompt-management.md)** - Library management only: Organizes, categorizes, discovers, and maintains the prompt library with metadata enhancement.

### Supporting Resources
- **[prompting-pattern-library/](meta/prompting-pattern-library/)** - Comprehensive library of prompting patterns, techniques, and best practices (25+ patterns, failure modes, model quirks).
- **[agentic-development/](meta/agentic-development/)** - Expert guidance on building autonomous AI agents and agentic workflows ("Just Talk To It" methodology).
- **[data_vault_refactor_prompt_generator.md](meta/data_vault_refactor_prompt_generator.md)** - Generator for creating Data Vault refactoring prompts for specific tables/entities.

---

## 💼 Career Development Prompts

**Location**: [career/](career/)

Comprehensive career planning, analysis, and role-specific guidance across all industries:

### Career Planning & Analysis
- **[career-analyzer.md](career/career-analyzer.md)** - Multi-domain career path analyzer for technology, business, creative, healthcare, and finance roles. Analyze career fit, create development plans, and identify skill gaps.
- **[career-cv-interviewer.md](career/career-cv-interviewer.md)** - Interview assistant for building comprehensive CV/resume content.

### Career Path Exploration by Industry

#### AI & Machine Learning Careers
**Location**: [career/ai_career_paths/](career/ai_career_paths/)

Specialized prompts for AI/ML career paths:

#### Technical Roles
- [ai_prompt_engineer.md](career/ai_career_paths/ai_prompt_engineer.md)
- [ml_engineer.md](career/ai_career_paths/ml_engineer.md)
- [deep_learning_engineer.md](career/ai_career_paths/deep_learning_engineer.md)
- [ai_research_scientist.md](career/ai_career_paths/ai_research_scientist.md)
- [nlp_engineer.md](career/ai_career_paths/nlp_engineer.md)
- [computer_vision_engineer.md](career/ai_career_paths/computer_vision_engineer.md)

#### Business & Strategy Roles
- [ai_product_manager.md](career/ai_career_paths/ai_product_manager.md)
- [ai_strategist.md](career/ai_career_paths/ai_strategist.md)
- [ai_customer_success_manager.md](career/ai_career_paths/ai_customer_success_manager.md)

#### Governance & Compliance Roles
- [ai_ethics_officer.md](career/ai_career_paths/ai_ethics_officer.md)
- [ai_governance_specialist.md](career/ai_career_paths/ai_governance_specialist.md)
- [ai_compliance_manager.md](career/ai_career_paths/ai_compliance_manager.md)

#### Specialized Roles
- [ai_coach.md](career/ai_career_paths/ai_coach.md)
- [ai_content_creator.md](career/ai_career_paths/ai_content_creator.md)
- [ai_change_management_specialist.md](career/ai_career_paths/ai_change_management_specialist.md)
- [conversational_ai_ux_designer.md](career/ai_career_paths/conversational_ai_ux_designer.md)
- [data_annotator_ai_trainer.md](career/ai_career_paths/data_annotator_ai_trainer.md)

#### Technology (Non-AI) Careers
**Location**: [career/tech_career_paths/](career/tech_career_paths/)

Traditional technology and software engineering roles:
- [full_stack_engineer.md](career/tech_career_paths/full_stack_engineer.md) ✅ **Created**
- DevOps Engineer / SRE (template ready)
- Cloud Architect (template ready)
- Cybersecurity Specialist (template ready)
- Database Administrator (template ready)
- QA/Test Automation Engineer (template ready)
- Systems Administrator (template ready)
- Network Engineer (template ready)

#### Business & Management Careers
**Location**: [career/business_career_paths/](career/business_career_paths/)

Business strategy, analysis, and management roles:
- [product_manager.md](career/business_career_paths/product_manager.md) ✅ **Created**
- Project Manager (template ready)
- Business Analyst (template ready)
- Management Consultant (template ready)
- Operations Manager (template ready)
- Strategy Consultant (template ready)
- Agile Coach/Scrum Master (template ready)

#### Creative & Design Careers
**Location**: [career/creative_career_paths/](career/creative_career_paths/)

Design, content, and creative professional roles:
- [ux_ui_designer.md](career/creative_career_paths/ux_ui_designer.md) ✅
- [graphic_designer.md](career/creative_career_paths/graphic_designer.md) ✅
- [content_writer.md](career/creative_career_paths/content_writer.md) ✅
- [digital_marketing_specialist.md](career/creative_career_paths/digital_marketing_specialist.md) ✅
- [video_producer.md](career/creative_career_paths/video_producer.md) ✅
- [brand_strategist.md](career/creative_career_paths/brand_strategist.md) ✅
- [event_planner.md](career/creative_career_paths/event_planner.md) ✅
- [executive_assistant.md](career/creative_career_paths/executive_assistant.md) ✅
- [digital_craft_business.md](career/creative_career_paths/digital_craft_business.md) ✅ (Etsy/maker with laser cutting, 3D printing, CNC)

#### Healthcare (Non-Tech) Careers
**Location**: [career/healthcare_career_paths/](career/healthcare_career_paths/)

Healthcare professional and administrative roles:
- [nurse_practitioner.md](career/healthcare_career_paths/nurse_practitioner.md) ✅
- [healthcare_administrator.md](career/healthcare_career_paths/healthcare_administrator.md) ✅
- [clinical_research_coordinator.md](career/healthcare_career_paths/clinical_research_coordinator.md) ✅
- [medical_device_sales.md](career/healthcare_career_paths/medical_device_sales.md) ✅

#### Finance & Sales Careers
**Location**: [career/finance_sales_career_paths/](career/finance_sales_career_paths/)

Finance, accounting, and sales professional roles:
- [financial_analyst.md](career/finance_sales_career_paths/financial_analyst.md) ✅
- [accountant_cpa.md](career/finance_sales_career_paths/accountant_cpa.md) ✅
- [sales_engineer.md](career/finance_sales_career_paths/sales_engineer.md) ✅
- [account_executive.md](career/finance_sales_career_paths/account_executive.md) ✅
- [customer_success_manager.md](career/finance_sales_career_paths/customer_success_manager.md) ✅

#### Vocational & Stepping-Stone Careers
**Location**: [career/vocational_career_paths/](career/vocational_career_paths/)

Entry-level careers that don't require 4-year degrees and serve as stepping stones to higher-level roles. These paths allow you to earn while you learn and gain practical experience:

**Technology Entry Points:**
- [help_desk_technician.md](career/vocational_career_paths/help_desk_technician.md) ✅ → IT Support → Systems Admin/Network Engineer
- [web_developer_bootcamp.md](career/vocational_career_paths/web_developer_bootcamp.md) ✅ (Bootcamp/self-taught) → Full Stack Developer
- [qa_tester.md](career/vocational_career_paths/qa_tester.md) ✅ (Manual testing) → QA Automation Engineer

**Business Entry Points:**
- [sales_development_rep.md](career/vocational_career_paths/sales_development_rep.md) ✅ (SDR) → Account Executive → Sales Manager
- [customer_support_rep.md](career/vocational_career_paths/customer_support_rep.md) ✅ → Customer Success Manager → Account Manager

**Healthcare Entry Points:**
- [medical_assistant.md](career/vocational_career_paths/medical_assistant.md) ✅ (Certificate) → LPN → RN → Nurse Practitioner
- [pharmacy_technician.md](career/vocational_career_paths/pharmacy_technician.md) ✅ (Certificate) → Pharmacy roles or healthcare admin

**Skilled Trades:**
- [electrician.md](career/vocational_career_paths/electrician.md) ✅ (Apprenticeship) → Journeyman → Master → Contractor
- [hvac_technician.md](career/vocational_career_paths/hvac_technician.md) ✅ (Apprenticeship) → Master Tech → Business Owner
- [automotive_technician.md](career/vocational_career_paths/automotive_technician.md) ✅ (Certificate/Trade School) → Master Tech → Shop Owner

**Professional Services:**
- [paralegal.md](career/vocational_career_paths/paralegal.md) ✅ (Certificate/Associate) → Senior Paralegal → Legal Operations

### Job Search & Resume Resources
**Location**: [career/job-search-strategist/](career/job-search-strategist/) & [career/resume-builder/](career/resume-builder/)

---

## 🔄 Workflows

**Location**: [workflows/](workflows/)

Multi-step workflow prompts for complex tasks:

### Slide Deck Workflow
**Location**: [workflows/slide_deck_workflow/](workflows/slide_deck_workflow/)

Four-step workflow for creating enterprise slide decks:
- [01_corporate_style_extractor.md](workflows/slide_deck_workflow/01_corporate_style_extractor.md) - Extract corporate style from existing presentations
- [02_corporate_style_applicator.md](workflows/slide_deck_workflow/02_corporate_style_applicator.md) - Apply extracted style to new content
- [03_enterprise_deck_architect.md](workflows/slide_deck_workflow/03_enterprise_deck_architect.md) - Architect comprehensive slide deck structure
- [04_deck_assemply_and_validation.md](workflows/slide_deck_workflow/04_deck_assemply_and_validation.md) - Assemble and validate final deck

**Time**: 2-4 hours | **Deliverable**: Complete enterprise slide deck ready for presentation

### Career Transition Workflow
**Location**: [workflows/career-transition/](workflows/career-transition/)

Four-step workflow for successful career transitions:
- [01_career_analysis.md](workflows/career-transition/01_career_analysis.md) - Career path selection and analysis
- [02_qualification_assessment.md](workflows/career-transition/02_qualification_assessment.md) - Detailed qualification assessment with personalized roadmap
- [03_resume_development.md](workflows/career-transition/03_resume_development.md) - Resume and professional materials creation
- [04_job_search_strategy.md](workflows/career-transition/04_job_search_strategy.md) - Strategic job search execution

**Time**: 4-6 hours setup + ongoing execution | **Timeline**: 3-12 months to job offer

---

## 🎯 Specialized Prompts

**Location**: [specialized/](specialized/)

Domain-specific utility prompts:

- **[@tutor](specialized/tutor-learning-assistant.md)** - AI tutor for personalized learning and skill development.
- **[@coach](specialized/coaching-session-builder.md)** - Creates structured coaching sessions with instructor guide, student manual, and quick reference. Builds from fundamentals to advanced with Socratic questioning.

---

## 💻 Development Prompts

**Location**: [development/](development/)

Software development and coding assistance prompts:

- **[vibe-coding/](development/vibe-coding/)** - Modern coding assistant focused on developer experience, clean code, and iterative development.

---

## 🎯 Strategy Prompts

**Location**: [strategy/](strategy/)

Strategic planning, evaluation, and decision-making prompts:

- **[ai-vendor-evaluation/](strategy/ai-vendor-evaluation/)** - Systematic framework for evaluating AI vendors, tools, and platforms with vendor-neutral analysis.

---

## 🛠️ Utilities

**Location**: [utilities/](utilities/)

Productivity tools and automation utilities:

### Home & Equipment Maintenance
- **[@equipment-doc](utilities/equipment-maintenance-documenter.md)** - Create comprehensive maintenance documentation for equipment, tools, appliances, vehicles, HVAC, and home systems. Works for renters and owners with climate-aware guidance.
- **[@maintenance-planner](utilities/household-maintenance-planner.md)** - Synthesize individual equipment docs into optimized household maintenance master schedule with task grouping, budget planning, and calendar optimization.

### Shopping & Gifts
- **[@giftfinder](utilities/giftfinder-shopping-assistant.md)** - Intelligent gift discovery assistant with recipient profiling, web search, and organized tracking for thoughtful gift-giving.

### Office Productivity
- **[excel-automation/](utilities/excel-automation/)** - Automate Excel spreadsheet creation, data manipulation, and formula generation.
- **[excel-editing/](utilities/excel-editing/)** - Expert assistance for editing existing Excel files, creating pivot tables, and advanced Excel features.

---

---

## 🚀 Usage Guidelines

### Using Prompts in Claude Code

Reference prompts using the @-mention syntax with mnemonics:
```
@architect help me design a data architecture
@tutor create a learning plan for Python
@giftfinder help me find a gift for my friend
```

Or reference the full path:
```
@ai-resources/prompts/documentation/arcdoc-documentation-architect.md review my docs
```

### Creating New Prompts

1. Use [@meta](meta/meta-prompt-engineer.md) to create high-quality prompts with systematic evaluation
2. Place prompts in the appropriate category folder
3. Update this README catalog when adding new prompts
4. Use consistent frontmatter with title, author, version, tags

### Prompt Maintenance

- **Versioning**: Update version numbers in frontmatter when making significant changes
- **Documentation**: Keep this README updated with new prompts
- **Organization**: Keep prompts organized by category for easy discovery

---

## 📊 Quick Reference

| Category | Count | Use Case |
|----------|-------|----------|
| Architecture | 6 ready + 3 templates | Data Vault, Cloud (AWS/Azure/GCP), API (REST/GraphQL/gRPC), Security (zero-trust), diagrams, requirements + reusable templates |
| Documentation | 4 | Project docs, business rules, meeting notes |
| Meta | 10 | **Setup** (@bootstrap), **Navigation** (@nav, @discover, Quick Start), prompt engineering, library management, patterns, agentic development |
| Career | 60 | Career planning across all industries: AI (16), Tech (8), Business (7), Creative (9), Healthcare (4), Finance/Sales (5), Vocational (11), plus analyzer & tools |
| Workflows | 5 | Multi-step processes (slide decks, career transition) |
| Specialized | 2 | Domain utilities (tutoring, coaching sessions) |
| Development | 1 | Coding assistance, clean code practices |
| Strategy | 1 | Vendor evaluation, strategic planning |
| Utilities | 5 | Home/equipment maintenance, Excel automation, gift shopping, productivity tools |
| **Total** | **93 ready + 3 templates** | Centralized general-purpose prompts + reusable templates + navigation tools |

---

## 🔗 Related Resources

- **Configuration**: [.ai/instructions.md](../../.ai/instructions.md) - Customize with your personal context
- **Additional Context**: [.ai/context.md](../../.ai/context.md) - Optional domain-specific context
- **Skills**: [ai-resources/skills/](../skills/) - Packaged skill files

---

*Last Updated: 2025-10-25 by Dan Brickey*
*Version v3.0.0: **Phase 5A Complete** - Enhanced Navigation & Discovery System. Created @discover (interactive prompt finder), Quick Start Guide (persona-based top picks), and upgraded @nav Navigator v2.0 with architecture expert routing and decision trees. Library now has comprehensive discovery tools to help users find the right prompt from 90+ options.*
