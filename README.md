# Finance & Economics Literature Lab

A research tool by **M. R. Hoque** for exploring finance and economics literature and organizing evidence into main ideas, findings, limitations and possible next studies.

[Open the lab](https://rezoanhoque.github.io/tools/finance-literature/) · [See the animated pipeline](https://rezoanhoque.github.io/demos/finance-literature-pipeline/) · [Methods](https://rezoanhoque.github.io/tools/reproducibility/)

## What works today

- Search a public bibliographic snapshot spanning 27 journals (72,743 records in the October 11, 2026 release; historical coverage is incomplete).
- Inspect title and available abstract-term matches, journal/year filters and original paper links.
- Enter your own research topic across finance and economics; the interface goes directly to paper search.
- Inspect an optional four-column comparison: Keywords, Paper, Paper gap, Future gap. Missing limitations and unverified proposed questions are labeled explicitly.
- An implemented, separately hosted synthesis service can organize 3–8 accessible abstracts into a source-linked draft. Public activation is pending hosting configuration.

The full implementation uses Astro/TypeScript for the interface, Python for collection and Node.js/MySQL for the separate synthesis service. This repository is a project overview and a small replication exercise, not the production application.

## Try the method without an API

Copy `evidence-template.csv`. Choose three papers on a narrow topic, enter their verified DOIs, distinguish what you read (abstract or full paper), and fill in the evidence fields. Compare contexts and methods before proposing an extension. Record evidence that challenges your proposed direction.

`example-synthesis.json` is entirely synthetic and illustrates the output structure; it does not report actual papers or scientific findings. See `METHOD.md` for the workflow.

## Research limits

Missing evidence is a coverage limitation, not proof of a gap. An abstract is not a full-paper review. Suggested directions are hypotheses; novelty and identification assumptions require expert review. A reviewed 5,000-paper full-text core remains a collection target, not an existing collection.

## Public and private materials

This repository contains a summary, method and synthetic examples. Production source, server configuration, credentials, private PDFs and unpublished datasets are maintained privately. The browser-delivered website is necessarily inspectable by visitors. No credentials or private research are needed to repeat this exercise.

For collaboration or a specific replication request, [contact me](https://rezoanhoque.github.io/contact/).

The comparison includes a one-line proposed research direction with source links. The prepared backend rejects missing/mismatched returned DOIs and unknown model citation IDs. These checks establish source identity, not a hallucination-free interpretation; suggestions still require researcher review.

The current Crossref snapshot includes a version and import date for each record. Coverage totals are regenerated from the exact published JSON during every build. An OpenAlex import is being staged separately; the website does not claim it is already using that replacement.
