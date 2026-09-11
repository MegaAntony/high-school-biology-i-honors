# AGENT.md — Master Architecture, Context & Operations Guide

> **Repository:** `MegaAntony/high-school-biology-i-honors`  
> **Local Workspace:** `/Volumes/Backup/Antony/HighSchool/Grade9/Biology-Honors-V2`  
> **Production Live Site:** [`https://megaantony.github.io/high-school-biology-i-honors/`](https://megaantony.github.io/high-school-biology-i-honors/)  
> **Course:** Grade 9 Biology I Honors • South Forsyth High School (Forsyth County, GA)  
> **Instructor:** Dr. Sarah Irwin (Room #371) • Academic Year 2026–2027  
> **State Standard Alignment:** Georgia Standards of Excellence (GSE) **SB1 through SB6**  
> **Canvas LMS Course ID:** `276259` (`30115y - Irwin - 501`)

---

## 🏛️ 1. Project Background & Repository Dual-Setup

### Historical Context & Separation of Concerns
Originally, the course materials were hosted in a single repository:
* **V1 / Legacy Repo:** [`MegaAntony/biology-honors`](https://github.com/MegaAntony/biology-honors)  
  * Local path: `/Volumes/Backup/Antony/HighSchool/Grade9/Biology-Honors`  
  * Live URL: `https://megaantony.github.io/biology-honors/`  
  * **CRITICAL DIRECTIVE:** V1 is **FROZEN & UNTOUCHED**. It remains active on GitHub Pages to guarantee that any preexisting bookmarks or links created by the student, family, or teacher continue to resolve without interruption.

* **V2 / Master Academic Year Repo:** [`MegaAntony/high-school-biology-i-honors`](https://github.com/MegaAntony/high-school-biology-i-honors)  
  * Local path: `/Volumes/Backup/Antony/HighSchool/Grade9/Biology-Honors-V2`  
  * Live URL: `https://megaantony.github.io/high-school-biology-i-honors/`  
  * **PURPOSE:** This is the primary, refactored, long-term workspace for the entire academic year (Units 01 through 10, Semester 1 & 2 Schedules, and Georgia Milestones EOC review). All new materials, tests, and weekly plans are added exclusively here.

---

## 📂 2. Full Directory Tree & Architecture

```
Biology-Honors-V2/
├── index.html                                 # Web Dashboard (Responsive 10-unit curriculum portal)
├── notInLocal.html                            # Master Cloud Links (Canvas Studio, Blooket, YouTube)
├── Georgia_Standards-Biology I Honors.md      # Official state curriculum standards (SB1–SB6)
├── ACADEMIC_YEAR_PLAN_AND_UNIT_PLAYBOOK.md    # 36-Week Roadmap & 6-Phase New Unit Ingestion Guide
├── AGENT.md                                   # This agent onboarding & context file
├── WEEKEND_CLEANUP_PLAN.md                    # Weekend Legacy Directories Cleanup Guide
├── README.md                                  # Repository overview and quick-launch bar
├── .gitignore                                 # Ignores .DS_Store, node_modules, temp files
│
├── schedule/                                  # 📅 Tactical Weekly Planners
│   ├── semester-1.md                          # S1 Master Calendar (Weeks 1–18 with deep links)
│   └── semester-2.md                          # S2 Master Calendar (Weeks 19–36 & EOC review)
│
├── units/                                     # 🧬 Permanent Unit Knowledge Base (10 Units)
│   ├── unit-01-biochemistry/                  # GSE: SB1.c
│   │   ├── README.md                          # Unit overview, targets, resource index
│   │   ├── materials/                         # Original PDFs, PPTs, and student packets
│   │   └── tests/                             # Interactive HTML quizzes (Vocab + Summative)
│   │
│   ├── unit-02-cells-and-transport/           # GSE: SB1.a & SB1.d (CURRENT UNIT)
│   │   ├── README.md                          # Complete Unit 2 resource hub
│   │   ├── cell_transport_final_cheat_sheet.html # Printable 1-column walk-in reference sheet
│   │   ├── notInLocal.html                    # Unit-level cloud links
│   │   ├── materials/
│   │   │   ├── pdf/                           # 10 teacher source PDFs/PPTs
│   │   │   └── md/                            # 19 searchable Markdown study guides & vocab tables
│   │   └── tests/                             # 26 interactive HTML test files (635 MCQs)
│   │       ├── index.html                     # Unit 2 Test Portal & card launcher
│   │       ├── test-01 to test-15.html        # 15 targeted concept deep dives (20 Qs each)
│   │       ├── test-doc-01 to doc-09.html     # 9 in-class handout drills (20 Qs each)
│   │       └── test-unit-2-part-1-comprehensive-mastery.html # 55-Q Master Exam
│   │
│   ├── unit-03-cellular-energetics/           # GSE: SB1.e (Scaffolded)
│   ├── unit-04-cellular-reproduction/         # GSE: SB1.b (Scaffolded)
│   ├── unit-05-gene-expression/               # GSE: SB2.a, SB2.b (Scaffolded)
│   ├── unit-06-genetics/                      # GSE: SB3.a–c (Scaffolded)
│   ├── unit-07-biotechnology/                 # GSE: SB2.c, SB4.a (Scaffolded)
│   ├── unit-08-evolution/                     # GSE: SB6.a–e (Scaffolded)
│   ├── unit-09-ecology/                       # GSE: SB5.a–c (Scaffolded)
│   └── unit-10-diversity-of-life/             # GSE: SB4.a, SB4.b (Scaffolded)
│
├── cumulative-exams/                          # 🏆 Benchmarks & State EOC Prep
│   ├── semester-1-final/                      # Comprehensive S1 Benchmark (Dec)
│   └── georgia-milestones-eoc/                # Georgia State Milestones Exam Prep (May)
│
├── Week-9-7/tests/                            # 🔁 Backwards-compatible redirects (26 stubs)
└── unit01-tests/                              # 🔁 Backwards-compatible redirects (3 stubs)
```

---

## 🚀 3. GitHub Pages Deployment Details

* **Hosting:** GitHub Pages via GitHub Actions / Legacy Jekyll static pipeline.
* **Source:** Branch `main`, path `/ (root)`.
* **Live Base URL:** `https://megaantony.github.io/high-school-biology-i-honors/`
* **Custom Configuration:**
  * Enforce HTTPS: `true`
  * CNAME: None (uses `megaantony.github.io`)
* **Dual URL Compatibility (Backwards Compatibility Architecture):**
  * When migrating from V1, all existing test paths (`Week-9-7/tests/*.html` and `unit01-tests/*.html`) were mapped using 0-millisecond `<meta http-equiv="refresh">` redirect stubs.
  * **Result:** Any user accessing either the new clean path (`units/unit-02-cells-and-transport/tests/...`) OR the legacy path (`Week-9-7/tests/...`) on the new domain is served seamlessly with HTTP 200.
* **Deployment Verification Workflow:**
  After pushing commits to `main`, monitor the build using GitHub CLI:
  ```bash
  gh api /repos/MegaAntony/high-school-biology-i-honors/pages/builds --jq '.[0].status'
  # Wait until it outputs "built"
  # Then verify live response:
  /usr/bin/curl -s -o /dev/null -w "%{http_code}\n" https://megaantony.github.io/high-school-biology-i-honors/
  ```

---

## 🧪 4. Complete Test Suite Inventory (27 Assessments / 657 Questions)

Every quiz in the repository is a self-contained, responsive single-page web app built with Tailwind CSS, FontAwesome icons, and a client-side JavaScript engine.

### Data Model Schema (`questionsData` array):
```javascript
const questionsData = [
  {
    id: 1,
    topic: "Phospholipid Bilayer",
    question: "Exact question stem describing a biological mechanism?",
    options: [
      "Distractor A (conceptually plausible misconception)",
      "Distractor B (partially correct statement)",
      "Correct Answer",
      "Distractor D"
    ],
    answer: 2, // 0-indexed integer
    clue: "Guiding pedagogical hint without revealing the answer.",
    explanation: "Comprehensive rationale explaining why C is correct and why A, B, and D are incorrect."
  }
];
```

### Full Test Inventory Roster:

| Test ID | Relative Path | Focus & Standard | Questions |
| :--- | :--- | :--- | :---: |
| **U1-Vocab** | `units/unit-01-biochemistry/tests/Unit_1_Complete_Vocab_Mastery_Quiz.html` | 78 terms, flashcards (`SB1.c`) | 78 |
| **U1-Exam** | `units/unit-01-biochemistry/tests/Unit_1_Summative_Practice_Test.html` | Macromolecules & enzyme kinetics (`SB1.c`) | 44 |
| **U2-Master** | `units/unit-02-cells-and-transport/tests/test-unit-2-part-1-comprehensive-mastery.html` | Master exam for Part 1 (`SB1.a, d`) | 55 |
| **Test 01** | `units/unit-02-cells-and-transport/tests/test-01-membrane-structure.html` | Bilayer architecture & fluidity (`SB1.d`) | 20 |
| **Test 02** | `units/unit-02-cells-and-transport/tests/test-02-simple-diffusion.html` | Concentration gradients & small nonpolar gas transport | 20 |
| **Test 03** | `units/unit-02-cells-and-transport/tests/test-03-facilitated-diffusion.html` | Channel & carrier proteins, aquaporins | 20 |
| **Test 04** | `units/unit-02-cells-and-transport/tests/test-04-osmosis-fundamentals.html` | Osmotic pressure & U-tube mechanics | 20 |
| **Test 05** | `units/unit-02-cells-and-transport/tests/test-05-tonicity-scenarios.html` | Hypo/hyper/isotonic, crenation, lysis, turgor | 20 |
| **Test 06** | `units/unit-02-cells-and-transport/tests/test-06-molecular-pumps.html` | ATP pumps, $\text{Na}^+/\text{K}^+$ ATPase | 20 |
| **Test 07** | `units/unit-02-cells-and-transport/tests/test-07-endocytosis.html` | Phago/pinocytosis & receptor-mediated | 20 |
| **Test 08** | `units/unit-02-cells-and-transport/tests/test-08-exocytosis.html` | Vesicle fusion, insulin, neurotransmitters | 20 |
| **Test 09** | `units/unit-02-cells-and-transport/tests/test-09-passive-vs-active.html` | Comprehensive comparative transport matrix | 20 |
| **Test 10** | `units/unit-02-cells-and-transport/tests/test-10-transport-labs.html` | Dialysis tubing, potato osmolarity, egg lab | 20 |
| **Test 11** | `units/unit-02-cells-and-transport/tests/test-11-cell-theory.html` | Hooke, Leeuwenhoek, Schleiden, Schwann, Virchow | 20 |
| **Test 12** | `units/unit-02-cells-and-transport/tests/test-12-prokaryotes-vs-eukaryotes.html` | Nucleoid vs. nucleus, organelles, $70\text{S}/80\text{S}$ | 20 |
| **Test 13** | `units/unit-02-cells-and-transport/tests/test-13-plant-vs-animal.html` | Vacuole, chloroplast, cell wall, centrioles | 20 |
| **Test 14** | `units/unit-02-cells-and-transport/tests/test-14-surface-area-volume.html` | $SA:V$ math, diffusion limits, cell size | 20 |
| **Test 15** | `units/unit-02-cells-and-transport/tests/test-15-microscopy-investigation.html` | Compound light microscope parts & FOV math | 20 |
| **Doc 01** | `units/unit-02-cells-and-transport/tests/test-doc-01-osmosis-tonicity.html` | Dr. Irwin's Tonicity Practice Questions | 20 |
| **Doc 02** | `units/unit-02-cells-and-transport/tests/test-doc-02-cells-organelles.html` | Cells 1: Organelles Study Sheet | 20 |
| **Doc 03** | `units/unit-02-cells-and-transport/tests/test-doc-03-membrane-transport-ppt.html` | Part 1 Lecture Slides Drill | 20 |
| **Doc 04** | `units/unit-02-cells-and-transport/tests/test-doc-04-cell-theory-structure-ppt.html` | Part 2 Lecture Slides Drill | 20 |
| **Doc 05** | `units/unit-02-cells-and-transport/tests/test-doc-05-honors-cell-stations.html` | Honors Cell Investigation Stations | 20 |
| **Doc 06** | `units/unit-02-cells-and-transport/tests/test-doc-06-microscope-parts-use.html` | Microscope Protocol & Parts PPT | 20 |
| **Doc 07** | `units/unit-02-cells-and-transport/tests/test-doc-07-transport-situation-cards.html` | In-class 15 Transport Situation Cards | 20 |
| **Doc 08** | `units/unit-02-cells-and-transport/tests/test-doc-08-cell-transport-student-packet.html` | Part 1 Student Packet Review Questions | 20 |
| **Doc 09** | `units/unit-02-cells-and-transport/tests/test-doc-09-cell-structure-student-packet.html` | Part 2 Student Packet Organelle Drills | 20 |
| **Cheat Sheet**| `units/unit-02-cells-and-transport/cell_transport_final_cheat_sheet.html` | 1-Column Printable Walk-In Review | Ref |

---

## 🧬 5. Curriculum Standards Map (Georgia GSE SB1–SB6)

When adding materials or generating tests, agents must map concepts to these exact codes:

* **`SB1` — Cellular Structure & Function**
  * `SB1.a`: Cell structures, organelles, and functions in maintaining homeostasis.
  * `SB1.b`: Role of cellular reproduction (mitosis & cell cycle) in maintaining genetic continuity.
  * `SB1.c`: Macromolecules (carbohydrates, lipids, proteins, nucleic acids) and role of enzymes.
  * `SB1.d`: Selective permeability of cell membranes and transport mechanisms (passive vs. active).
  * `SB1.e`: Energy transformations (cellular respiration and photosynthesis, ATP cycle).
* **`SB2` — Molecular Genetics & Biotechnology**
  * `SB2.a`: DNA and RNA structure, replication, transcription, translation (Central Dogma).
  * `SB2.b`: Role of DNA mutations in causing genetic variation.
  * `SB2.c`: Societal, ethical, and environmental impacts of biotechnology (PCR, gel electrophoresis, CRISPR).
* **`SB3` — Heredity & Patterns of Inheritance**
  * `SB3.a`: Meiosis, crossing over, independent assortment, and gametogenesis.
  * `SB3.b`: Mendelian and non-Mendelian inheritance (incomplete dominance, codominance, sex-linked, multiple alleles).
  * `SB3.c`: Pedigree analysis and karyotypes to track genetic disorders.
* **`SB4` — Classification & Biodiversity**
  * `SB4.a`: Organism classification based on evolutionary relationships and taxonomy (3 Domains, 6 Kingdoms).
  * `SB4.b`: Cladograms, phylogenetic trees, and dichotomous keys.
* **`SB5` — Ecology & Ecosystem Dynamics**
  * `SB5.a`: Interdependence of organisms, trophic pyramids, 10% rule, and food webs.
  * `SB5.b`: Biogeochemical cycles (Carbon, Nitrogen, Water, Phosphorus).
  * `SB5.c`: Population ecology (carrying capacity, limiting factors, ecological succession).
* **`SB6` — Evolution & Natural Selection**
  * `SB6.a`: Natural selection mechanisms (variation, overproduction, differential survival).
  * `SB6.b`: Evidence for evolution (fossil record, anatomical homologies, embryology, molecular sequences).
  * `SB6.c`: Genetic drift, gene flow, mutations, and non-random mating.
  * `SB6.d`: Speciation and reproductive isolation mechanisms.
  * `SB6.e`: Hardy-Weinberg equilibrium modeling.

---

## 🛠️ 6. Rules & Protocols for Future Agents

Whenever an agent performs work in `/Volumes/Backup/Antony/HighSchool/Grade9/Biology-Honors-V2`, the following rules **MUST** be obeyed:

### Rule 1: Zero Broken Relative Links
Never push code without running the validation script:
```bash
python3 -c '
import os, re, urllib.parse
from pathlib import Path

root = Path(".")
html_md_files = list(root.glob("**/*.html")) + list(root.glob("**/*.md"))
broken = []
checked = 0

for f in html_md_files:
    if ".git" in f.parts: continue
    try: content = f.read_text(encoding="utf-8", errors="ignore")
    except Exception: continue
    content_no_code = re.sub(r"```[\s\S]*?```", "", content)
    html_links = re.findall(r"href=[\"\x27]([^\s\"\x27>]+)[\"\x27]", content_no_code)
    md_links = re.findall(r"\[[^\]]*\]\(([^)\s]+)\)", content_no_code)
    for raw_link in html_links + md_links:
        if raw_link.startswith(("http://", "https://", "mailto:", "javascript:", "#")): continue
        clean_link = urllib.parse.unquote(raw_link.split("?")[0].split("#")[0])
        link_path = (f.parent / clean_link).resolve()
        checked += 1
        if not link_path.exists():
            broken.append((str(f.relative_to(root)), raw_link))

print(f"Checked {checked} relative links across {len(html_md_files)} files.")
if broken:
    print(f"❌ Found {len(broken)} broken link(s):")
    for src, l in broken: print(f"  {src} -> {l}")
    exit(1)
else:
    print("✅ All relative links are 100% valid! Zero broken links.")
'
```

### Rule 2: Ingesting New Units (Units 03–10)
Follow the 6-phase playbook documented in [`ACADEMIC_YEAR_PLAN_AND_UNIT_PLAYBOOK.md`](ACADEMIC_YEAR_PLAN_AND_UNIT_PLAYBOOK.md):
1. **Ingest:** Download PDFs to `units/unit-XX-[name]/materials/pdf/`.
2. **Digest:** Extract clean markdown notes into `units/unit-XX-[name]/materials/md/`.
3. **Build:** Create `test-vocab-mastery.html`, `test-concept-application.html`, and `test-unit-XX-summative-mastery.html` using the standardized quiz engine template.
4. **Wire:** Update `units/unit-XX/README.md`, `tests/index.html`, root `index.html`, and `schedule/semester-1.md` or `semester-2.md`.
5. **Audit:** Execute the Python link verification script.
6. **Deploy:** `git commit` and `git push origin main`. Confirm status `"built"` via `gh api`.

### Rule 3: Maintain Backward Compatibility
Do NOT delete or rename files in `Week-9-7/tests/` or `unit01-tests/`. These redirect stubs ensure that any historical browser bookmarks continue to route seamlessly to the new unit locations.

### Rule 4: Do Not Touch V1
Never make commits or file edits in `/Volumes/Backup/Antony/HighSchool/Grade9/Biology-Honors` or push to remote `MegaAntony/biology-honors`.
