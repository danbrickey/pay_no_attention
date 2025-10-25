---
title: "Documentation Index - AI Resources Ecosystem"
author: "Dan Brickey"
version: "1.0.0"
last_updated: "2025-10-25"
category: "documentation-index"
purpose: "Master index for discovering and navigating all documentation in the docs/ folder"
usage: "AI-optimized navigation for finding technical docs, guides, and reference materials"
---

# Documentation Index

This is the master index for all documentation in the `docs/` folder. This index is designed to help both humans and AI assistants quickly discover relevant documentation.

## Quick Navigation by Intent

| What I Need | Where to Look |
|-------------|---------------|
| Gift recipient profiles | [gift-profiles/](gift-profiles/) |
| Documentation taxonomy/classification | [taxonomy.md](taxonomy.md) |

## Index by Document Type

### Reference Guides
Currently empty - reference documentation will be indexed here

### Process Guides
Currently empty - process documentation will be indexed here

### Technical Specifications
Currently empty - technical specs will be indexed here

### Personal Knowledge Base

#### Gift Management
- **[Gift Profiles](gift-profiles/)** - Recipient profiles for thoughtful gift selection
  - [profile-index.md](gift-profiles/profile-index.md) - Index of all gift recipient profiles
  - [profile-template.md](gift-profiles/profile-template.md) - Template for creating new profiles
  - [README.md](gift-profiles/README.md) - Overview of gift profile system

## Index by Category

### Personal Productivity
- [gift-profiles/](gift-profiles/) - Gift recipient profile management

---

## How to Use This Index

### For Humans
Browse by intent, document type, or category to find what you need. Each entry links to the actual documentation.

### For AI Assistants
1. **Start here** when users ask "Where's the info on X?" or "Do we have docs for Y?"
2. Use "Quick Navigation by Intent" to match user questions to documentation
3. Fall back to category/type browsing when intent is unclear
4. When creating new documentation, **register it here** in all relevant sections

---

## Maintenance Instructions

**When creating new documentation** (applies to all documentation-generating prompts):

1. **Add to Quick Navigation by Intent** (if applicable)
   - Add row with user's likely question → path to docs
   - Make intent descriptions user-friendly

2. **Add to Index by Document Type**
   - Place in appropriate type section with description
   - Link to the file with brief purpose statement

3. **Add to Index by Category**
   - Organize by primary topic/domain
   - Group related docs together

4. **Update version and last_updated** in frontmatter above

5. **Consider updating taxonomy.md** if new classification terms needed

---

## Related Resources

- **[taxonomy.md](taxonomy.md)** - Controlled vocabulary for documentation classification
- **Prompts that create docs**:
  - [@arcdoc](../ai-resources/prompts/documentation/arcdoc-documentation-architect.md) - Architecture documentation
  - [@projdoc](../ai-resources/prompts/documentation/projdoc-expert.md) - Project documentation
  - [@bizrules](../ai-resources/prompts/documentation/bizrules-documenter.md) - Business rules documentation

---

*This index is maintained by documentation-generating prompts and should be updated whenever new documentation is created.*
