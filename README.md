# Coding Agents Need a Theory of the Codebase, Not Just Code Generation

*A position paper*

📄 [Read the PDF](./theory-of-the-codebase.pdf)

## Abstract

Coding agents built on frontier language models resolve a majority of curated software-engineering benchmark tasks, yet degrade sharply outside them. This paper argues the cause is representational, not a matter of scale: even agents that move beyond flat text to structural representations — dependency graphs, call graphs, AST-derived structures — model a codebase only as an *artifact*, a snapshot of what the code currently is. They cannot capture *why* the code is that way, *which* of its structural properties are load-bearing constraints versus historical accident, or *how* team conventions have shifted over the repository's history. We develop this artifact-versus-decisions distinction through three failure modes structural graphs cannot represent by construction — intent, constraint provenance, and convention drift — survey a thinner literature already gesturing at this gap, and confront directly the strongest counterargument that sufficiently rich retrieval could recover this information without any new representation. We argue retrieval is a similarity operation and the relevant failures — precedence, cross-episode conflict, defeasibility — are not similarity problems, giving falsifiable criteria for telling the two apart. We close by sketching, at position-paper level, what an adequate representation would need to satisfy, and address the practical objections (cost, staleness, curation) any such approach must answer.

## Contents

| File | Description |
|---|---|
| `theory-of-the-codebase.tex` | LaTeX source |
| `references.bib` | BibTeX bibliography |
| `theory-of-the-codebase.pdf` | Compiled PDF |

## Building from source

Requires a standard TeX Live installation (`pdflatex`, `bibtex`).

```bash
pdflatex theory-of-the-codebase.tex
bibtex theory-of-the-codebase
pdflatex theory-of-the-codebase.tex
pdflatex theory-of-the-codebase.tex
```


## Citation

```bibtex
@misc{theory_of_the_codebase,
  title  = {Coding Agents Need a Theory of the Codebase, Not Just Code Generation},
  author = {ur Rehman, Ibad},
  year   = {2026},
  note   = {Position paper}
}
```
If you'd like to reference this work, see [CITATION.cff](CITATION.cff) or cite the PDF directly.

## Author

Ibad - Independent Researcher - August 2026


## License

This work is licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).
