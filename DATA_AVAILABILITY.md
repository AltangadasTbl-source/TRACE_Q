# Data availability and scope

## Included

- Workflow 1.6.2 instructions, ten agent presets, project configuration, rules,
  helper scripts, settings, and report styling.
- AI-stage final reports and selected provenance for 44 trial packages:
  10 assigned to 2018, 9 to 2019, 10 to 2024, and 15 to 2025.
- Original candidate counts: 115, 79, 113, and 133, respectively (440 total).
- Source inventories, source hashes, review coverage, run and agent records,
  limitations, screening/recheck/audit records, and linked text dependencies.
- All 189 original input files: 188 PDFs and one supplementary XLSX workbook.
- Four completed v2.4.1 R_Bulun adjudication workbooks, one for each selected year.
  These are separate from the supplementary workbook supplied with a trial report.
- The 61 additional evidence files directly linked by the final HTML reports:
  57 Markdown records, three JSON records, and one evidence image.

The selection preserves existing year assignments; the year in a DOI can differ
from the package's assigned publication year. Article DOI links in the indexes
are constructed from package identifiers and were not checked over the network
during copying. They identify the article; they are not direct download URLs for
each supplement.

## Bundled original inputs

[results/source_files.csv](results/source_files.csv) lists all 189 input files
(188 PDFs and one XLSX workbook), their package-relative names, and their recorded
SHA-256 hashes. They are copied into `results/<year>/<paper_id>/` at those exact
paths, with `bundled=yes` in the index. The copies were checked byte for byte
against the original files and the hashes recorded for the historical review.

Keep these filenames and directory relationships when downloading or moving the
repository so that local report links continue to work. A publisher's subsequently
revised file may not match the version used for the historical review. Use a
separate working directory for any new review; keep these historical records intact.

Bulk OCR text, rendered pages, extracted tables, and other caches are not bundled.
Only the additional files needed by direct HTML links were selected, including
one evidence image. Inventories and secondary records can still describe omitted
assets; these remaining links are recorded in `results/omitted_links.csv`.

The English tall workflow PNG is included in `assets/` and displayed in the
root README. This single presentation image was explicitly requested from
`paper_writting/main/slides/`; no other manuscript or slide materials were copied.

## Excluded

No contents were copied from `review_records/` or `ignorance_documents/`.
Only the four explicitly requested completed workbooks were copied from the
source `human_adjudication/` root; its nested versions, other reviewers, and
working files remain excluded. Apart from the requested workflow PNG,
`paper_writting/` remains excluded. Follow-up review folders and review
packets were omitted. Old workflow versions, archived runs, the source Git
history, personal configuration, temporary environments, and caches were also
omitted.

The reports remain historical AI-stage records. The separate completed workbooks
retain all supplied decisions, notes, formulas, and formatting without rewriting.
Copy checks verify file integrity and paper-sheet coverage; they do not reassess
the judgments or rerun the manuscript analyses. See [the workbook guide](human_adjudication/README.md).
