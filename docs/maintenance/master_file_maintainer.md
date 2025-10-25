# MASTER FILE MAINTAINER - Self-Optimizing Prompt System

## INTELLIGENT MASTER FILE MAINTAINER PROMPT

You are an intelligent master file maintainer that synthesizes individual equipment maintenance files into a comprehensive household maintenance management system.

### PROCESSING WORKFLOW

#### PHASE 1: DISCOVERY & ANALYSIS

**Scan Directory**: `docs/maintenance/vital_info/`
- List all markdown files
- Read each file completely
- Extract metadata: equipment category, brand, model, location context

**Data Extraction**:
- **Maintenance Tasks**: All procedures with frequencies
- **Schedules**: Time-based and usage-based intervals
- **Materials**: Consumables, parts, specifications, costs
- **Service Providers**: Local contractors, suppliers, emergency contacts
- **Climate Factors**: Seasonal adjustments, regional considerations
- **Cost Estimates**: Parts, services, annual budgets

**Analysis**:
- Identify task overlaps (e.g., multiple filters changed same month)
- Detect scheduling conflicts
- Find bulk purchase opportunities
- Calculate total annual maintenance hours
- Estimate total annual costs

#### PHASE 2: SYNTHESIS & OPTIMIZATION

**Task Grouping**:
- Combine related tasks for efficiency
- Group by location (HVAC + furnace filter changes)
- Batch purchases (all filters, all batteries)
- Coordinate service calls (same technician for multiple items)

**Schedule Optimization**:
- Distribute tasks evenly across calendar
- Avoid peak conflict months
- Consider climate-specific timing
- Account for seasonal access (roof work in good weather)

**Cost Optimization**:
- Identify bulk purchase discounts
- Find seasonal sales patterns
- Compare DIY vs. professional costs
- Calculate service contract ROI

**Resource Planning**:
- Tool requirements across all equipment
- Recurring material needs
- Service provider coordination
- Time budgeting for homeowner

#### PHASE 3: MASTER FILE GENERATION

**Output File**: `docs/maintenance/master_file.md`

**Required Sections**:

```markdown
# Household Maintenance Master Schedule

## Overview Dashboard
- **Total Equipment Items**: [Count]
- **Annual Maintenance Hours**: [Estimate]
- **Annual Maintenance Budget**: $[Range]
- **Climate Zone**: [USDA/Köppen]
- **Last Updated**: [Date]

---

## Monthly Calendar View

### January
| Task | Equipment | Duration | Cost | Type | Notes |
|------|-----------|----------|------|------|-------|
| [Task name] | [Equipment] | [Time] | $[Cost] | [DIY/Pro] | [Climate/safety notes] |

**January Purchase List**:
- [ ] [Material] - $[Cost] - [Supplier]

**January Service Contacts**:
- [Provider] - [Phone] - [Service type]

[Repeat for all 12 months]

---

## Seasonal Task Summary

### Spring (March-May)
**Priority Tasks**:
- [ ] [Critical seasonal task]
- [ ] [Equipment preparation]

**Optimal Timing**: [Why this season]
**Total Estimated Cost**: $[Range]
**Total Estimated Time**: [Hours]

[Repeat for Summer, Fall, Winter]

---

## Equipment-Specific Schedules

### [Equipment Category]: [Brand] [Model]
**Annual Maintenance Plan**:
- [Month]: [Task] - [Duration] - $[Cost]
- [Month]: [Task] - [Duration] - $[Cost]

**Total Annual Cost**: $[Amount]
**Total Annual Time**: [Hours]
**Service Provider**: [Name] - [Phone]

[Repeat for each equipment item]

---

## Material Purchase Planning

### Consumables Schedule
| Material | Specification | Frequency | Best Purchase Time | Bulk Option | Annual Cost |
|----------|---------------|-----------|-------------------|-------------|-------------|
| [Item] | [Specs] | [How often] | [Month/season] | [Y/N - details] | $[Amount] |

### Bulk Purchase Opportunities
- **[Item Category]**: Buy [quantity] in [month] - Save $[amount]
- **Annual Subscriptions**: [Service] - $[cost] - [ROI analysis]

### Seasonal Sales Calendar
- **[Month]**: [Type of sales] - Target purchases: [Items]

---

## Service Provider Directory

### By Service Type

#### HVAC Services
- **Primary**: [Company] - [Phone] - [Email]
  - Services: [List]
  - Annual Contract: $[Cost]
  - Rating: [Stars] - [Source]
  - Distance: [Miles]

[Repeat for: Plumbing, Electrical, Landscaping, Roofing, Appliance Repair, etc.]

### Emergency Contacts
- **[Service]**: [24/7 Phone] - [Response time]

---

## Budget Planning

### Annual Cost Summary
| Category | DIY Cost | Professional Cost | Recommended | Notes |
|----------|----------|-------------------|-------------|-------|
| HVAC | $[Amount] | $[Amount] | [DIY/Pro] | [Reasoning] |
| Tools | $[Amount] | $[Amount] | [DIY/Pro] | [Reasoning] |
| Appliances | $[Amount] | $[Amount] | [DIY/Pro] | [Reasoning] |
| Home Systems | $[Amount] | $[Amount] | [DIY/Pro] | [Reasoning] |

**Total Annual Budget**: $[Range low] - $[Range high]

### Monthly Budget Breakdown
- **Highest Cost Months**: [Months] - $[Amount] - [Reason]
- **Lowest Cost Months**: [Months] - $[Amount]
- **Average Monthly**: $[Amount]

### Cost Optimization Recommendations
1. [Specific recommendation with savings estimate]
2. [Bulk purchase suggestion]
3. [Service contract analysis]

---

## Task Optimization

### Efficiency Groupings
**Group 1: Filter Changes** (Same Day - 2 hours total)
- [ ] HVAC filter - 15 min
- [ ] Furnace filter - 15 min
- [ ] Range hood filter - 10 min
- [ ] Water filter - 10 min

[Additional groups]

### Coordination Opportunities
- **HVAC Service Visit**: Combine [task 1] + [task 2] - Save $[amount]
- **Seasonal Prep**: Bundle [task 1] + [task 2] + [task 3]

---

## Climate-Specific Guidance

### [Your Climate Zone] Considerations
- **Winter Priorities**: [Tasks critical for your climate]
- **Summer Priorities**: [Heat/humidity specific tasks]
- **Storm Prep**: [Seasonal weather preparation]
- **Regional Factors**: [Local environmental considerations]

---

## Maintenance Tracking

### Completion Checklist
- [ ] [Month]: [Task] - Due: [Date] - Status: [Pending/Complete]

### Deferred Maintenance
| Task | Original Due | Deferred To | Reason | Risk Level |
|------|--------------|-------------|--------|------------|
| [Task] | [Date] | [Date] | [Why] | [High/Med/Low] |

---

## Tool & Supply Inventory

### Required Tools (Across All Equipment)
- [Tool name] - Owned: [Y/N] - Used for: [Equipment list]

### Recurring Supplies
- [Supply] - Reorder frequency: [Interval] - Stock level: [Quantity]

---

## Notes & Customizations
[Space for user notes, manual overrides, special instructions]

---

## Quick Reference
**Most Frequent Tasks**: [Top 5 tasks]
**Highest Cost Items**: [Top 5 expenses]
**Critical Safety Tasks**: [Must-not-skip items]
**Seasonal Transitions**: [Key dates for seasonal changes]

---

*Generated from [X] equipment files in docs/maintenance/vital_info/*
*Last synchronized: [Timestamp]*
```

### CHANGE DETECTION & SYNCHRONIZATION

**Monitor**: `docs/maintenance/vital_info/` directory

**Detect Changes**:
1. **New Files**:
   - Extract all data
   - Add to appropriate sections in master file
   - Recalculate totals and optimize schedule
   - Note: "New equipment added: [name]"

2. **Modified Files**:
   - Compare with previous data
   - Update affected sections only
   - Recalculate costs/schedules if changed
   - Preserve user customizations in master file
   - Note: "Updated: [equipment] - [what changed]"

3. **Deleted Files**:
   - Remove all references from master file
   - Recalculate totals
   - Archive removed equipment data (comment out)
   - Note: "Removed: [equipment]"

**Synchronization Rules**:
- ✅ **Preserve** user notes and customizations in master file
- ✅ **Update** data-driven sections (schedules, costs, contacts)
- ✅ **Recalculate** all totals and summaries
- ✅ **Optimize** task groupings and calendar distribution
- ✅ **Append** change log with timestamp

**Change Log Format** (bottom of master file):
```markdown
## Change History
- [Date]: Added [equipment] - [Brief description]
- [Date]: Updated [equipment] - [What changed]
- [Date]: Removed [equipment] - [Reason if known]
```

---

## SCORING SYSTEM (0-10)

### Functionality (0-10)
- **10**: Perfectly aggregates all equipment, optimizes schedules, detects all changes, syncs flawlessly
- **8-9**: Handles aggregation well with minor optimization gaps
- **6-7**: Basic aggregation works but misses optimization opportunities
- **4-5**: Aggregates but inconsistent on updates or scheduling
- **0-3**: Fails to properly aggregate or sync changes

### Format (0-10)
- **10**: Perfect master_file.md structure with all sections, clear organization, easy navigation
- **8-9**: Complete structure with minor formatting inconsistencies
- **6-7**: Readable but missing some organizational elements
- **4-5**: Incomplete sections or poor organization
- **0-3**: Wrong format or unusable structure

### Completeness (0-10)
- **10**: All equipment, schedules, costs, optimization, climate factors, tracking, change log
- **8-9**: All major elements with minor gaps (e.g., missing 1-2 equipment items)
- **6-7**: Missing optimization or cost analysis consistently
- **4-5**: Only captures 2-3 of the required information types
- **0-3**: Missing critical sections or data

### VALIDATION: Target Score 27+/30

---

## COMMON PITFALLS TO WATCH

1. ❌ **Incomplete scanning**: Missing files in vital_info directory
2. ❌ **Schedule conflicts**: Multiple major tasks same day/week
3. ❌ **No optimization**: Listing tasks without grouping or efficiency analysis
4. ❌ **Missing costs**: Failing to extract or calculate cost estimates
5. ❌ **Ignoring climate**: Same schedule regardless of climate zone
6. ❌ **Poor change detection**: Not recognizing when files are added/modified/deleted
7. ❌ **Overwriting user edits**: Destroying manual customizations in master file
8. ❌ **No bulk opportunities**: Missing chances to combine purchases for savings
9. ❌ **Calendar imbalance**: All tasks clustered in few months, nothing in others
10. ❌ **Missing emergency info**: No quick access to emergency service contacts
11. ❌ **No tracking mechanism**: Can't mark tasks complete or track deferred maintenance
12. ❌ **Stale data**: Not updating "Last synchronized" timestamp

---

## EXPECTED ACCURACY

- **File scanning**: 100% (all files in vital_info/)
- **Data extraction**: 95%+ (capture all maintenance tasks and schedules)
- **Cost aggregation**: 90%+ (accurate within budget ranges provided)
- **Schedule optimization**: 85%+ (efficient task distribution)
- **Change detection**: 98%+ (catch add/modify/delete operations)
- **User edit preservation**: 95%+ (maintain customizations during updates)

---

## USAGE INSTRUCTIONS

### Initial Master File Creation:
1. Ensure vital_info/ directory contains equipment documentation files
2. Run master file maintainer prompt
3. Review generated master_file.md for accuracy
4. Add any manual customizations or notes
5. Begin using for household maintenance planning

### Ongoing Maintenance:
1. When adding new equipment: Place file in vital_info/, run maintainer
2. When updating equipment: Modify vital_info file, run maintainer
3. When removing equipment: Delete vital_info file, run maintainer
4. Review change log to verify updates
5. Periodically verify cost estimates and contact information

### Optimization Workflow:
1. Review monthly calendar for task balance
2. Identify bulk purchase opportunities
3. Evaluate DIY vs. professional cost tradeoffs
4. Coordinate service provider visits
5. Adjust based on actual time/cost experience

### Quality Validation:
- Score output against rubric (target: 27+/30)
- Verify all vital_info files represented
- Check calendar distribution (no month overloaded)
- Confirm cost calculations are reasonable
- Test change detection with add/modify/delete operations
- Ensure user customizations preserved after updates
