# Evidence grading protocol for Parkinson's questions

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.23175063.svg)](https://doi.org/10.5281/zenodo.23175063)

A versioned rulebook for grading published evidence against the questions people with Parkinson's ask. Version 0.2.1, dated 17 August 2026. Written by Ryan Smith, Navigator Consulting, Sunshine Coast, Australia.

## What it is

The protocol is a set of rules, each with an id, that take a study and a claim and produce a Priority grade for the claim. It covers what is allowed to count as evidence and at what trust level (source registry), which scale applies to which kind of claim (lanes), starting scores by study design, the modifiers applied to them, how modifiers stack, when general-population evidence may enter a Parkinson's question, caps, how scores map to tiers, claim-level grading across a body of evidence, funding and conflict rules, a layer for non-obvious findings, and the governance rules that keep the whole thing controlled.

The YAML file is the protocol. The HTML and PDF are rendered from it and cannot disagree with it.

Grades are derived, never stored. Every rule is a dial: change a value, bump the version, re-run, and diff the answers. A grade that feels wrong means a rule is wrong, and the fix is a rule change applied everywhere, not an override (G-5).

## What it is not

It is not medical advice. Every patient-facing output produced under this protocol carries this disclaimer, word for word (G-6):

> Priority ratings rank the strength of published evidence for each claim. They are not medical advice and are not instructions. Decisions about medication, diet or exercise belong with you and your treating team.

It is a draft. No clinician has reviewed it, and clinician sign-off is a release gate for anything patient-facing (G-4). The author has run it on two questions (lifestyle, and medication) to develop the rules. Those outputs are not published, and nothing graded under this protocol has been released.

## What is not here

The grading engine that applies these rules, the study and claim data, and the graded outputs are separate and are not in this repository. They are maintained by the author and are available as a service. Questions about the protocol itself can be raised as issues on this repository.

## Files

| File | What it is |
|---|---|
| `protocol/evidence-protocol-v0.2.1.yaml` | The protocol. This is the file to read, cite and diff |
| `protocol/evidence-protocol-v0.2.1.html` | The same, rendered for reading |
| `protocol/evidence-protocol-v0.2.1.pdf` | The same, as a four-page PDF |
| `CHANGELOG.md` | Every version from the first draft on 11 August 2026, copied from the protocol's own change record |
| `CITATION.cff` | How to cite it |
| `LICENSE` | CC BY 4.0 |

## Versioning

Semantic versioning. Any rule change bumps the version (G-1). Every published answer is stamped with the version that produced it (G-2). Rule changes are logged with their rationale and every affected claim is re-graded, with the diff shipping alongside the next answer (G-3). Wording changes to the disclaimer are rule changes.

## Licence

Creative Commons Attribution 4.0 International (CC BY 4.0). You may use, share and adapt the protocol, including commercially, provided you credit the author and link to the licence. See `LICENSE`.

## Citation

Smith, R. (2026). Evidence grading protocol for Parkinson's questions (version 0.2.1). Zenodo. https://doi.org/10.5281/zenodo.23175063

That DOI is for version 0.2.1. To link to the latest version, use the concept DOI: https://doi.org/10.5281/zenodo.23175062
