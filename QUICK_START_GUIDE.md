# Resume Specialist Agent - Quick Start Reference Guide

**Last Updated:** 3 May 2026  
**Target User:** HR Managers, Recruiters, Talent Screeners  
**Time to Generate CV:** 15-20 minutes  
**Output Format:** Europass-compliant, 1-3 pages, PDF-ready

---

## 🚀 Quick Start in 5 Steps

### Step 1: Collect Raw Data (5 min)
**Provide the candidate with this checklist:**

```
□ Full name and current contact info
□ Work experience (dates, titles, companies, responsibilities)
□ Quantified achievements (metrics, percentages, business impact)
□ Education and degree details
□ Languages with proficiency level (or we'll convert for you)
□ Certifications and dates
□ Technical skills with years of experience
```

**Better input = Better output** ✅

---

### Step 2: Load Into Agent (2 min)
1. Access `resume-generator.agent.md` (source of truth)
2. Load all JSON files from `.github/agents/` folders
3. Run input validation stage to flag issues
4. Candidate receives validation report

---

### Step 3: Run Transformation Pipeline (5 min)
Agent automatically:

| Stage | Action | Time |
|-------|--------|------|
| **Validation** | Check format, language, GDPR | 1 min |
| **Extraction** | Parse data, flag unsupported claims | 1 min |
| **Categorization** | Map to skill frameworks | 1 min |
| **Compliance** | GDPR check, age discrimination prevention | 1 min |
| **Transformation** | Remove buzzwords, format dates, organize | 1 min |

---

### Step 4: Review & Approve (5 min)
Agent generates:
- ✅ Cleaned CV (1-3 pages)
- ✅ Transformation report (what changed and why)
- ✅ Quality score (see scoring section below)
- ⚠️ Escalation flags (if any)

Candidate reviews and approves.

---

### Step 5: Export & Send (2 min)
- PDF download with Europass formatting
- Filename: `FirstName_LastName_CV.pdf`
- Ready to submit to employers

---

## 🎯 What This Agent Fixes

### ❌ Before (Raw Input Issues)
```
"I am a passionate and dynamic rockstar engineer 
with a proven track record in leading teams. 
Results-driven professional who think outside the box."
```

### ✅ After (Agent Output)
```
"Senior QA Engineer with 10+ years' experience 
leading enterprise testing initiatives across HRIS, 
payroll, and financial systems. Reduced critical 
defect escape rate from 8% to 2% through structured 
test strategy implementation. Directed testing for 
systems processing 500K+ daily transactions."
```

---

## 📋 Input Format Template

Provide candidates with this template to fill:

### Personal Information
```
Full Name: [First Last]
Email: [professional@email.com]
Phone: [+country code number]
Current Location: [City, Country]
LinkedIn: [optional URL]
```

### Work Experience (For Each Role)
```
Company: [Full Legal Name]
Job Title: [Official Title]
Employment Type: [Full-time/Contract/Remote]
Start Date: [Month Year]
End Date: [Month Year or "Present"]

Description of Key Responsibilities:
- [Responsibility 1]
- [Responsibility 2]
- [Responsibility 3]

Measurable Achievements:
- [Specific metric or outcome 1]
- [Specific metric or outcome 2]
- [Specific metric or outcome 3]
```

**IMPORTANT:** Achievements must include:
- **What** was accomplished
- **How** it was done (approach/methodology)
- **Impact** (numbers, percentages, business value)

### Example - Good vs. Bad
```
❌ BAD:
"Performed testing across multiple systems"

✅ GOOD:
"Designed and executed regression test suite for 
payroll module: 450+ test cases covering 95% code 
coverage; caught 28 critical defects pre-release, 
preventing estimated $200K revenue loss"
```

---

## 🔍 Agent Decision Tree

```
User provides raw resume
        ↓
Is the input valid?
        ├─ NO → Return validation errors & request input
        └─ YES ↓
        
Does it contain Americanisms/buzzwords?
        ├─ YES → Auto-convert (show changes)
        └─ NO ↓
        
Does it exceed 3 pages when formatted?
        ├─ YES → Return with consolidation suggestions
        └─ NO ↓
        
Does it contain prohibited personal data?
        ├─ YES → Auto-remove (flag for review)
        └─ NO ↓
        
Are all achievements quantified?
        ├─ NO → Flag for user to provide metrics
        └─ YES ↓
        
Generate Europass-compliant CV
        ↓
Calculate quality score
        ↓
Export PDF with report
```

---

## ⚡ Common Issues & Fixes

### Issue 1: "Experienced in X technology"
**Problem:** No proficiency level or experience duration  
**Fix:** Request: "How many years? Used in how many projects?"  
**Converts to:** "Python - Advanced (5 years, 12 production projects)"

### Issue 2: "Led the team"
**Problem:** No scope, no metrics, no business impact  
**Fix:** Request: "How many people? What were the results?"  
**Converts to:** "Supervised QA team of 6; improved on-time delivery from 75% to 98%; reduced bug escape rate by 45%"

### Issue 3: "Responsible for testing"
**Problem:** Sounds like a job description, not an achievement  
**Fix:** Request: "What was the impact? Any metrics?"  
**Converts to:** "Owned regression testing for enterprise HRIS system (5 modules, 200+ data fields); prevented 34 data loss incidents through edge case validation"

### Issue 4: "Strong communication skills"
**Problem:** Subjective; no evidence  
**Fix:** Remove from CV; OR  
**Convert to:** "Delivered quarterly test strategy presentations to C-level stakeholders; trained 3 junior QA engineers; documented 50+ technical specifications"

### Issue 5: Dates like "05/15/2024"
**Problem:** US format (ambiguous)  
**Fix:** Auto-convert to: "15 May 2024" or "15/05/2024"

---

## 📊 Quality Score Interpretation

**Scoring Formula:** See detailed scoring section below

| Score | Status | Recommendation |
|-------|--------|---|
| 90-100 | Excellent | Ready to submit immediately |
| 80-89 | Strong | Ready; minor enhancements optional |
| 70-79 | Acceptable | Acceptable; recommend revisions |
| 60-69 | Needs Work | Requires revisions before submission |
| <60 | Weak | Major overhaul needed |

**Score Breakdown Example:**
```
Content Quality:        32/35  (91%) - Strong impact metrics
Structure Compliance:   18/20  (90%) - Europass format
Tone & Language:        15/15  (100%) - Professional, objective
Evidence Density:       14/15  (93%) - Mostly quantified
Completeness:           10/10  (100%) - All sections present
Formatting:             10/10  (100%) - Date, spelling, layout

TOTAL SCORE: 99/105 = 94% ⭐ EXCELLENT
```

---

## ✅ Pre-Submission Checklist

Before sending to employers, verify:

```
□ No buzzwords (checked against prohibited list)
□ All dates in DD/MM/YYYY or "Month YYYY" format
□ All achievements include metrics/numbers
□ No first-person pronouns (I, me, my)
□ No personal data except name, email, location, phone
□ CV is 1-3 pages maximum (2 pages preferred)
□ CEFR format for all languages (A1-C2)
□ All work experience in reverse chronological order
□ All certifications have issue and expiration dates
□ No exclamation marks or marketing language
□ Score ≥ 75 (minimum acceptable)
```

---

## 🎓 Framework Components Reference

When working with the agent, you'll encounter:

### Skill Cards (Categorization)
- **language-skills.json** → Languages must be CEFR (A1-C2)
- **digital-skills.json** → Tech skills organized by category
- **interpersonal-skills.json** → Soft skills (evidence-based only)
- **organizational-skills.json** → Leadership with measurable outcomes
- **sector-specific-skills.json** → Industry expertise

### Guardrails (Enforcement)
- **tone-and-language.json** → Buzzword detection & removal
- **formatting-standards.json** → Dates, structure, length
- **content-constraints.json** → Evidence levels, personal data rules

### Context Gates (Boundaries)
- **cv-structure.json** → Section hierarchy & templates
- **european-compliance.json** → GDPR, age discrimination prevention
- **remote-applicant-guidelines.json** → Global applicant standards

---

## 🌟 Success Metrics

A **good output** from this agent achieves:

✅ **Europass Compliant** - Internationally recognized format  
✅ **Evidence-Dense** - Every claim backed by metrics  
✅ **Senior-Appropriate** - Shows leadership & impact (if applicable)  
✅ **Objective Tone** - Zero buzz words, pure facts  
✅ **GDPR Safe** - No unnecessary personal data  
✅ **Globally Ready** - Works for EU and remote applicants  
✅ **Concise** - 1-3 pages, prioritized by relevance  
✅ **No Hallucination** - Every word from candidate's input  

---

## 🆘 Troubleshooting

| Problem | Solution |
|---------|----------|
| **"CV exceeds 3 pages"** | Consolidate roles >10 years old; reduce non-essential details |
| **"Missing metrics"** | Request candidate to provide numbers: revenue, time saved, defect counts, etc. |
| **"Buzzwords detected"** | System auto-removes; candidate approves replacements |
| **"No career progression shown"** | Restructure to highlight increasing responsibility; use org skills framework |
| **"Score too low (<70)"** | Review transformation report; likely due to lacking quantified achievements |
| **"Format not accepted"** | Verify reverse chronological order, Europass compliance, and section structure |

---

## 📋 Quick Scoring Run

- The agent computes a 0–100 score using: .github/agents/framework-enhancements/cv-scoring-system.json
- Thresholds: 90+ Excellent, 80–89 Strong, 70–79 Acceptable, 60–69 Needs Work, <60 Weak
- Output includes dimension breakdown and top 3 improvements

Run order:
1) Validate → 2) Extract → 3) Categorize → 4) Transform → 5) Assemble → 6) Score → 7) Export

---

## Example: Applying To Nadine Tolentino

Input: .github/agents/raw-resume/nadine-tolentino-2026.md

Agent produced:
- Actionable Items: scale context, metrics (before→after), leadership scope, mainframe specialization evidence
- Improved CV: .github/agents/improved-cv-examples/nadine-tolentino-2026-improved.md
- Scoring reports saved under .github/agents/scoring-reports/

Notes:
- No fabrication; prompts ask the candidate to supply real data
- Final CV is concise, senior-positioned, and Europass-compliant

---

**Version:** 1.0  
**Status:** Production Ready  
**Last Updated:** 3 May 2026
