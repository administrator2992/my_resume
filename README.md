# Personal academic curriculum vitae (CV) latex templates
Click `use this template` and replace the content to your information.

Enabling github actions and Github pages will make your CV available online at ```https://{your_github_username}.github.io/{repo_name}/main_cv.pdf```.

## Note

Access `https://{your_github_username}.github.io/{repo_name}` will redirect to `main_cv.pdf`

---

# AI CV-Optimization Agent — Tutorial

This repo doubles as a workspace for an **AI agent** that tailors your CV to a
specific job or academic application. The agent reads your master data, maps it
against a target job description (JD), rewrites your experience using measurable
(XYZ) bullet points, keeps the document ATS-friendly, and builds the PDF — all
on a dedicated git branch.

## How it works (the big picture)

```
  PROFILE.md  ──(your master data, single source of truth)
      │
      ▼
  JOB_PROFILE.md  ──(paste a job description, agent maps it to your data)
      │
      ▼
  main_cv.tex  ──(agent edits this on a cv/... branch, applies XYZ + ATS rules)
      │
      ▼
  CV_Nabhaan_<Target>.pdf  ──(compiled output)
```

## File map — what each file is for

| File | Role |
|---|---|
| `PROFILE.md` | **Single source of truth.** All your real data (contact, education, experience, research, publications, skills). Edit this first if anything is outdated. |
| `JOB_PROFILE.md` | **Per-target worksheet.** Paste one job description here; the agent fills in keyword extraction, gap analysis, and an edit plan. |
| `main_cv.tex` | The actual LaTeX CV the agent edits and compiles. |
| `biblio.bib` | Publication references (used by biblatex). |
| `AGENTS.md` | The agent's rules: ATS methodology, XYZ formula, word limits, git/LaTeX workflow. |
| `skills.md` | The agent's 5 operational skills (formatter, keyword balancer, word-count validator, bilingual manager, git/LaTeX builder). |
| `PROMPTS.md` | Ready-to-copy prompt templates (industry & academic). |
| `TASKS.md` | The agent's persistent memory/recovery notes. |

## Step-by-step: tailor your CV to a job

### 1. Make sure `PROFILE.md` is current
The agent only uses what's in `PROFILE.md`. If a job, score, or skill is missing
or wrong, fix `PROFILE.md` **before** generating a CV. (Ask the agent:
*"check the LaTeX CV against PROFILE.md and reconcile differences."*)

### 2. Fill in the target in `JOB_PROFILE.md`
Open `JOB_PROFILE.md` and complete **Section 1**:
- Company / institution, position, location, CV language (ID/EN),
  and whether it's **Industri** or **Akademik**.
- Paste the full job description into the ```text ... ``` block.

### 3. Ask the agent to optimize
Use one of the templates in `PROMPTS.md`, or just say:

> *"Optimize my CV for the job in JOB_PROFILE.md."*

The agent will:
1. Extract **hard + soft skills** from the JD (Section 2 of `JOB_PROFILE.md`).
2. Run a **gap analysis** vs. `PROFILE.md` (Section 3).
3. Draft a Personal Summary + **XYZ bullets** and an edit plan (Section 4).
4. Edit `main_cv.tex` on a new branch `cv/<target>-<position>-<year>`.
5. Build the PDF.

### 4. Review and build
Compile locally (the document uses **biblatex + biber**, so a single `pdflatex`
is not enough):

```bash
pdflatex main_cv.tex
biber main_cv
pdflatex main_cv.tex
pdflatex main_cv.tex
```

Output is renamed per target, e.g. `CV_Nabhaan_KAUST.pdf`.

## The two modes

### Industry (corporate job)
- Pulls only the **most relevant** experience for the JD.
- Every experience bullet uses the **XYZ formula**:
  *"Achieved [X] measured by [Y], by doing [Z]"* — at least 5 measurable metrics.
- Each bullet contains ≥1 hard/soft keyword from the JD (no keyword stuffing).
- No first-person pronouns, clichés, or buzzwords.
- Target length: **475–600 words**.

### Academic (Master's / PhD / research lab)
- Prioritizes **Research Experience** and **Education** from `PROFILE.md`.
- Includes language scores (TOEFL) and publication/LinkedIn links.
- Uses XYZ to describe experimental results and algorithmic efficiency.
- **Ignores** the 600-word cap — research and publications are detailed in full.

## Rules the agent always follows (from `AGENTS.md`)
- `PROFILE.md` is the single source of truth.
- Mandatory contacts: Email, Phone, LinkedIn (+ publications for academic).
- ≥ 5 measurable XYZ metrics across the document.
- Balanced hard/soft keywords, inserted naturally.
- Anti-fluff: plain, direct sentences.
- Language: International = EN, Domestic = ID.
- Git: always branch off `main` as `cv/<target>-<year>`; **commit/push only when you ask.**

## Tips
- One job at a time: archive an old target in **Section 6** of `JOB_PROFILE.md`
  before pasting a new one.
- Keep `PROFILE.md` honest and complete — better input data = better tailored CV.
- For a new target language, tell the agent up front (ID or EN); it adjusts
  section headers and action verbs.
