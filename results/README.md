# Application records

The [index](index.csv) lists 44 packages and 440 registered AI candidates.
Each package now also includes its original paper, protocol, SAP, and supplements
at the original package-relative paths. The 188 PDFs and supplementary workbook
are enumerated in [source_files.csv](source_files.csv).
Evidence records and report text retain their original content. Five HTML copies
have navigation-only anchor additions, listed in [html_navigation_fixes.csv](html_navigation_fixes.csv).
Historical candidate IDs, claims, evidence states, and limitations have not been
rewritten or updated from later human judgments.

## Selection

Each package retains its two `final_report_1_6_2` files and these canonical files
under `.ai_paper_validation/review_1_6_2/`:

- `source_inventory.md`, `source_coverage.md`, and source hashes before/after;
- `candidate_ledger.md` and `screening/inclusion_screen.md`;
- `verification/evidence_recheck.md` and `quality/evidence_quality_audit.md`;
- `routing_preflight.md`, `run_state.md`, `agent_execution_manifest.md`, and
  `tooling_record.md`;
- `limitations.md` and `review_validation.json`.

Text files referenced by these records are included recursively when they belong
to the same current review profile. This includes relevant inventories, checking
records, audit parts, and hash-check logs. A few package-root policy documents
are retained because the reports directly link to them; agent configuration and
helper code are supplied once in `toolkit/`.

The source-document update additionally includes 61 evidence files that the final
HTML reports link to directly: 57 Markdown records, three JSON records, and one
image. This is a link-based selection, not a copy of entire extraction or OCR
directories. Source-document links retain their original relative paths.

## Local links

[omitted_links.csv](omitted_links.csv) records links whose targets are outside
this copy. Paths in its `referring_file` column are relative to the repository
root. The remaining entries refer to secondary-record dependencies, excluded
human-review materials, or pre-existing malformed markup. There are no unbundled
original inputs or unavailable direct local file links in the 44 final HTML
reports. The manifest does not imply that excluded targets never existed.

Two pre-existing Markdown expressions in the `jama.2019.2210` supporting
statistical records resemble links to `.99` inside a mathematical calculation.
They were inspected and classified as malformed mathematical markup, not missing
scientific source files. The original text was preserved.

All other recognized local file links in the selected records either resolve to
an included file or appear in the omission manifest. The scan checks Markdown
links and HTML `href`/`src` references, not arbitrary paths in prose or code spans.
Final HTML source-file targets, PDF page-fragment bounds, and internal anchor
targets are checked separately in the repository-level validation record. Five
HTML copies needed 53 empty anchor aliases at their existing candidate headings;
removing those added spans restores the exact original HTML bytes. Browser-specific
PDF/Office display behavior is not certified by a file-link check.

Open each final HTML report locally with the repository structure intact to follow
its source links. Some supporting records still cite omitted OCR/extraction caches
or later review records; those omissions do not change the historical AI findings.
The repository includes all original inputs, but not every intermediate artifact
or every subsequent review record. The four completed adjudication workbooks
are included separately in [human_adjudication/](../human_adjudication/README.md);
`index.csv` identifies the matching workbook and worksheet for each paper.

`review_validation.json` describes the original full package at its recorded run.
Do not rerun a scientific review in this directory or interpret its historical
`PASS` as a new validation of this reduced copy. Copy integrity is checked
separately in [copy_validation.json](../copy_validation.json).
