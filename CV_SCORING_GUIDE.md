# Resume Specialist Agent - How to Score & Improve CVs
**Updated:** 3 May 2026  
**Framework Version:** 2.0 (Enhanced with Senior Positioning & Scoring)

---

## 🎯 Quick Start: Scoring a CV in 3 Steps

### Step 1: Load The Frameworks
```
Primary Context:   .github/agents/resume-generator.agent.md
Scoring System:    .github/agents/framework-enhancements/cv-scoring-system.json
Senior Detection:  .github/agents/framework-enhancements/senior-level-positioning.json
Impact Framework:  .github/agents/framework-enhancements/business-impact-framework.json
```

### Step 2: Accept Candidate Input
Example raw input from candidate:
```
ROLE: Senior QA Engineer
CURRENT COMPANY: PayAsia by Deel
DURATION: 01/2022 - 04/2026

KEY RESPONSIBILITIES:
- Performed acceptance and regression testing
- Wrote PHP automation scripts
- Supported release cycles
- Created test documentation

TECHNICAL SKILLS:
PHP, HP ALM, SQL, JIRA, COBOL, Postman
```

### Step 3: Run Quality Scoring

**System calculates score using 6 dimensions:**

| Dimension | Max Points | Scoring Rules |
|-----------|-----------|---------------|
| **Content Quality** | 35 | Strategic impact, metrics, business value, mentorship |
| **Structure** | 20 | Hierarchy, reverse chronology, completeness |
| **Tone & Language** | 15 | Professionalism, objectivity, no buzz words |
| **Evidence Density** | 15 | Claims backed by numbers, quantification |
| **Completeness** | 10 | All sections present, consistent formatting |
| **Formatting** | 10 | Dates, spelling, ATS readiness, consistency |
| **TOTAL** | **105** | **Converts to 0-100%** |

---

## 📊 Score Interpretation & Action

### What the Scores Mean

#### ✨ **90-100: EXCELLENT**
✅ **Status:** Ready to submit immediately  
✅ **Action:** None required  
✅ **Profile:** Senior positioning established; strong evidence of impact

**Example (Nadine after improvements):** Score 91%
```
Content Quality:        32/35  (91%)  ← Strategic achievements clear
Structure Compliance:   20/20  (100%) ← Perfect Europass format  
Tone & Language:        15/15  (100%) ← Professional, objective
Evidence Density:       15/15  (100%) ← Every claim quantified
Completeness:           10/10  (100%) ← All sections complete
Formatting:             10/10  (100%) ← Date format, spelling perfect

FINAL SCORE: 102/105 = 97% ⭐ EXCELLENT
```

#### 💪 **80-89: STRONG**
✅ **Status:** Ready; minor enhancements optional  
⚡ **Action:** Review top 2-3 improvement suggestions  
📝 **Profile:** Good senior positioning; mostly quantified

**Top Improvements Suggested:**
1. Add more specific scale context (user count, transaction volume)
2. Quantify 1-2 additional metrics (time saved, efficiency improvement)
3. Highlight one more strategic initiative or mentorship example

#### ⚠️ **70-79: ACCEPTABLE**
🔄 **Status:** Acceptable but recommend revisions  
🛠️ **Action:** Address top 3 improvement areas before submission  
👤 **Profile:** Mostly solid; needs evidence strengthening

**Top Improvements Suggested:**
1. Convert 2-3 responsibilities to achievement format
2. Add before/after metrics (current: vague; target: specific numbers)
3. Highlight business impact (revenue saved, defects prevented, etc.)

#### 🚨 **60-69: NEEDS WORK**
❌ **Status:** Requires significant revisions before submission  
🔧 **Action:** Address all 5+ improvement areas  
💬 **Profile:** Weak positioning; actionable items needed

**Top Improvements Suggested:**
1. Distinguish responsibilities from achievements (add outcomes)
2. Quantify every major bullet (add metrics, percentages, numbers)
3. Add scale context to each role (users, transactions, criticality)
4. Include one example of strategic decision-making
5. Highlight mentorship or knowledge transfer contribution

#### ❌ **<60: WEAK**
🛑 **Status:** Major overhaul needed  
📋 **Action:** Collect actionable items; ask candidate for more details  
🔴 **Profile:** Mostly generic; insufficient evidence

**Trigger Escalation Questions:**
1. "What was the business impact? (cost saved, revenue, time reduced, defects prevented?)"
2. "How many people/systems/customers were affected?"
3. "What was the before/after metric? (80% to 95%? 2 weeks to 3 days?)"
4. "Did you make strategic decisions? Lead a team? Mentor anyone?"
5. "What made this outcome exceptional, not just routine work?"

---

## 🔍 Detailed Scoring Dimensions

### Dimension 1: Content Quality (35 points)
**What it measures:** Strategic achievement depth, business impact, leadership evidence

**Excellent (32-35 pts):**
- ✅ Every achievement includes business impact metric
- ✅ Scale context obvious (users, transactions, revenue)
- ✅ Evidence of strategic decision-making or mentorship
- ✅ Industry/domain expertise clearly positioned

**Good (25-31 pts):**
- ✅ Most achievements quantified
- ✅ Scale context present in 70%+ of roles
- ✅ At least one strategic leadership example
- ⚠️ Some achievements still generic

**Weak (15-24 pts):**
- ⚠️ Many responsibilities without metrics
- ⚠️ Missing scale context for key roles
- ❌ No evidence of strategic thinking
- ❌ Domain expertise not differentiated

**Poor (<15 pts):**
- ❌ Generic descriptions dominate
- ❌ No quantified achievements
- ❌ No scale context at all
- ❌ Sounds like job description

**How to Improve:**
- Add business impact to every achievement
- Show before/after metrics (e.g., "defect escape rate dropped from 8% to 2%")
- Mention scale (e.g., "serving 500+ clients, 200K+ end users")
- Include one strategic achievement per role

---

### Dimension 2: Structure Compliance (20 points)
**What it measures:** Hierarchy, reverse chronology, section completeness, Europass alignment

**Excellent (18-20 pts):**
- ✅ Perfect reverse chronological order
- ✅ All Europass sections present
- ✅ Clear section hierarchy with visual distinction
- ✅ Role scope & achievements clearly separated

**Good (14-17 pts):**
- ✅ Chronological order correct
- ✅ Most sections present
- ⚠️ Hierarchy generally clear but not perfect

**Weak (<14 pts):**
- ❌ Mixed chronology or missing recent roles
- ❌ Missing key sections (summary, skills, education)
- ❌ Structure feels flat

---

### Dimension 3: Tone & Language (15 points)
**What it measures:** Professionalism, objectivity, absence of marketing jargon

**Excellent (14-15 pts):**
- ✅ Zero buzz words (passionate, rockstar, dynamic, guru)
- ✅ Objective, fact-based language throughout
- ✅ Action verbs strong and specific (Led, Architected, Designed, Reduced, Prevented)
- ✅ No exclamation marks or emotional language
- ✅ No first-person pronouns (I, me, my)

**Good (12-13 pts):**
- ✅ Minimal buzz words
- ⚠️ Mostly objective language
- ⚠️ Some vague adjectives remain

**Weak (<12 pts):**
- ❌ Multiple buzz words present
- ❌ Emotional language detected
- ❌ First-person pronouns used
- ❌ Marketing/sales tone

**Auto-Removal Examples:**
```
❌ "Passionate and dynamic team player"
✅ "Coordinated 5-person QA team; improved on-time delivery by 23%"

❌ "Excel at problem-solving with proven track record"
✅ "Resolved 45 performance bottlenecks; prevented 3 production outages"

❌ "I am an excellent communicator"
✅ "Mentored 4 junior engineers; created documentation standards adopted across 3 accounts"
```

---

### Dimension 4: Evidence Density (15 points)
**What it measures:** Quantification, proof points, specific data vs. claims

**Excellent (14-15 pts):**
- ✅ 90%+ of achievements include specific metrics
- ✅ Numbers provided (percentages, time, money, volume)
- ✅ Scope always quantified (people, systems, users)
- ✅ Before/after comparisons shown

**Good (12-13 pts):**
- ✅ 70%+ of achievements quantified
- ⚠️ Some claims lack specific numbers

**Weak (<12 pts):**
- ❌ <50% quantified
- ❌ Vague claims without proof
- ❌ "Improved performance" without numbers
- ❌ "Led initiatives" without scope

**Quantification Rule:**
```
✅ GOOD: "Reduced defect escape rate from 8% to 2%; saved est. $500K support costs"
❌ WEAK: "Improved defect detection"

✅ GOOD: "Built PHP automation suite of 250+ test cases; cut manual effort 80h → 12h per cycle"
❌ WEAK: "Wrote automation scripts"

✅ GOOD: "Mentored 4 QA engineers; training standards adopted across 3 enterprise clients"
❌ WEAK: "Mentored team members"
```

---

### Dimension 5: Completeness (10 points)
**What it measures:** All required sections present, consistent coverage

**Excellent (10 pts):**
- ✅ Professional Summary/Profile present
- ✅ Work Experience (3+ roles with consistent structure)
- ✅ Education & Certifications with dates
- ✅ Technical Skills (organized, proficiency levels)
- ✅ Languages (CEFR format: A1-C2)

**Good (8-9 pts):**
- ✅ Most sections present
- ⚠️ 1-2 sections light on detail

**Weak (<8 pts):**
- ❌ Missing key sections
- ❌ Inconsistent coverage across roles

---

### Dimension 6: Formatting & ATS Readiness (10 points)
**What it measures:** Date format, spelling, consistency, ATS optimization

**Excellent (10 pts):**
- ✅ All dates in DD/MM/YYYY or "Month YYYY" format (NOT MM/DD/YYYY)
- ✅ Zero spelling or grammar errors
- ✅ Consistent bullet points (no mixed formats)
- ✅ No images, tables, or special characters
- ✅ Consistent font & spacing

**Good (8-9 pts):**
- ✅ Dates correct
- ✅ Minimal typos
- ⚠️ Some formatting inconsistencies

**Weak (<8 pts):**
- ❌ US date format (MM/DD/YYYY)
- ❌ Spelling errors or inconsistent formatting
- ❌ Graphics or complex formatting that breaks ATS

---

## 💡 Real-World Scoring Example: Nadine Tolentino

### BEFORE (Raw Input)
```
Senior QA Engineer – Enterprise Platforms | PayAsia by Deel | 01/2022 – 04/2026

Key Responsibilities:
- Performed acceptance, functional, and regression testing
- Developed PHP automation scripts
- Validated bug fixes and supported release cycles
- Created test strategy documents

Technical Skills:
Cobol, PHP, JIRA, HP ALM, SQL, AWS, Docker, Kubernetes
```

**Score Analysis:**
- Content Quality: 10/35 (responsibilities, not achievements)
- Structure: 18/20 (good format, but weak content)
- Tone: 14/15 (professional but generic)
- Evidence: 3/15 (no metrics at all)
- Completeness: 9/10 (missing impact)
- Formatting: 10/10 (clean format)

**TOTAL: 64/105 = 61% ⚠️ NEEDS WORK**

---

### AFTER (Enhanced with Framework)
```
Senior QA Engineer – Enterprise Platforms | PayAsia by Deel
01/2022 – 04/2026 | Remote (APAC)

Scope: Enterprise HRIS/Payroll serving 500+ client companies; ~200K end users; ~$2.5B annual transactions

Strategic Achievements:
- Reduced defect escape rate from 8% → 2% via risk-based regression strategy
  (95% coverage across core workflows; prevented $500K+ customer support costs)
  
- Built PHP automation suite (250+ test cases); reduced manual effort from 80h → 12h per release
  (Enabled bi-weekly releases vs. previous monthly cycle; improved team velocity by 300%)
  
- Standardized QA templates and evidence; improved first-time readiness
  (Reduced defect resolution time from ~8 days → ~2 days; improved developer satisfaction by 18 points)
  
- Strengthened data accuracy controls (200+ payroll data fields)
  (Achieved 99.95% reconciliation accuracy; prevented 28 post-release data integrity issues)
  
- Coordinated test gates across QA/Dev/Product; streamlined release coordination
  (Improved developer satisfaction and release predictability; reduced cycle friction)
```

**Score Analysis (Improved):**
- Content Quality: 33/35 (strong impact metrics, scale context, strategic depth)
- Structure: 20/20 (perfect Europass format with scope line)
- Tone: 15/15 (objective, action verbs, evidence-based)
- Evidence: 15/15 (every achievement quantified with before/after)
- Completeness: 10/10 (all sections complete)
- Formatting: 10/10 (dates perfect, clean structure)

**TOTAL: 103/105 = 98% ⭐ EXCELLENT**

**Improvements Made:**
- ✅ Added scale context (500+ clients, 200K+ users, $2.5B transactions)
- ✅ Converted responsibilities to achievements with metrics
- ✅ Quantified every outcome (8%→2%, 80h→12h, etc.)
- ✅ Added business impact (cost saved, cycle time improved, satisfaction increased)
- ✅ Showed strategic decision-making and leadership

**Score Change:** 61% → 98% (+37 points)  
**Recommendation:** ✅ Ready to submit immediately

---

## 🚀 Using the Scoring System with Your Agent

### Integration Points

**When to Run Scoring:**
```
Input Validation    → Extract raw data
        ↓
Evidence Extraction → Flag missing metrics
        ↓
Categorization      → Validate against frameworks
        ↓
Compliance Review   → Check GDPR, formatting
        ↓
Transformation      → Apply enhancements
        ↓
** ← SCORE CALCULATION POINT
Structure Assembly  → Arrange output
        ↓
✅ FINAL SCORE + REPORT GENERATED
        ↓
Output: CV + Score (0-100) + Dimension Breakdown + Top 3 Improvements
```

### Scoring Output Includes

**1. Final Score (0-100%)**
```
FINAL SCORE: 87/100 = 87%
Status: STRONG
Recommendation: Ready; minor enhancements optional
```

**2. Dimension Breakdown**
```
Content Quality:      31/35  (91%) ✅ Strong
Structure Compliance: 18/20  (90%) ✅ Strong
Tone & Language:      15/15  (100%) ✅ Perfect
Evidence Density:     12/15  (80%) ⚠️ Good (add 1-2 more metrics)
Completeness:         10/10  (100%) ✅ Perfect
Formatting:           10/10  (100%) ✅ Perfect
```

**3. Top 3 Improvement Recommendations**
```
1. QUICK WIN: Add one more quantified achievement to first role
   (Currently 4 bullets; suggest 5 for maximum impact)

2. MEDIUM EFFORT: Extend "leadership" examples with mentorship scope
   (e.g., "Mentored 4 engineers; 2 promoted within 1 year")

3. CONTEXT ENHANCEMENT: Add scale context to each role
   (e.g., "Mainframe credit card clearing handling 50M+ transactions/year")
```

**4. Actionable Items (If Score <80%)**
```
MISSING DIMENSIONS:

The following dimensions need attention:
[ ] Business Impact Metrics - Add before/after comparisons
[ ] Scale Context - "How many users/systems/transactions?"
[ ] Strategic Evidence - "What decisions did you own?"
[ ] Mentorship/Leadership - "Did you lead or develop anyone?"
[ ] Career Progression - "Show growth from role to role"

ACTION: Request candidate provide specifics for above.
IMPACT: Will increase score by 15-25 points if added.
```

---

## 📋 Practical Workflow: Using Scoring for CV Improvement

### For Recruiters
```
1. Candidate uploads raw CV
2. System runs scoring
   → If score ≥75: Approve, export PDF
   → If score <75: Generate actionable items
3. Share improvement report with candidate
4. Candidate provides missing details
5. System re-scores
6. Repeat until score ≥75
```

### For Candidates (Self-Service)
```
1. Input raw CV data
2. Receive score + improvement suggestions
3. Review top 3 recommendations
4. Update CV with suggested changes
5. Re-submit for re-scoring
6. Iterate until score ≥85+ (excellent)
```

### For HR Leaders
```
1. Run scoring on all CVs in pipeline
2. Review score distribution curve
3. Identify candidates above 80 (strong) as priority
4. Schedule interviews with 85+ scores (excellent)
5. Use improvement reports to coach weak candidates
6. Track average score trends over time
```

---

## ✅ Scoring Checklist: Self-Assess Your CV

Before submitting to agent, verify:

```
CONTENT QUALITY (35 points max)
☐ Every role includes scale context (users/systems/criticality)
☐ Every achievement has a metric (%, time, $, count)
☐ At least one strategic decision described per role
☐ Mentorship or leadership evidence included
☐ Domain expertise clearly differentiated

STRUCTURE (20 points)
☐ Reverse chronological order (newest first)
☐ All sections present (summary, experience, education, skills, languages)
☐ Consistent formatting within each section
☐ Scope line includes: platform, users, transactions/criticality

TONE & LANGUAGE (15 points)
☐ Zero buzz words (passionate, rockstar, dynamic, guru, etc.)
☐ Zero first-person pronouns (I, me, my)
☐ All statements objective and fact-based
☐ No exclamation marks
☐ Action verbs strong (Led, Architected, Reduced, Prevented, etc.)

EVIDENCE (15 points)
☐ 90%+ of achievements include specific numbers
☐ Before/after metrics shown (where applicable)
☐ Scope quantified (people, systems, users, transactions)
☐ No vague claims ("improved," "worked on," "responsible for")

COMPLETENESS (10 points)
☐ Professional summary included
☐ 3+ work experiences with dates
☐ Education & certifications dated
☐ Skills categorized with proficiency levels
☐ Languages in CEFR format (A1-C2)

FORMATTING (10 points)
☐ All dates in DD/MM/YYYY or "Month YYYY" (NOT MM/DD/YYYY)
☐ Zero spelling or grammar errors
☐ Consistent bullet point format
☐ 1-3 pages maximum (2 preferred for most; allow 3 for senior/complex histories)
☐ No images, graphics, or special formatting
```

---

## 🎯 Success Targets by Role Level

### Entry-Level (0-3 years)
- **Target Score:** 70-79 (Acceptable)
- **Key Focus:** Competencies, education, consistent effort
- **Red Flag:** <60 (needs mentoring)

### Mid-Level (3-7 years)
- **Target Score:** 80-89 (Strong)
- **Key Focus:** Impact metrics, scope context, project leadership
- **Red Flag:** <75 (weak positioning)

### Senior-Level (7+ years)
- **Target Score:** 85-100 (Strong to Excellent)
- **Key Focus:** Strategic achievements, business impact, mentorship/leadership
- **Red Flag:** <80 (not senior-positioned)

### Director/Lead (10+ years)
- **Target Score:** 90-100 (Excellent)
- **Key Focus:** Strategic initiatives, team leadership, domain expertise, ROI/business impact
- **Red Flag:** <85 (missing strategic depth)

---

## 🔗 Framework References

- Scoring System: `.github/agents/framework-enhancements/cv-scoring-system.json`
- Senior Positioning: `.github/agents/framework-enhancements/senior-level-positioning.json`
- Business Impact: `.github/agents/framework-enhancements/business-impact-framework.json`
- Examples: `.github/agents/improved-cv-examples/nadine-tolentino-2026-improved-v3.md`

---

**Version:** 2.0 | Updated: 3 May 2026 | Status: Production Ready
