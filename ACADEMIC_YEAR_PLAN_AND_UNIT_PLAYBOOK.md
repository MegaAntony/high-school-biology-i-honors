# Biology I Honors (Grade 9) — Full Academic Year Plan & New Unit Ingestion Playbook
### South Forsyth High School • Dr. Sarah Irwin (Room #371) • Academic Year 2026–2027
*Aligned to Georgia Standards of Excellence (GSE) for Science: **SB1 through SB6***

---

## 🧭 Executive Summary & Core Philosophy

This document serves as the master curriculum roadmap and the standardized operational playbook for the entire 36-week Grade 9 Biology I Honors course. It is built to achieve two simultaneous goals:
1. **Academic Excellence:** Provide comprehensive, standard-aligned preparation for daily coursework, weekly formative quizzes, unit summative tests, the Semester 1 Final Exam, and the high-stakes spring **Georgia Milestones Biology End-of-Course (EOC) Assessment**.
2. **Operational Repeatability:** Establish an automated, modular workflow for ingesting teacher lecture decks, lab packets, worksheets, and study guides, transforming them into searchable markdown summaries and interactive HTML self-assessment test suites without breaking repository architecture or GitHub Pages deployments.

---

## 📅 Part 1: Full Academic Year Curriculum Roadmap (36 Weeks)

The curriculum is structured across 10 core units, divided into two 18-week semesters. Every unit is strictly mapped to the Georgia Standards of Excellence (GSE).

```
╔══════════════════════════════════════════════════════════════════════════════════════════╗
║                          SEMESTER 1: CELLULAR & MOLECULAR BIOLOGY                        ║
╠══════════╦═════════════════════════════════════════════╦═══════════════╦═════════════════╣
║ Unit     ║ Curriculum Topic                            ║ GSE Standard  ║ Timeline        ║
╠══════════╬═════════════════════════════════════════════╬═══════════════╬═════════════════╣
║ Unit 01  ║ Biochemistry & Macromolecules               ║ SB1.c         ║ Weeks 01 – 03   ║
║ Unit 02  ║ Cell Architecture & Membrane Transport     ║ SB1.a, SB1.d  ║ Weeks 04 – 06   ║
║ Unit 03  ║ Cellular Energetics (Photo & Respiration)   ║ SB1.e         ║ Weeks 07 – 09   ║
║ Unit 04  ║ Cellular Reproduction & Mitosis             ║ SB1.b         ║ Weeks 10 – 11   ║
║ Unit 05  ║ Molecular Genetics & Protein Synthesis      ║ SB2.a, SB2.b  ║ Weeks 12 – 14   ║
║ Unit 06A ║ Meiosis & Mendelian Genetics Foundations    ║ SB3.a, SB3.b  ║ Weeks 15 – 16   ║
║ Review   ║ S1 Cumulative Review & Final Benchmark      ║ SB1 – SB3     ║ Weeks 17 – 18   ║
╠══════════╩═════════════════════════════════════════════╩═══════════════╩═════════════════╣
║                          SEMESTER 2: GENETICS, EVOLUTION & ECOLOGY                       ║
╠══════════╦═════════════════════════════════════════════╦═══════════════╦═════════════════╣
║ Unit 06B ║ Complex Inheritance & Pedigree Analysis     ║ SB3.b, SB3.c  ║ Weeks 19 – 21   ║
║ Unit 07  ║ Biotechnology & Genetic Engineering         ║ SB2.c, SB4.a  ║ Weeks 22 – 24   ║
║ Unit 08  ║ Evolution & Natural Selection               ║ SB6.a – SB6.e ║ Weeks 25 – 28   ║
║ Unit 09  ║ Ecology & Ecosystem Dynamics                ║ SB5.a – SB5.c ║ Weeks 29 – 32   ║
║ Unit 10  ║ Diversity of Life, Taxonomy & Cladistics    ║ SB4.a, SB4.b  ║ Weeks 33 – 34   ║
║ EOC Prep ║ Georgia Milestones State Biology EOC Review ║ SB1 – SB6     ║ Week 35         ║
║ Finals   ║ Spring Finals & State Milestones Exam       ║ SB1 – SB6     ║ Week 36         ║
╚══════════╩═════════════════════════════════════════════╩═══════════════╩═════════════════╝
```

---

### Unit-by-Unit Detailed Scope & High-Yield Focus

#### Unit 01: Biochemistry & Macromolecules (Weeks 1–3) — `SB1.c`
* **Status:** Complete & Archived (`units/unit-01-biochemistry/`)
* **Core Concepts:** Water properties (polarity, hydrogen bonding, adhesion, cohesion, high specific heat); Carbon chemistry; The 4 Macromolecules (Carbohydrates, Lipids, Proteins, Nucleic Acids); Monomers vs. Polymers (dehydration synthesis vs. hydrolysis); Enzyme structure, active sites, induced fit, activation energy; Factors affecting enzyme velocity (temperature, pH, substrate concentration, competitive/non-competitive inhibitors); Chemical indicators (Benedict's, Lugol's Iodine, Biuret, Sudan III).

#### Unit 02: Cell Architecture & Membrane Transport (Weeks 4–6) — `SB1.a, SB1.d`
* **Status:** In Progress / Current (`units/unit-02-cells-and-transport/`)
* **Core Concepts:** Cell Theory & historical contributors (Hooke, Leeuwenhoek, Schleiden, Schwann, Virchow); Prokaryotic vs. Eukaryotic ultrastructure; Organelles of endomembrane system (Nucleus, RER, SER, Golgi apparatus, Lysosomes, Vacuoles); Energy organelles (Mitochondria with cristae, Chloroplasts with thylakoids/stroma); Endosymbiotic Theory; Fluid Mosaic Model of plasma membrane (phospholipid bilayer, amphipathic nature, cholesterol, integral/peripheral proteins, glycoproteins); Passive Transport (Simple diffusion, facilitated diffusion via channels/carriers, osmosis); Tonicity dynamics (hypertonic, hypotonic, isotonic; plasmolysis, turgor pressure, crenation, lysis); Active Transport (Primary ATP pumps, Sodium-Potassium ATPase pump 3 Na+ out / 2 K+ in, bulk transport via endocytosis/exocytosis, phagocytosis vs. pinocytosis); Surface area-to-volume ratio limits on cell size.

#### Unit 03: Cellular Energetics (Weeks 7–9) — `SB1.e`
* **Standard:** *Develop and use models to explain the role of cellular reproduction and energy transformation.*
* **Directory:** `units/unit-03-cellular-energetics/`
* **Core Concepts:**
  * **ATP/ADP Cycle:** High-energy phosphate bonds, phosphorylation, coupled reactions.
  * **Photosynthesis:** Chemical equation ($6\text{CO}_2 + 6\text{H}_2\text{O} \to \text{C}_6\text{H}_{12}\text{O}_6 + 6\text{O}_2$), chloroplast anatomy (thylakoid membrane, grana, stroma), chlorophyll $a/b$ and accessory pigments.
  * **Light-Dependent Reactions:** Photosystem II & I, photolysis of water (releasing $\text{O}_2$), electron transport chain, proton gradient, ATP synthase (photophosphorylation), NADPH generation.
  * **Light-Independent Reactions (Calvin Cycle):** Carbon fixation via RuBisCO, reduction, RuBP regeneration, glucose production in the stroma.
  * **Cellular Respiration:** Chemical equation ($\text{C}_6\text{H}_{12}\text{O}_6 + 6\text{O}_2 \to 6\text{CO}_2 + 6\text{H}_2\text{O} + 36\text{--}38\text{ ATP}$), mitochondria anatomy (outer membrane, intermembrane space, inner folded cristae, matrix).
  * **Stages of Respiration:** Glycolysis (cytoplasm, anaerobic, net 2 ATP + 2 NADH), Pyruvate Oxidation / Link reaction, Krebs Cycle / Citric Acid Cycle (matrix, produces $\text{CO}_2$, ATP, NADH, $\text{FADH}_2$), Electron Transport Chain & Chemiosmosis (inner cristae, oxygen as terminal electron acceptor forming water, oxidative phosphorylation generating 32–34 ATP).
  * **Anaerobic Fermentation:** Lactic acid fermentation (animals & bacteria) vs. Alcoholic fermentation (yeast, ethanol + $\text{CO}_2$); regeneration of $\text{NAD}^+$ to maintain glycolysis.

#### Unit 04: Cellular Reproduction & Cell Cycle (Weeks 10–11) — `SB1.b`
* **Standard:** *Develop and use models to explain the role of cellular reproduction in maintaining genetic continuity.*
* **Directory:** `units/unit-04-cellular-reproduction/`
* **Core Concepts:**
  * **Cell Cycle Architecture:** Interphase ($\text{G}_1$ growth, $\text{S}$ phase DNA replication, $\text{G}_2$ preparation), M phase (Mitosis & Cytokinesis), $\text{G}_0$ resting phase.
  * **Mitosis Stages:** Prophase (chromatin condenses into chromosomes, nuclear envelope breaks down, spindle forms), Metaphase (chromosomes align at equatorial metaphase plate), Anaphase (sister chromatids separated by spindle fibers at centromere), Telophase (nuclei reform, chromosomes decondense).
  * **Cytokinesis:** Cleavage furrow via microfilaments (animals) vs. Cell plate formation via Golgi vesicles (plants).
  * **Cycle Regulation & Checkpoints:** $\text{G}_1/\text{S}$ checkpoint (restriction point), $\text{G}_2/\text{M}$ checkpoint, M-spindle (SAC) checkpoint; cyclins and cyclin-dependent kinases (CDKs); contact inhibition; apoptosis (programmed cell death).
  * **Disruption & Cancer:** Oncogenes, mutated tumor suppressor genes ($p53$), benign vs. malignant tumors, metastasis.
  * **Stem Cells & Differentiation:** Totipotent, pluripotent, multipotent stem cells; differential gene expression leading to specialized cells (erythrocytes, neurons, myocytes).

#### Unit 05: Molecular Genetics & Gene Expression (Weeks 12–14) — `SB2.a, SB2.b`
* **Standard:** *Obtain, evaluate, and communicate information on how the structures of DNA and RNA lead to gene expression.*
* **Directory:** `units/unit-05-gene-expression/`
* **Core Concepts:**
  * **Nucleic Acid Structure:** DNA double helix, antiparallel strands ($5' \to 3'$ vs. $3' \to 5'$), phosphodiester backbone, complementary base pairing (Chargaff's rules: A=T with 2 hydrogen bonds, G≡C with 3 hydrogen bonds).
  * **DNA Replication (Semi-Conservative):** Meselson-Stahl proof; replication fork enzymes: Helicase (unwinds), Single-Strand Binding Proteins (stabilizes), Topoisomerase/Gyrase (relieves supercoiling), Primase (RNA primer), DNA Polymerase III (synthesizes leading continuously and lagging via Okazaki fragments), DNA Polymerase I (removes primers), Ligase (seals nicks).
  * **The Central Dogma:** $\text{DNA} \xrightarrow{\text{Transcription}} \text{mRNA} \xrightarrow{\text{Translation}} \text{Protein}$.
  * **Transcription:** RNA polymerase binding to promoter (TATA box), elongation of mRNA strand, termination; pre-mRNA processing in eukaryotes (5' methylguanosine cap, 3' poly-A tail, spliceosome intron excision and exon splicing).
  * **Translation:** Ribosome structure (A, P, E sites), tRNA structure with anticodon and attached amino acid; Codons on mRNA; Universal genetic code chart; Initiation (AUG Start codon / Methionine), Elongation (peptide bond synthesis), Termination (UAA, UAG, UGA Stop codons, release factor).
  * **Genetic Mutations:** Point mutations (Silent, Missense, Nonsense); Frameshift mutations (Nucleotide insertion or deletion altering the reading frame); Chromosomal mutations (inversion, translocation, duplication, deletion); Mutagens and phenotypic consequences.

#### Unit 06: Mendelian & Complex Genetics (Weeks 15–16 & 19–21) — `SB3.a, SB3.b, SB3.c`
* **Standard:** *Obtain, evaluate, and communicate information on how biological traits are passed on to successive generations.*
* **Directory:** `units/unit-06-genetics/`
* **Core Concepts:**
  * **Meiosis & Gametogenesis:** Meiosis I (reduction division: homologous chromosome separation) vs. Meiosis II (equational division: sister chromatid separation); Prophase I Synapsis & Crossing over (chiasmata); Metaphase I Independent assortment; Spermatogenesis (4 viable sperm) vs. Oogenesis (1 viable ovum + 3 polar bodies); Sources of genetic variation.
  * **Mendelian Principles:** Law of Segregation, Law of Independent Assortment, Dominant vs. Recessive alleles, Genotype (homozygous dominant, heterozygous, homozygous recessive) vs. Phenotype; Monohybrid and Dihybrid Punnett square probability ($9:3:3:1$ ratio).
  * **Non-Mendelian & Complex Inheritance:** Incomplete dominance (intermediate blend, e.g., red $\times$ white $=$ pink); Codominance (both expressed simultaneously, e.g., roan coat, AB blood); Multiple alleles (ABO blood group with $I^A$, $I^B$, $i$); Polygenic inheritance (continuous distribution, skin color, height); Pleiotropy; Epistasis.
  * **Sex-Linked Inheritance & Pedigrees:** X-linked recessive disorders (hemophilia, red-green color blindness, Duchenne muscular dystrophy); Carrier females; Pedigree chart reading and tracking inheritance patterns across generations; Karyotyping, nondisjunction, and aneuploidy (Trisomy 21 Down syndrome, Turner syndrome XO, Klinefelter syndrome XXY).

#### Unit 07: Biotechnology & Genetic Engineering (Weeks 22–24) — `SB2.c, SB4.a`
* **Standard:** *Construct an argument based on evidence about the societal, ethical, and environmental impacts of biotechnology.*
* **Directory:** `units/unit-07-biotechnology/`
* **Core Concepts:**
  * **Restriction Enzymes & Gel Electrophoresis:** Recognition sequences (palindromes), sticky ends vs. blunt ends; Agarose gel mechanics, negative DNA charge migrating toward positive anode; Fragment separation by size (small fragments travel faster/farther); DNA fingerprinting in forensics and paternity testing.
  * **Recombinant DNA & Transformation:** Bacterial plasmids as cloning vectors, insertion of target genes (e.g., human insulin), DNA ligase; Heat-shock calcium chloride transformation, antibiotic selection markers (e.g., $amp^R$) to identify transformants.
  * **Polymerase Chain Reaction (PCR):** Denaturation ($95^\circ\text{C}$), Annealing ($55^\circ\text{C}$), Extension ($72^\circ\text{C}$); Taq polymerase thermostability; Exponential amplification of DNA.
  * **Modern Tools & Ethics:** CRISPR-Cas9 targeted genome editing, guide RNA (gRNA); Genetically Modified Organisms (GMOs) in agriculture; Gene therapy; Bioethics regarding human germline editing, ecological risks, and patenting genetic materials.

#### Unit 08: Evolution & Natural Selection (Weeks 25–28) — `SB6.a–e`
* **Standard:** *Obtain, evaluate, and communicate information to explain how evolution leads to biodiversity.*
* **Directory:** `units/unit-08-evolution/`
* **Core Concepts:**
  * **Mechanisms of Natural Selection:** Overproduction, variation, struggle for existence, differential survival and reproduction ("survival of the fittest"); Adaptations (structural, physiological, behavioral); Environmental selective pressures.
  * **Patterns of Selection:** Directional selection, Stabilizing selection, Disruptive selection; Sexual selection and artificial selection.
  * **Lines of Evidence for Evolution:** Fossil record (transitional fossils, Law of Superposition, radiometric dating); Comparative Anatomy (Homologous structures showing common ancestry, Analogous structures from convergent evolution, Vestigial organs); Comparative Embryology; Molecular/Biochemical homology (DNA sequence and cytochrome $c$ amino acid comparison).
  * **Population Genetics & Microevolution:** Gene pool, allele frequency shifts; Genetic drift (Bottleneck effect, Founder effect); Gene flow (migration); Mutations; Non-random mating; Hardy-Weinberg equilibrium conditions ($p + q = 1$, $p^2 + 2pq + q^2 = 1$).
  * **Macroevolution & Speciation:** Biological Species Concept; Reproductive isolation (Pre-zygotic: geographic, behavioral, temporal, mechanical, gametic; Post-zygotic: hybrid inviability, hybrid sterility); Allopatric speciation vs. Sympatric speciation; Rates of evolution (Gradualism vs. Punctuated Equilibrium); Adaptive radiation.

#### Unit 09: Ecology & Ecosystem Dynamics (Weeks 29–32) — `SB5.a–c`
* **Standard:** *Assess the dependence of all organisms on one another and the flow of energy and matter within their ecosystems.*
* **Directory:** `units/unit-09-ecology/`
* **Core Concepts:**
  * **Ecological Hierarchy:** Organism $\to$ Population $\to$ Community $\to$ Ecosystem $\to$ Biome $\to$ Biosphere; Biotic factors vs. Abiotic factors; Habitats and ecological niches (fundamental vs. realized; Competitive Exclusion Principle).
  * **Trophic Dynamics & Energy Flow:** Producers/Autotrophs (photosynthetic, chemosynthetic) vs. Consumers/Heterotrophs (herbivores, carnivores, omnivores, detritivores, decomposers); Food chains and food webs; Energy pyramids, biomass pyramids, pyramids of numbers; The 10% Ecological Rule of energy transfer (90% lost as heat and metabolic work).
  * **Biogeochemical Cycling:** Water cycle (evaporation, transpiration, condensation, precipitation, runoff); Carbon cycle (photosynthesis, cellular respiration, combustion, fossil fuel reservoirs); Nitrogen cycle (nitrogen fixation by rhizobium bacteria, nitrification, assimilation, ammonification, denitrification); Phosphorus cycle (weathering of rock, sedimentation, lack of atmospheric phase).
  * **Community Interactions:** Symbiosis (Mutualism $+/+$, Commensalism $+/0$, Parasitism $+/-$); Predation, herbivory, competition (interspecific vs. intraspecific); Keystone species and trophic cascades (e.g., sea otters, wolves).
  * **Population Ecology:** Exponential growth ($J$-curve) vs. Logistic growth ($S$-curve); Carrying capacity ($K$); Limiting factors: Density-dependent (competition, predation, disease) vs. Density-independent (natural disasters, temperature, drought).
  * **Ecological Succession:** Primary succession (starts on bare rock, pioneer species lichens/mosses, soil formation) vs. Secondary succession (follows disturbance like wildfire/clearing, begins with intact soil); Climax community.
  * **Human Impacts:** Biomagnification of toxins (DDT, microplastics, mercury); Eutrophication (fertilizer runoff, algal blooms, hypoxia, fish kills); Invasive species impact on native biodiversity; Deforestation, habitat fragmentation, greenhouse effect, and ocean acidification.

#### Unit 10: Diversity of Life, Taxonomy & Cladistics (Weeks 33–34) — `SB4.a, SB4.b`
* **Standard:** *Assess how organisms are classified based on evolutionary relationships and cellular structure.*
* **Directory:** `units/unit-10-diversity-of-life/`
* **Core Concepts:**
  * **Taxonomic Hierarchy:** Domain $\to$ Kingdom $\to$ Phylum $\to$ Class $\to$ Order $\to$ Family $\to$ Genus $\to$ Species ("Dear King Philip Came Over For Good Soup"); Binomial nomenclature (Carolus Linnaeus: capitalized *Genus*, lowercase *species*, italicized).
  * **The 3 Domains & 6 Kingdoms:**
    * Domain Archaea (Kingdom Archaebacteria: extremophiles, methanogens, halophiles, ether-linked lipids, lack peptidoglycan).
    * Domain Bacteria (Kingdom Eubacteria: true bacteria, ester-linked lipids, peptidoglycan cell walls, Gram-positive vs. Gram-negative).
    * Domain Eukarya: Kingdom Protista (paramecium, amoeba, algae), Kingdom Fungi (chitin cell walls, heterotrophic absorption, hyphae/mycelium), Kingdom Plantae (cellulose cell walls, autotrophic, chloroplasts), Kingdom Animalia (multicellular, heterotrophic ingestion, no cell walls).
  * **Dichotomous Keys:** Step-by-step paired contrasting statements to identify unknown organisms.
  * **Phylogenetics & Cladistics:** Cladograms and phylogenetic trees; Nodes (common ancestors), Sister taxa, Outgroups, Root; Derived characters (synapomorphies) vs. ancestral traits; Clades (monophyletic groups); Interpreting evolutionary divergence from molecular data.
  * **Viruses:** Viral structure (capsid protein coat, nucleic acid genome DNA or RNA, optional viral envelope); Non-living status (acellular, no independent metabolism, obligate intracellular parasite); Lytic cycle (rapid host cell lysis and virion release) vs. Lysogenic cycle (provirus/prophage integration into host genome, dormancy, excision upon stress); Retroviruses (reverse transcriptase).

---

## 🛠️ Part 2: Step-by-Step New Unit Ingestion Playbook

Follow this standardized 6-phase procedure whenever Dr. Irwin releases materials for a new unit on Canvas.

```
┌────────────────────────────────────────────────────────────────────────┐
│                      NEW UNIT INGESTION WORKFLOW                       │
├─────────────────┬──────────────────────────────────────────────────────┤
│ Phase 1: Ingest │ Download Canvas PDFs/PPTs ➔ Place in materials/pdf/ │
│ Phase 2: Digest │ Extract high-yield notes & tables ➔ materials/md/   │
│ Phase 3: Build  │ Generate interactive self-grading HTML test suite    │
│ Phase 4: Wire   │ Update unit README, tests index, and main dashboard  │
│ Phase 5: Audit  │ Run automated script to verify 100% valid links      │
│ Phase 6: Deploy │ Git commit & push ➔ Live on GitHub Pages             │
└─────────────────┴──────────────────────────────────────────────────────┘
```

---

### Phase 1: Material Acquisition & File Ingestion
1. **Download source files from Canvas:** Retrieve lecture slide decks, unit packets, reading guides, and teacher scenario cards.
2. **Standardized Directory Placement:**
   ```bash
   # Example for Unit 3 Cellular Energetics:
   mkdir -p units/unit-03-cellular-energetics/materials/pdf
   mkdir -p units/unit-03-cellular-energetics/materials/md
   mkdir -p units/unit-03-cellular-energetics/tests
   ```
3. **File Naming Rules:**
   * Keep original teacher filenames for PDFs in `materials/pdf/` for exact reference.
   * Avoid spaces in web-facing test files; use kebab-case: e.g., `test-photosynthesis-mechanisms.html`.

---

### Phase 2: Markdown Knowledge Extraction (`materials/md/`)
Convert complex teacher slide decks and lab packets into concise, searchable markdown study files.

Every converted markdown file in `materials/md/` must follow this structure:
1. **Title & Standard Header:** Specify the exact GSE Standard (`SB1.e`, etc.).
2. **Master Concept Summary:** 5–10 high-yield bullet points capturing essential testable mechanisms.
3. **High-Yield Terminology Table:**
   | Term | Definition / Molecular Role | Why Dr. Irwin Tests It (Trap Alert) |
   | :--- | :--- | :--- |
4. **Step-by-Step Pathway / Reaction Breakdown:** Chemical equations, reactants, products, and subcellular locations.
5. **Teacher Situation Scenarios:** Practice analysis questions modeled after classroom whiteboard questions.

---

### Phase 3: Interactive Practice Test Generation (`tests/`)

Every unit requires an interactive HTML test suite. Each test must be built as a self-contained, client-side web application.

#### Standard Test Specifications
* **Visual Theme:** Consistent with the modern glassmorphism dark/light design of Units 1 & 2 (Inter/system fonts, responsive layout, clear status badges).
* **Question Archetypes:**
  1. *Vocabulary Recall:* Direct definition identification.
  2. *Scenario Analysis:* Experimental data tables, solution concentration shifts, and enzyme velocity graphs.
  3. *Misconception Traps:* Answers featuring common student errors with explicit corrective explanations.
* **Core Interactive Features:**
  * Instant feedback with immediate green/red highlighting.
  * Detailed educational explanations for **both** correct and incorrect choices.
  * Running score counter and percentage calculator.
  * Filter/Restart buttons allowing the student to retry missed questions.
  * 100% offline and static-host compatible (no external backend required).

#### Standard Unit Test Suite Roster
For every unit, build:
1. `test-vocab-mastery.html` (30–50 flashcard-style MCQs covering all unit terminology).
2. `test-concept-application.html` (25–35 scenario, diagram, and graph analysis questions).
3. `test-unit-XX-summative-mastery.html` (50–60 comprehensive MCQs simulating the real unit exam).
4. `index.html` (Unit Test Hub linking all unit quizzes).

---

### Phase 4: Hub & Navigation Wiring
Once materials and tests are built, link them into the repository navigation architecture:

1. **Unit README (`units/unit-XX/README.md`):**
   * Overview, learning targets, table of all markdown study guides, PDF downloads, and test links.
2. **Unit Test Index (`units/unit-XX/tests/index.html`):**
   * Grid of test cards showing question count, difficulty, topic tags, and launch buttons.
3. **Master Dashboard (`index.html`):**
   * Update the unit card in the 10-Unit Master Grid from `Planned` to `Active`.
   * Add direct links to the new unit hub and primary tests.
4. **Master Schedule (`schedule/semester-1.md` or `semester-2.md`):**
   * Add direct relative links under the relevant week headers.
5. **Master README (`README.md`):**
   * Ensure quick-launch links point to the currently active weekly materials.

---

### Phase 5: Automated Verification & Link Integrity Audit

Never push code without running a link verification audit. Run this Python script to ensure 100% of relative links resolve:

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
    try:
        content = f.read_text(encoding="utf-8", errors="ignore")
    except Exception:
        continue
    content_no_code = re.sub(r"```[\s\S]*?```", "", content)
    html_links = re.findall(r"href=[\"\x27]([^\s\"\x27>]+)[\"\x27]", content_no_code)
    md_links = re.findall(r"\[[^\]]*\]\(([^)\s]+)\)", content_no_code)
    all_links = html_links + md_links

    for raw_link in all_links:
        if raw_link.startswith(("http://", "https://", "mailto:", "javascript:", "#")):
            continue
        clean_link = urllib.parse.unquote(raw_link.split("?")[0].split("#")[0])
        link_path = (f.parent / clean_link).resolve()
        checked += 1
        if not link_path.exists():
            broken.append((str(f.relative_to(root)), raw_link, str(link_path)))

print(f"Checked {checked} relative links across {len(html_md_files)} files.")
if broken:
    print(f"❌ Found {len(broken)} broken link(s):")
    for src, l, lp in broken:
        print(f"  {src} -> {l}")
    exit(1)
else:
    print("✅ All relative links are 100% valid! Zero broken links.")
'
```

---

### Phase 6: Git Commit & GitHub Pages Deployment

Deploy the validated unit cleanly:

```bash
# 1. Review status
git status

# 2. Stage all new unit files
git add units/unit-XX-* schedule/ index.html README.md

# 3. Commit with standard semantic message
git commit -m "Add Unit XX (Topic Name): materials, study guides, and test suite"

# 4. Push to GitHub
git push origin main

# 5. Verify live deployment
gh api /repos/MegaAntony/high-school-biology-i-honors/pages/builds --jq ".[0].status"
```

---

## 📋 Part 3: Ready-to-Use Unit Templates

### Template 1: Unit `README.md`

```markdown
# Unit XX: [Unit Name]
### Biology I Honors • Georgia Standards of Excellence: [GSE Codes, e.g., SB1.e]
*South Forsyth High School • Dr. Sarah Irwin*

---

## 🎯 Learning Objectives & State Standards
* **[Standard Code]:** [Full standard text description]
* **Target 1:** [Specific measurable student target]
* **Target 2:** [Specific measurable student target]

---

## 📚 Study Guides & High-Yield Notes (`materials/md/`)
* 📄 [Unit Overview & Detailed Vocab](materials/md/unit-XX-vocab-guide.md)
* 📄 [Lecture Slides & Concept Notes](materials/md/unit-XX-lecture-notes.md)
* 📄 [Situation Cards & Problem Solving](materials/md/unit-XX-situation-cards.md)

---

## 🧪 Interactive Practice Tests (`tests/`)
* ⚡ [Unit XX Master Test Hub](tests/index.html)
* 🗂️ [Vocabulary Mastery Test](tests/test-vocab-mastery.html) — *40 Questions*
* 🔬 [Concept & Scenario Practice](tests/test-concept-application.html) — *30 Questions*
* 🏆 [Summative Practice Exam](tests/test-unit-XX-summative-mastery.html) — *55 Questions*

---

## 📁 Teacher Source Documents (`materials/pdf/`)
* 📥 [Unit Packet PDF](materials/pdf/unit-XX-student-packet.pdf)
* 📥 [Lecture Slides Presentation PDF](materials/pdf/unit-XX-presentation.pdf)
```

---

### Template 2: Interactive Quiz Card Generator (HTML/JS Engine)

Use this verified template to build responsive quizzes with zero build tools or dependencies:

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Unit XX Practice Quiz | Biology I Honors</title>
  <script src="https://cdn.tailwindcss.com"></script>
  <style>
    body { font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, sans-serif; }
    .correct { background-color: #dcfce7 !important; border-color: #22c55e !important; color: #15803d !important; }
    .incorrect { background-color: #fee2e2 !important; border-color: #ef4444 !important; color: #b91c1c !important; }
  </style>
</head>
<body class="bg-slate-50 text-slate-800 p-4 md:p-8">
  <div class="max-w-3xl mx-auto">
    <!-- Header -->
    <header class="mb-6 pb-4 border-b border-slate-200">
      <a href="index.html" class="text-sm font-semibold text-emerald-600 hover:text-emerald-700">← Back to Unit Tests</a>
      <h1 class="text-2xl md:text-3xl font-bold mt-2 text-slate-900">Unit XX: Practice Assessment</h1>
      <p class="text-slate-600 text-sm mt-1">Biology I Honors • Dr. Irwin • Georgia Standard [Standard]</p>
      <div class="mt-4 flex items-center justify-between bg-white p-3 rounded-lg border border-slate-200 shadow-sm">
        <span id="score-display" class="font-medium text-slate-700">Score: 0 / 0 (0%)</span>
        <button onclick="resetQuiz()" class="px-3 py-1 bg-slate-100 hover:bg-slate-200 text-slate-700 text-sm rounded font-medium transition">Reset Quiz</button>
      </div>
    </header>

    <!-- Questions Container -->
    <div id="quiz-container" class="space-y-6"></div>
  </div>

  <script>
    const questions = [
      {
        q: "Sample question stem explaining a biological scenario or mechanism?",
        options: [
          "Incorrect distractor representing a common student misconception",
          "Correct answer based on scientific evidence",
          "Distractor with partially correct terms",
          "Distractor from another unrelated unit"
        ],
        answer: 1,
        explanation: "Detailed explanation clarifying why choice B is scientifically correct and why the other choices are incorrect."
      }
      // Add questions here...
    ];

    let answeredCount = 0;
    let correctCount = 0;

    function renderQuiz() {
      const container = document.getElementById('quiz-container');
      container.innerHTML = '';
      questions.forEach((item, index) => {
        const card = document.createElement('div');
        card.className = "bg-white p-6 rounded-xl border border-slate-200 shadow-sm transition";
        card.id = `q-${index}`;

        const qText = document.createElement('h3');
        qText.className = "font-semibold text-base md:text-lg text-slate-900 mb-4";
        qText.innerHTML = `<span class="text-emerald-600 mr-2">Q${index + 1}.</span>${item.q}`;
        card.appendChild(qText);

        const optsDiv = document.createElement('div');
        optsDiv.className = "space-y-2.5";

        item.options.forEach((opt, optIndex) => {
          const btn = document.createElement('button');
          btn.className = "w-full text-left p-3.5 rounded-lg border border-slate-200 text-slate-700 hover:border-emerald-400 hover:bg-emerald-50/50 text-sm font-medium transition flex items-start";
          btn.innerHTML = `<span class="w-6 h-6 rounded-full bg-slate-100 text-slate-600 text-xs flex items-center justify-center mr-3 shrink-0">${String.fromCharCode(65 + optIndex)}</span><span>${opt}</span>`;
          btn.onclick = () => selectOption(index, optIndex);
          optsDiv.appendChild(btn);
        });

        card.appendChild(optsDiv);

        const expDiv = document.createElement('div');
        expDiv.id = `exp-${index}`;
        expDiv.className = "hidden mt-4 p-4 rounded-lg bg-slate-50 border border-slate-200 text-xs md:text-sm text-slate-700";
        card.appendChild(expDiv);

        container.appendChild(card);
      });
    }

    function selectOption(qIdx, optIdx) {
      const card = document.getElementById(`q-${qIdx}`);
      const buttons = card.querySelectorAll('button');
      if (buttons[0].disabled) return;

      const q = questions[qIdx];
      buttons.forEach((b, i) => {
        b.disabled = true;
        if (i === q.answer) b.classList.add('correct');
        if (i === optIdx && i !== q.answer) b.classList.add('incorrect');
      });

      answeredCount++;
      if (optIdx === q.answer) correctCount++;

      const pct = Math.round((correctCount / answeredCount) * 100);
      document.getElementById('score-display').textContent = `Score: ${correctCount} / ${answeredCount} (${pct}%)`;

      const exp = document.getElementById(`exp-${qIdx}`);
      exp.innerHTML = `<strong>${optIdx === q.answer ? '✅ Correct!' : '❌ Incorrect.'}</strong> ${q.explanation}`;
      exp.classList.remove('hidden');
    }

    function resetQuiz() {
      answeredCount = 0;
      correctCount = 0;
      document.getElementById('score-display').textContent = "Score: 0 / 0 (0%)";
      renderQuiz();
    }

    renderQuiz();
  </script>
</body>
</html>
```

---

## 🎯 Part 4: Pre-Flight & Post-Flight Quality Checklist

Before considering any unit addition "Done", verify each item on this checklist:

### 1. Pre-Flight (Materials Ingestion)
- [ ] All teacher PDFs/PPTs stored in `units/unit-XX/materials/pdf/`.
- [ ] Converted markdown files in `units/unit-XX/materials/md/` contain no placeholder text.
- [ ] Vocabulary terms include exact GSE definitions and "Teacher Trap" explanations.
- [ ] Lab or classroom scenario questions documented.

### 2. Build & Assembly
- [ ] Vocabulary quiz built (`test-vocab-mastery.html`).
- [ ] Concept/Scenario application quiz built (`test-concept-application.html`).
- [ ] Summative mastery exam built (`test-unit-XX-summative-mastery.html`).
- [ ] Unit Test Index built (`units/unit-XX/tests/index.html`).
- [ ] Unit README created (`units/unit-XX/README.md`).

### 3. Navigation & Dashboard Integration
- [ ] Unit card in root `index.html` updated to active with correct relative paths.
- [ ] Semester calendar (`schedule/semester-1.md` or `semester-2.md`) updated with weekly schedule and deep links.
- [ ] Root `README.md` quick-launch bar updated if this is the active in-class unit.

### 4. Quality Assurance & Link Audit
- [ ] Link audit script executed with **0 broken links** reported.
- [ ] Interactive tests tested in browser (desktop + mobile viewport).
- [ ] Question answer keys and explanations verified against state standards.

### 5. Deployment & Remote Verification
- [ ] Git commit created with semantic message.
- [ ] Pushed to `origin main` on `https://github.com/MegaAntony/high-school-biology-i-honors`.
- [ ] GitHub Pages build status confirmed `"built"`.
- [ ] Live URL verified via `curl` returning HTTP 200.
