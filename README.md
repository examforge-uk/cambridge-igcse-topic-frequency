# Cambridge IGCSE & O Level topic frequency dataset (2020–2025)

How often each syllabus topic has been tested in real Cambridge IGCSE and O Level past papers, by marks,
questions and year: **2,492 past papers across 23 subjects, 2020–2025**.

Built by [ExamForge](https://examforge.uk), where every number here links to the real questions behind it:
[see what Cambridge tests most](https://examforge.uk/stats).

## What's inside

| File | One row per | Use it for |
|---|---|---|
| [`data/subjects.csv`](data/subjects.csv) | subject | papers analysed and topics tracked per syllabus |
| [`data/topics.csv`](data/topics.csv) | subject × topic | total marks, questions, how many years it appeared, first/last seen, longest gap |
| [`data/topics_by_year.csv`](data/topics_by_year.csv) | subject × topic × year | trends: questions and marks per year |
| [`data/papers_included.csv`](data/papers_included.csv) | paper | exactly which papers were counted |

Direct CSV links (for spreadsheets / pandas): `https://raw.githubusercontent.com/examforge-uk/cambridge-igcse-topic-frequency/main/data/topics.csv`

## Subjects

| Qualification | Subject | Code | Papers | Topics | Interactive |
|---|---|---|---|---|---|
| Cambridge IGCSE | Business Studies | 0264 | 84 | 29 | [most-tested topics](https://examforge.uk/igcse-topical-past-papers/business-0264/most-tested-topics) |
| Cambridge IGCSE | ICT | 0417 | 42 | 57 | [most-tested topics](https://examforge.uk/igcse-topical-past-papers/ict-0417/most-tested-topics) |
| Cambridge IGCSE | Accounting | 0452 | 82 | 27 | [most-tested topics](https://examforge.uk/igcse-topical-past-papers/accounting-0452/most-tested-topics) |
| Cambridge IGCSE | Economics | 0455 | 84 | 36 | [most-tested topics](https://examforge.uk/igcse-topical-past-papers/economics-0455/most-tested-topics) |
| Cambridge IGCSE | Computer Science | 0478 | 71 | 34 | [most-tested topics](https://examforge.uk/igcse-topical-past-papers/computer-science-0478/most-tested-topics) |
| Cambridge IGCSE | Islamiyat | 0493 | 48 | 34 | [most-tested topics](https://examforge.uk/igcse-topical-past-papers/islamiyat-0493/most-tested-topics) |
| Cambridge IGCSE | Mathematics | 0580 | 168 | 73 | [most-tested topics](https://examforge.uk/igcse-topical-past-papers/extended-mathematics-0580/most-tested-topics) |
| Cambridge IGCSE | Additional Mathematics | 0606 | 84 | 76 | [most-tested topics](https://examforge.uk/igcse-topical-past-papers/additional-mathematics-0606/most-tested-topics) |
| Cambridge IGCSE | Biology | 0610 | 250 | 66 | [most-tested topics](https://examforge.uk/igcse-topical-past-papers/biology-0610/most-tested-topics) |
| Cambridge IGCSE | Chemistry | 0620 | 248 | 55 | [most-tested topics](https://examforge.uk/igcse-topical-past-papers/chemistry-0620/most-tested-topics) |
| Cambridge IGCSE | Physics | 0625 | 251 | 26 | [most-tested topics](https://examforge.uk/igcse-topical-past-papers/physics-0625/most-tested-topics) |
| Cambridge IGCSE | Combined Science | 0653 | 220 | 85 | [most-tested topics](https://examforge.uk/igcse-topical-past-papers/combined-science-0653/most-tested-topics) |
| Cambridge IGCSE | Co-ordinated Sciences | 0654 | 238 | 112 | [most-tested topics](https://examforge.uk/igcse-topical-past-papers/co-ordinated-sciences-0654/most-tested-topics) |
| Cambridge IGCSE | Environmental Management | 0680 | 79 | 53 | [most-tested topics](https://examforge.uk/igcse-topical-past-papers/environmental-management-0680/most-tested-topics) |
| Cambridge O Level | Islamic Studies | 2068 | 30 | 15 | [most-tested topics](https://examforge.uk/o-level-topical-past-papers/islamic-studies-o-level-2068/most-tested-topics) |
| Cambridge O Level | Economics | 2281 | 48 | 39 | [most-tested topics](https://examforge.uk/o-level-topical-past-papers/economics-o-level-2281/most-tested-topics) |
| Cambridge O Level | Mathematics (Syllabus D) | 4024 | 48 | 42 | [most-tested topics](https://examforge.uk/o-level-topical-past-papers/mathematics-d-4024/most-tested-topics) |
| Cambridge O Level | Additional Mathematics | 4037 | 48 | 79 | [most-tested topics](https://examforge.uk/o-level-topical-past-papers/additional-mathematics-4037/most-tested-topics) |
| Cambridge O Level | Physics | 5054 | 94 | 63 | [most-tested topics](https://examforge.uk/o-level-topical-past-papers/physics-o-level-5054/most-tested-topics) |
| Cambridge O Level | Chemistry | 5070 | 95 | 49 | [most-tested topics](https://examforge.uk/o-level-topical-past-papers/chemistry-o-level-5070/most-tested-topics) |
| Cambridge O Level | Biology | 5090 | 84 | 52 | [most-tested topics](https://examforge.uk/o-level-topical-past-papers/biology-o-level-5090/most-tested-topics) |
| Cambridge O Level | Business Studies | 7115 | 48 | 24 | [most-tested topics](https://examforge.uk/o-level-topical-past-papers/business-studies-o-level-7115/most-tested-topics) |
| Cambridge O Level | Accounting | 7707 | 48 | 27 | [most-tested topics](https://examforge.uk/o-level-topical-past-papers/accounting-o-level-7707/most-tested-topics) |

## Columns (topics.csv)

- `question_count`, `total_marks`: questions tagged to the topic and the marks they carry, 2020–2025.
- `years_present` / `years_in_range`: in how many of the years the topic appeared.
- `recurrence`: `recurring_every_year`, `recurring` or `one_off`.
- `first_seen`, `last_seen`, `longest_gap_years`: appearance history within the range.
- `examforge_url`: the topic's page, with the real questions and their mark schemes.

## How it was built

1. Every published question paper and its official mark scheme, catalogued by syllabus, paper, variant and session.
2. Each question matched to the topics of the official Cambridge syllabus (AI-assisted, checked by a practising IGCSE teacher before a subject goes live).
3. Marks and questions counted per topic and year from the mark-scheme totals.

Full method: [https://examforge.uk/how-it-works](https://examforge.uk/how-it-works)

## Limitations (read before drawing conclusions)

- **Descriptive, not predictive.** A topic that appeared every year can still be left out next time.
- **A question that tests two topics counts for both**, so topic totals overlap and sum to more than the paper total.
- **Coverage varies by subject** (see `papers_included.csv`); some subjects have fewer papers or sessions.
- **Business 0264** replaces Business Studies 0450 from 2027; its counts come from 0450 papers tagged to the 0264 syllabus.
- Tagging is AI-assisted and teacher-checked; individual tags can be imperfect.

## Licence and citation

[CC BY 4.0](LICENSE): free to use, share and adapt, including commercially, **with attribution**:

> Topic frequency data from ExamForge (examforge.uk), 2026-09-29.

Please link to https://examforge.uk/stats where you use it. See [CITATION.cff](CITATION.cff) for a formal citation.

Not affiliated with or endorsed by Cambridge University Press & Assessment. Cambridge, IGCSE and O Level
are its trademarks; syllabus topic names are used descriptively. This dataset contains no question text,
mark-scheme text or images.

_Last updated 2026-09-29._
