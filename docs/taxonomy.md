---
title: "Documentation Taxonomy"
author: "Dan Brickey"
version: "1.0.0"
last_updated: "2025-10-25"
category: "documentation-classification"
purpose: "Controlled vocabulary for classifying and organizing documentation"
usage: "Reference this when creating documentation frontmatter to ensure consistent classification"
---

# Documentation Taxonomy

This taxonomy provides controlled vocabulary for classifying documentation. Use these terms in frontmatter metadata to ensure consistent organization and discoverability.

## Document Types

### Primary Types
- `reference-guide` - Reference documentation for APIs, tools, languages, or frameworks
- `process-guide` - Step-by-step process or workflow documentation
- `technical-spec` - Technical specifications and design documents
- `architecture-doc` - Architecture diagrams, patterns, and design decisions
- `business-rules` - Business logic, domain rules, and decision tables
- `meeting-notes` - Meeting summaries and action items
- `how-to-guide` - Practical how-to instructions
- `concept-guide` - Conceptual explanations and learning materials
- `troubleshooting` - Problem-solving and debugging guides
- `profile` - Personal profiles (gift recipients, personas, etc.)

### Meta Types
- `index` - Index or catalog documents
- `template` - Templates for creating other documents
- `taxonomy` - Classification and vocabulary definitions

## Categories (Primary Organization)

### Technical Categories
- `architecture` - System architecture and design
- `data-architecture` - Data modeling, Data Vault, dimensional models
- `development` - Software development and coding
- `infrastructure` - Infrastructure, DevOps, deployment
- `testing` - Testing strategies and test documentation
- `security` - Security policies, practices, and guidelines

### Business Categories
- `business-analysis` - Business requirements and analysis
- `domain-knowledge` - Business domain expertise and rules
- `strategy` - Strategic planning and decision-making
- `process` - Business processes and workflows

### Personal Categories
- `personal-productivity` - Personal productivity tools and systems
- `career` - Career development and planning
- `learning` - Learning materials and educational content

### Meta Categories
- `documentation-system` - Documentation about documentation
- `library-management` - AI resources library organization

## Audience Types

Use these in `audience:` frontmatter field:

- `executives` - C-level executives and senior leadership
- `business-stakeholders` - Business owners and decision-makers
- `architects` - System and data architects
- `engineers` - Software engineers and developers
- `data-engineers` - Data engineers and ETL developers
- `analysts` - Business analysts and data analysts
- `technical-leads` - Tech leads and engineering managers
- `all-technical` - All technical staff
- `all-business` - All business staff
- `everyone` - General audience

## Status Values

Use these in `status:` frontmatter field:

- `active` - Current, actively maintained documentation
- `draft` - Work in progress, not yet finalized
- `review` - Under review, pending approval
- `archived` - No longer current but kept for reference
- `deprecated` - Superseded by newer documentation
- `experimental` - Experimental or exploratory content

## Complexity Levels

Use these in `complexity:` frontmatter field (optional):

- `basic` - Introductory, suitable for beginners
- `intermediate` - Requires some background knowledge
- `advanced` - For experts or deep technical dive

## Common Tags

### Technical Topics
- `data-vault-2.0` - Data Vault 2.0 methodology
- `dimensional-modeling` - Kimball dimensional modeling
- `medallion-architecture` - Medallion/lakehouse architecture
- `snowflake` - Snowflake platform
- `etl` - Extract, Transform, Load processes
- `api` - API documentation
- `database-design` - Database design patterns
- `cloud` - Cloud technologies
- `cicd` - CI/CD and automation

### Business Domains
- `broker` - Producer/broker domain
- `claims` - Claims processing domain
- `financial` - Financial/billing domain
- `membership` - Member enrollment domain
- `product` - Product/plan domain
- `provider` - Provider network domain

### Documentation Concerns
- `getting-started` - Onboarding and getting started
- `best-practices` - Best practices and guidelines
- `patterns` - Design patterns and solutions
- `anti-patterns` - Things to avoid
- `troubleshooting` - Debugging and problem-solving
- `migration` - Migration guides
- `reference` - Quick reference material

### Personal Tags
- `gift-giving` - Gift selection and recipient profiles
- `productivity` - Productivity tools and techniques

## Usage in Frontmatter

### Example: Technical Architecture Doc

```yaml
---
title: "Multi-Tenant Data Vault Design Pattern"
author: "Dan Brickey"
version: "1.0.0"
last_updated: "2025-10-25"
document_type: "architecture-doc"
category: "data-architecture"
tags: ["data-vault-2.0", "multi-tenant", "patterns", "best-practices"]
status: "active"
audience: ["architects", "data-engineers", "technical-leads"]
complexity: "advanced"
related_docs: ["data-vault-overview.md", "medallion-architecture.md"]
---
```

### Example: Business Rules Doc

```yaml
---
title: "Claims Adjudication Business Rules"
author: "Dan Brickey"
version: "2.1.0"
last_updated: "2025-10-25"
document_type: "business-rules"
category: "domain-knowledge"
tags: ["claims", "business-rules", "adjudication", "reference"]
status: "active"
audience: ["business-stakeholders", "analysts", "all-technical"]
business_domain: "claims"
related_docs: ["claims-workflow.md"]
---
```

### Example: Personal Profile

```yaml
---
title: "Sarah - Gift Recipient Profile"
author: "Dan Brickey"
version: "1.0.0"
last_updated: "2025-10-25"
document_type: "profile"
category: "personal-productivity"
tags: ["gift-giving", "recipient-profile"]
status: "active"
audience: ["personal"]
profile_type: "gift-recipient"
---
```

## Extending the Taxonomy

When you need a term that doesn't exist:

1. **Check for similar terms first** - Can an existing term work?
2. **Propose new term** - Add it to appropriate section with definition
3. **Update documentation-index.md** - Ensure new docs are discoverable
4. **Use consistently** - Apply new term across related documentation
5. **Document rationale** - Note why new term was needed

---

## Maintenance

This taxonomy should evolve as documentation needs grow. When proposing changes:

- Keep terms specific enough to be useful, general enough to apply broadly
- Avoid creating too many overlapping terms
- Prioritize discoverability - would someone search for this term?
- Consider both human and AI assistant usage patterns

---

*This taxonomy is referenced by documentation-generating prompts to ensure consistent classification.*
