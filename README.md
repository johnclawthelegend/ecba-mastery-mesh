# ECBA Mastery Mesh

A single-page study companion for the **IIBA® Entry Certificate in Business Analysis™ (ECBA™)**, built around **BABOK® v3**.

🔗 **Live site:** https://johnclawthelegend.github.io/ecba-mastery-mesh/

## What's inside

- **Knowledge Map** — all six BABOK v3 Knowledge Areas and their tasks:
  1. Business Analysis Planning and Monitoring (5 tasks)
  2. Elicitation and Collaboration (5 tasks)
  3. Requirements Life Cycle Management (5 tasks)
  4. Strategy Analysis (4 tasks)
  5. Requirements Analysis and Design Definition (6 tasks)
  6. Solution Evaluation (5 tasks)
- **Master Mesh** — 30 concept rows linking BABOK concepts to the practice questions that test them.
- **Practice Exam** — 120 questions (three tests of 40), each with answer, explanation, and a link back to its concept.

## Exam facts (per the IIBA ECBA 2025 update)

| Item | Value |
| --- | --- |
| Questions | 50 |
| Duration | 75 minutes |
| Format | Multiple choice (standard + situation-based) |
| Pass mark | Not disclosed by IIBA — results are reported as performance indicators |
| Certifying body | IIBA |

## Build

The page is assembled from a content file and an HTML template:

```bash
python3 assemble_mesh.py   # ecba_full_content.txt + ecba_study_mesh_template.html -> index.html
```

The assembler parses the Knowledge Map, the three practice tests, and the Master Mesh, then injects them as a single `store` object into the template. It asserts 6 knowledge areas and 120 questions before writing output.

---

*Unofficial study aid. Not affiliated with or endorsed by IIBA. BABOK® and ECBA® are trademarks of the International Institute of Business Analysis.*
