# Copy provenance

This repository was prepared from the existing `ai-paper-val` project on
2026-10-25. The operation copies files; it does not move, rename, or delete the
source material. The destination's pre-existing Git repository is retained.
No commit, push, remote change, or publication is part of this operation.

## Selection and fidelity

The template source is `multi_agent_template/workflow1.6.2/`. Its 28 files are
copied unchanged into `toolkit/`, including its `.codex/` directory. The deployed
copies of these files in the 44 source packages were found to match the central
template during planning.

For each of the four year directories, the copy takes 16 canonical records from
each package, then follows links to eligible text dependencies within the current
review profile. The 704 canonical files and 467 linked dependencies are copied
unchanged, alongside the 28 toolkit files: 1,199 copied files in total. The copied
content initially totaled 35,948,245 bytes before generated indexes and documentation.

At the user's subsequent request, the copy was extended with all 189 original
source documents (188 PDFs and one supplementary workbook) at their existing
package-relative paths. It also adds the 61 evidence files directly linked by
the final HTML reports, so those reports' local file targets resolve. The copy
contains 1,449 copied files from that source-document update, whose source
contents total 273,827,106 bytes before generated indexes and documentation. Five HTML copies additionally receive
53 empty anchor spans to repair pre-existing candidate-navigation targets. No
report text changes, and removing those marked spans restores the exact original
HTML. All other previously copied toolkit and review files remain byte-identical.

The subsequently requested English tall workflow PNG is copied unchanged from
`paper_writting/main/slides/workflow_1_6_2_EN_tall.png` to
`assets/workflow_1_6_2_EN_tall.png` and embedded in the root README. This is an
explicit exception for one file, not inclusion of the manuscript directory.
That image addition brought the total to 1,450 copied files and 274,893,159 source bytes.

The user subsequently requested the four completed v2.4.1 R_Bulun workbooks
located directly under the source `human_adjudication/` folder. These files are
copied unchanged into the destination folder of the same name, with a new
guide and per-paper workbook/worksheet locators in `results/index.csv`. No
nested reviewer-run folders or other versions are copied. The current total
is 1,454 copied files and 275,283,424 source bytes.

The source-relative and destination-relative paths, byte counts, categories, and
SHA-256 hashes are in [migration_manifest.csv](migration_manifest.csv). The
`sha256` column records source bytes and `destination_sha256` records the copy;
they differ only for the five HTML files with anchor additions. The exact fixes
are listed in [results/html_navigation_fixes.csv](results/html_navigation_fixes.csv).
This manifest covers copied files. The new repository README, data-availability and
copy notes, results guide, indexes, omission manifest, Git ignore rules, and copy
validation record are newly generated support files, not historical artifacts.

The copy never traverses symlinks. The requested workflow PNG and four completed
workbooks are explicit exceptions to the earlier source exclusions; all other
excluded private/work directories and contents remain outside the copy. It also excludes follow-up packets, old profiles,
bulk extraction caches, environments, and the source Git history. Selected
directly linked evidence records and one image are included; whole cache
directories are not copied. Linked text inventories can still mention omitted paths.

## Verification

Mechanical checks cover copied-file hashes against the source and staging copy,
the 44-package index and 440 canonical candidate count, input-file hashes, the
exclusion rules, local link classification, Python syntax, and TOML parsing.
The four completed workbooks also pass XLSX ZIP-integrity and SHA-256 checks;
their worksheet names cover all 44 indexed paper packages. Cell judgments are
not reinterpreted or modified.
The source-document update additionally checks all final HTML file targets and
the validity of their PDF page-fragment bounds against the bundled PDFs.
These checks do not execute the scientific workflow, call models, rerun human
adjudication, or validate scientific conclusions. The repository-level result is
recorded in [copy_validation.json](copy_validation.json), separately from the
historical per-package review-validation files.

Source-project reports remain unchanged. Target HTML copies receive only the
documented navigation aliases; their scientific content is unchanged. Secondary
records may still refer to unavailable derivatives or contain pre-existing
formatting issues. The omission manifest makes that boundary explicit, and no
historical review is presented as newly scientifically validated.
