---
name: technical-latex-report
description: Create and maintain rigorous Russian university technical reports in LaTeX, following the provided course template, using clear modular source files and compiling reproducible PDFs into a build directory.
---

# Technical LaTeX report

Use this skill for Russian university reports and laboratory work in computer science, mathematics and related technical subjects.

## Required workflow

1. Inspect the assignment, source code, data, previous report and the supplied LaTeX example before drafting.
2. Treat the assignment as authoritative for scope, source code as authoritative for implementation, and measured outputs as authoritative for results. Do not invent missing values; leave explicit placeholders in draft reports.
3. Follow the course structure when applicable: title page, contents, introduction, problem statement, mathematical description, implementation, results, analysis, conclusion and references.
4. Keep the report modular. Use `main.tex` as the ordered assembly point, `settings.tex` for shared formatting, semantically named chapter files, and dedicated directories for tables, figures and code excerpts.
5. Use direct Russian technical prose. Define notation, distinguish implementation facts from interpretations, and keep numerical claims traceable to source code, a derivation, a measurement or a table.
6. Avoid numbered and bulleted lists in report prose. Present advantages, limitations, steps and classifications in connected paragraphs unless the assignment explicitly requires a list. Structured data may remain in tables.
7. For function descriptions, state the function name, input, output, behavior and complexity where relevant; follow with a short source listing when it clarifies the implementation.
8. Use restrained typography close to the supplied course template: A4, 14pt body text, serif text, Russian language support, readable tables and code. Avoid manual spacing hacks and numbered equations unless references require equation numbers.
9. Put generated auxiliary files and PDFs under `build/`. Compile with the project's existing `./build.sh` workflow and inspect warnings, references and rendered pages.
10. Before completion, validate assignment coverage, source/report consistency, duplicate labels, undefined references and final PDF layout.

## Project convention

The detailed source instruction is preserved in
`references/technical_latex_report_skill_v4.md`. Read it when the task involves
nontrivial report structure, evidence, mathematics, listings or validation.

For cellular-automaton laboratory reports, keep the mathematical definition, neighborhood, boundary handling, local rule, measured quantities and periodicity reasoning explicit. Match notation and bit order to the implementation. Preserve separate results and analysis sections when the supplied example uses them.
