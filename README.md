# esai-gagasan-lomba

A Claude skill for writing **idea-based scientific essays** (*esai ilmiah gagasan*) for Indonesian competitions, in Bahasa Indonesia.

> Status: new repository. Download and dependency counts are still at zero.

## What problem it solves

Indonesian essay competitions (high school, university, general) ask for a *gagasan*: a proposed solution to a real problem, not a research report. Many entries lose points before the judges reach the content, because the title reads like research, the idea drifts outside the theme, or the sections don't tell one story. The guidance that fixes this mostly lives in mentor bootcamps and recorded sessions, which a student has to piece together alone.

This skill puts that guidance into one workflow Claude can follow step by step.

## What it does

| Stage | What Claude does |
|---|---|
| 0. Intake | Reads the competition rules: theme, subtheme, page/word limits, format, rubric, AI-use policy |
| 1. Early research | Maps current issues, key data and local cases, existing solutions and their gaps, related regulations |
| 2. Idea | Tests whether the idea is a proposed solution or an experiment, and reframes research-style ideas |
| 3. Title | Validates the title against a checklist, then offers three alternatives in different styles |
| 4-6. Draft | Allocates space, then structures the introduction and the discussion (eight blocks, from idea overview to feasibility, impact, projection, and innovation) |
| 7. Visuals | Picks one main figure that answers "how does this work" and specifies it before it is drawn |
| 8. Closing | Conclusion, references, appendix |
| 9. Style polish | Edits repetitive or machine-sounding prose |
| 10. QA | Applies reviewer-style corrections and reports only the checks that failed |

You can enter at any stage: with no idea, with a draft title, with a full manuscript, or with a request for only a figure or a style pass.

## Principles built into it

- **Idea, not research.** No hypotheses, variables, or statistical tests in the structure.
- **Stay inside the theme and subtheme.**
- **One thread.** The problem in the title returns in the data, the design, the advantages, the impact, and the conclusion, in the same terms.
- **The competition's own rules win.** If the guidelines conflict with the skill, the guidelines are followed.
- **No invented data.** Statistics, quotes, and references are never made up. Missing data is marked `[DATA DIPERLUKAN: ...]` with a pointer to where to find it. A fabricated citation can disqualify an entry.

## Sources

Built from mentor teaching material (Royhan Saydi, ANSA Academy, Bootcamp Esai) and the "Bedah Esai" material from Muda Kompetisi, which annotates two example essays. Parts marked **[TAMBAHAN]** in the skill are general additions, not from those sources.

The skill codifies criteria that mentors say often decide scores. It does not guarantee a win: idea quality, data, and compliance with the guidelines still decide.

## Usage notes

- If a competition regulates AI use or disclosure, follow its rules. The skill does not promise to pass AI detectors.
- The example titles and essay breakdowns are pattern references, not text to copy.

## Repository layout

```
esai-gagasan-lomba/
├── SKILL.md                      # workflow and principles
└── references/
    ├── riset-awal.md             # early research and research sheet
    ├── judul.md                  # title components, styles, validation
    ├── bank-judul.md             # title pattern examples
    ├── kasus-review.md           # real reviewer corrections
    ├── bedah-pendahuluan-penutup.md
    ├── bedah-pembahasan.md       # discussion blocks B1-B8
    ├── naskah.md                 # intro/discussion points, data rules
    ├── visual-gambar.md          # figures, schemes, prototypes, tables
    ├── anti-ai-ringkas.md        # writing style rules
    └── checklist-qa.md           # final checks
```

## Installation

add the way you load skills into Claude

## Track record

2 Essay's wins the province competition (Juriscripture Law Competition), and the other's wins national essay competition (Kreasi Fest 2026 #1, HKN #1)

## Author

Reza Adriansyah · +62 852-8265-8277

## License

[CHOOSE A LICENSE]
