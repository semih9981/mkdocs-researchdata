# Processing & Analysis

## Data Processing

* Parsing of FASTA files
* Generation of sequence statistics
* Pattern recognition
* Classification by strand orientation

## Crunching with Python

Tools: `pandas`

Examples:

* Sequence length
* Nucleotide composition (A, T, C, G)

## Sequence Simplification & Export

### Simplified Representation Instead of Full Sequence

* Complete RNA sequences are often several thousand bases long
  Not suitable for Wikibase integration → decision for a shortened representation
* Instead: storage of length, base frequency, ID, type

### Export to Wikibase Cloud Instance

* Structured items: RNA, organism, length, strand, type
* SPARQL queries enable, for example:

  * All RNAs of a specific organism
  * Filtering by length ranges or RNA type
