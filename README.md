# Finance & Economics Literature Lab

A research tool by **M. R. Hoque** for finding finance, economics and related literature and downloading source-linked references.

[Open the lab](https://rezoanhoque.github.io/tools/finance-literature/) · [See the animated pipeline](https://rezoanhoque.github.io/demos/finance-literature-pipeline/) · [Methods](https://rezoanhoque.github.io/tools/reproducibility/)

## What works today

- Search a public bibliographic snapshot spanning 152 journals (193,233 records in the October 12, 2026 release; historical coverage is incomplete).
- Inspect title and available abstract-term matches, journal/year filters and original paper links.
- Enter your own research topic across finance and economics; the interface goes directly to paper search.
- Download shown references in Excel-compatible CSV, plain text, APA or RIS format. Compare papers is coming soon.
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

The planned comparison will include proposed research directions with source links. The prepared backend rejects missing/mismatched returned DOIs and unknown model citation IDs. These checks establish source identity, not a hallucination-free interpretation; suggestions still require researcher review.

The current Crossref snapshot includes a version and import date for each record. Coverage totals are regenerated from the exact published JSON during every build. An OpenAlex import is being staged separately; the website does not claim it is already using that replacement.

## Reference downloads

Download the shown references as Excel-compatible CSV, plain text, RIS, or APA text using Crossref citation formatting. Every reference includes its DOI; unavailable metadata is not invented. APA requires a live provider connection. Compare papers is coming soon.

New journal selection follows the [official ABDC list](https://abdc.edu.au/abdc-journal-quality-list/), B and above in finance, economics, econometrics, accounting and statistics. The 657 eligible titles are collection targets; the searchable catalog has partial archives and reports actual coverage.
