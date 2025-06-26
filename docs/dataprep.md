# Data Preparation

This document outlines the main steps of extracting and preparing genetic sequence data for further analysis in the project.

---

## What Do We Do With the Data?

### Extraction

- **ID**
- **Gene name**
- **Positions** (start & end)
- **Strand orientation** (forward / reverse)
- **Sequence** (for length and base composition)

### Structuring

- The extracted information is stored in formats such as `.csv` for further processing and integration.

---

## Preprocessing Steps

- **Parsing:** Automated parsing of FASTA files to extract relevant fields.
- **Filtering:** Removal of incomplete or duplicate entries.
- **Feature Calculation:** Calculation of sequence length and nucleotide composition (A, T, C, G).
- **Data reduction:** For downstream analyses and Wikibase integration, only summary features (length, base counts, etc.) are stored instead of full sequences.

---

## Example Output

| ID      | Gene name | Start   | End     | Strand   | Length | A  | T  | C  | G  |
|---------|-----------|---------|---------|----------|--------|----|----|----|----|
| xyz123  | ffs       | 12345   | 12456   | forward  | 112    | 32 | 28 | 25 | 27 |

---

*For further details on tools and integration, see the respective documentation files in the repository.*
