# 🚀 Quick Reference Card - Resume Specialist Agent

**Version:** 2.0 | **Status:** Production Ready | **Updated:** 3 May 2026

---

## What It Does (30-Second Overview)

```
Raw CV Input → Scoring (0-100) → Europpass-Compliant Output
              ↓
         Analyzes: Content quality, structure, tone, evidence
         Detects: Seniority level, business impact, career progression
         Outputs: Quality score + improvements + PDF-ready CV
```

---

## Quick Start: 3 Steps

### Step 1: Load Context
```
Load: .github/agents/resume-generator.agent.md
Also load: 
  - cv-scoring-system.json
  - senior-level-positioning.json
  - business-impact-framework.json
```

### Step 2: Input
```
Provide raw CV or candidate data with:
- Work experience (dates, titles, companies, responsibilities)
- Key achievements/accomplishments (with any metrics available)
- Education & certifications
- Technical skills with proficiency levels
- Languages
```

### Step 3: Output
```
Receive:
- Quality Score (0-100%)
- Dimension Breakdown (6 scoring categories)
- Top 3 Improvement Recommendations
- Transformation Report (what changed & why)
- Europass-Compliant CV (1-2 pages)
```

---

## Score Meaning (What to Do)

| Score | Action | Timeline |
|-------|--------|----------|
| 90-100 | ✅ Submit immediately | Ready now |
| 80-89 | ✅ Review suggestions optional | Ready in 1 day |
| 70-79 | 🔄 Apply improvements | 2-3 days |
| 60-69 | 🛠️ Collect actionable items | 3-5 days |
| <60 | 🚨 Major overhaul needed | 1 week |

---

## Scoring Dimensions (Know Your Weaknesses)

| Dimension | Max | What It Scores |
|-----------|-----|---|
| Content Quality | 35 | Strategic depth, metrics, business impact |
| Structure | 20 | Hierarchy, chronology, completeness |
| Tone | 15 | Professionalism, buzz word removal |
| Evidence | 15 | Quantification, proof points |
| Completeness | 10 | All sections present |
| Formatting | 10 | Dates, spelling, ATS readiness |

---

## Common Low-Score Problems & Fixes

| Problem | Score Impact | Fix |
|---------|---|---|
| ❌ "Responsible for testing" | -15 pts | ✅ Add metric: "Reduced defects 8% to 2%" |
| ❌ "Led team" | -15 pts | ✅ Add scope: "Supervised 5-person QA team" |
| ❌ No scale context | -20 pts | ✅ Add: "500K+ users, $2.5B transactions" |
| ❌ "Passionate engineer" | -10 pts | ✅ Remove buzz word, add achievement |
| ❌ Mixed date formats | -5 pts | ✅ Use DD/MM/YYYY format consistently |

---

## Real Example: Score Before/After

### BEFORE (Raw Input)
```
Responsible for regression testing
Developed PHP automation 
Supported release cycles
Created test documentation

Skills: PHP, SQL, JIRA, HP ALM
```
**Score: 45%** 🚨 Weak

### AFTER (Enhanced)
```
Reduced defect escape rate 8% → 2% via risk-based regression strategy
Built PHP automation suite (250+ cases); cut manual effort 80h → 12h per release
Standardized QA templates; reduced defect resolution time 8d → 2d
Achieved 99.95% payroll data accuracy; prevented 28 post-release data issues

Technical Skills:
Core (10+ years): PHP, SQL, HP ALM automation
Specialized: COBOL mainframe testing, PCI-DSS audit validation
```
**Score: 98%** ⭐ Excellent

**Improvement: +53 points (45% → 98%)**

---

## For Different Users

### I'm a Recruiter
```
1. Upload raw CV
2. Check score
   → If ≥75: Schedule interview
   → If <75: Send improvement suggestions to candidate
3. Candidate revises and resubmits
4. Score again
5. Export PDF when ready
```

### I'm a Candidate
```
1. Input raw CV data
2. Review score + top 3 improvements
3. Update CV with suggestions
4. Get rescore
5. Repeat until score ≥80+
6. Submit to employers
```

### I'm an HR Manager
```
1. Batch load 50+ CVs
2. Score all at once
3. Sort by score
4. Prioritize 80+ scores for interviews
5. Coach candidates <75 using improvement suggestions
```

---

## Key Frameworks Explained

### 1. Scoring System (cv-scoring-system.json)
- Calculates 0-100 quality score
- Weights: Content 33%, Structure 19%, Tone 14%, Evidence 14%, Completeness 10%, Formatting 10%
- Use: Understand what's weak and why

### 2. Senior Positioning (senior-level-positioning.json)
- Detects seniority level automatically
- Auto-enhances with strategic achievements if 7+ years
- Maps to: IC, Senior IC, Lead, Director roles
- Use: Ensures senior CVs are positioned correctly

### 3. Business Impact (business-impact-framework.json)
- 5 impact categories: Revenue/Cost, Efficiency, Risk, Quality, Leadership
- Provides metric templates and examples
- Use: Help quantify achievements with real numbers

### 4. Achievement Blocks (achievement-blocks-preset.json)
- Optional organizing labels for achievements
- Examples: "Automation Architecture", "Compliance & Risk", "Performance"
- Use: Add theme headers when needed (optional)

---

## What It Fixes Automatically

✅ **Buzzword Removal**
- "Passionate" ❌ → evidence-based statement ✅
- "Rockstar" ❌ → specific achievement ✅
- "Thinking outside the box" ❌ → concrete example ✅

✅ **Date Formatting**
- 05/15/2024 ❌ → 15 May 2024 ✅

✅ **First-Person Removal**
- "I designed..." ❌ → "Designed..." ✅

✅ **GDPR Compliance**
- Age ❌ → Removed
- Photo ❌ → Removed
- Marital status ❌ → Removed

✅ **Structure Normalization**
- Roles now in reverse chronological order
- Clear section hierarchy
- Consistent bullet formatting

---

## Golden Rules for High Scores (90+)

1. **Every achievement has a metric**
   ```
   ❌ "Improved performance"
   ✅ "Reduced latency from 500ms to 150ms (70% improvement)"
   ```

2. **Every role includes scale context**
   ```
   ❌ "Managed QA testing"
   ✅ "Managed QA for HRIS serving 500+ clients, 200K+ users"
   ```

3. **Show progression (if multiple roles)**
   ```
   ❌ Same level across 10 years
   ✅ IC (2013) → Senior IC (2016) → Lead (2019) → Director (2022)
   ```

4. **Prove senior leadership (if claiming seniority)**
   ```
   ❌ "Senior" in title only
   ✅ Mentored 4 engineers; 2 promoted; established standards adopted across org
   ```

5. **Quantify everything**
   ```
   ❌ Metrics: Cost saved, time, users, defects, revenue
   ✅ Numbers: Percentages, growth rates, before/after comparisons
   ```

---

## Framework Files Location Reference

```
Framework Hearts:
  .github/agents/framework-enhancements/
    ├── cv-scoring-system.json ← Core scoring algorithm
    ├── senior-level-positioning.json ← Seniority detection
    ├── business-impact-framework.json ← Impact quantification
    └── achievement-blocks-preset.json ← Organization labels

Always Load:
  .github/agents/resume-generator.agent.md ← Complete spec

Reference Examples:
  .github/agents/improved-cv-examples/
    ├── nadine-tolentino-2026-improved-v3.md ← 98% score example
    └── patrick-tolentino-2026-improved-v2.md ← Senior example
```

---

## Troubleshooting

| Issue | Cause | Fix |
|-------|-------|-----|
| Score is 45% | No metrics in CV | Add numbers: defects prevented, time saved, revenue impact |
| Score is 65% | Responsibilities not achievements | Reframe each as outcome: "achieved X by doing Y with impact Z" |
| Score is 75% | Missing scale context | Add: How many users/systems/transactions? What was the business criticality? |
| Score is 85% | Missing one dimension | Review all 6 categories; identify weakest (usually Evidence or Content Quality) |
| Can't get above 95% | Very minor issues | Perfect scores (100%) rare; 95% is excellent |

---

## Success Criteria

| Role Level | Target Score | Status |
|------------|---|---|
| **Entry** (0-3 yrs) | 70-79 | Acceptable |
| **Mid** (3-7 yrs) | 80-89 | Strong |
| **Senior** (7+ yrs) | 85-100 | Strong to Excellent |
| **Director** (10+ yrs) | 90-100 | Excellent |

---

## One-Minute Test

1. Load agent with `resume-generator.agent.md`
2. Use Nadine Tolentino's raw input (from `ANALYSIS_NADINE_CV_GAPS.md`)
3. Run scoring → Should get ~61% initially
4. Apply improvements → Should reach ~98% (v3 version)
5. Verify: Score breakdown makes sense?

✅ **If yes, agent is working correctly**

---

## Need More Help?

- **Why a score:** Read `CV_SCORING_GUIDE.md` (550 lines, detailed)
- **What was built:** Read `IMPLEMENTATION_STATUS.md` (369 lines, technical)
- **How to use:** Read `QUICK_START_GUIDE.md` (390 lines, user-friendly)
- **Complete spec:** Read `.github/agents/resume-generator.agent.md` (2,000+ lines, exhaustive)

---

**Quick Ref Version:** 2.0  
**Last Updated:** 3 May 2026  
**Status:** ✅ Production Ready


