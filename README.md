# Faym PM Internship Assignment

Complete submission: returns automation agent + SQL analysis + interactive guide.

## 🚀 Start Here

**[Interactive Guide (Live)](https://faym-assignment-omega.vercel.app/)** — 2-minute walkthrough of the entire submission.

---

## 📋 Three Submissions

### 1. Interactive HTML Guide
- **Live:** https://faym-assignment-omega.vercel.app/
- **Covers:** 7 spec gaps, architecture, key decisions, proof, scope
- **Review time:** 2 min (overview) → 10 min (deep dive)

### 2. Returns Automation Agent (`faym_agent/`)

**Quick Start**
```bash
cd faym_agent
pip install -r requirements.txt
python -m pytest tests/ -v          # 10/10 tests passing
python main.py --demo               # Dry-run demo (no credentials needed)
```

**What Works (Tested)**
- ✓ Excel read/write (10 spec fields)
- ✓ Order grouping, partial success
- ✓ Eligibility checking, deterministic flow detection
- ✓ Retry logic (eligibility 0×, transient 3×)
- ✓ Idempotent, resumable runs
- ✓ Structured audit logging

**What's Scaffolded**
- ⚠ CSS selectors (representative, not verified live)
- ⚠ Stealth measures (implemented, not bot-tested)

**Key Files**
- `core/models.py` — ReturnTask, OrderGroup, status enums
- `core/orchestrator.py` — Main loop, grouping, retries
- `core/flow_detector.py` — Batch vs sequential detection
- `adapters/{amazon,flipkart}.py` — Platform implementations
- `tests/` — Unit tests (no browser needed)
- `README.md` — Full setup guide
- `DESIGN.md` — Design rationale

### 3. SQL Assignment (`assets/Daksh_Jain_Faym_SQL_Assignment.pdf`)

**5 Questions, Real SQL Against SQLite**
- Q1: 7th highest IMPS debit = ₹9,525
- Q2: Transaction counts by category (IMPS 272, IFT 89, UPI 86, NEFT 33, RTGS 21)
- Q3: Distribution analysis (flagged: NOT normal, kurtosis -1.20)
- Q4: Monthly cohort retention (January cohort 87.5–100% through July)
- Q5: Top 10 percentile user (flagged: n=10, so "top 10%" = 1 user)

**Honest caveats included** for statistical assumptions and dataset limitations.

---

## ✅ How to Review

**2 minutes:** Open the [interactive guide](https://faym-assignment-omega.vercel.app/)

**10 minutes:** + Run tests (`pytest tests/ -v`) and `main.py --demo`

**30 minutes:** + Read `DESIGN.md` and inspect `core/` code

---

## 📊 Verification

- [x] 10/10 tests passing
- [x] 7 spec gaps identified and resolved
- [x] Partial success scenario unit-tested
- [x] Idempotent, resumable after crash
- [x] SQL queries executed against real data
- [x] Honest about tested vs. scaffolded

---

## 📧 Contact

**Daksh Jain**
- Email: dakshjain311@gmail.com
- Phone: +91 8377804969
- Location: Bangalore, India
- GitHub: github.com/YOUR_USERNAME/FAYM_ASSIGNMENT

---

**Live guide:** https://faym-assignment-omega.vercel.app/
