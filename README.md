# latex-template

My personal LaTeX template for formal presentations and
thesis/reports.

It contains a `report.tex` which is the main report file and a
`presentation.tex` which is the template for presentations.

## Report structure

The `report.tex` file, used to write thesis, books or similar stuff is
structured in the following manner:

1. `\documentclass` uses the book class. It could use other classes,
   such as the [Koma-Script Book](https://ctan.org/pkg/scrbook),
   [ElegantBook](https://ctan.org/pkg/elegantbook),
   [kaobook](https://github.com/fmarotta/kaobook) or
   [Tufte-LaTeX](https://github.com/Tufte-LaTeX/tufte-latex).
2. It then includes a large selection of packages that are generally
   needed for technical subjects and formatting. These packages, with
   their descriptions are found in `loaded-thesis.sty`.
3. It has a few explicit packages, such as the bibliography, to help
   the user customise them if needed.
4. It then declares a few helper functions and environmnets.
5. Finally, it includes the `acronyms.tex` and `glossaries.tex` files,
   which should have the definitions for acronyms and glossaries of
   your work.
6. Then the document starts. The cover page is separated into the
   `cover.tex` file and is included.
7. Finally, some more text is added and the table of contents are
   presented. The body of the work: chapters, bibliography and
   appendixes; are all included from external files to keep the
   `report.tex` file clean.
