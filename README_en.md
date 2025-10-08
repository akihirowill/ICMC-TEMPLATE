## ICMC-TEMPLATE

LaTeX template for academic documents (reports, articles, or other documents) developed for ICMC.

This repository contains a simple and well-structured LaTeX template with section organization, language configuration, and supporting files (images and bibliography).

## Repository structure

- `main.tex` — main project file (entry point for compiling the document).
- `bibliography.bib` — BibTeX file with bibliographic references.
- `config/` — configuration files (for example `code_lang.tex` for code listing settings).
- `images/` — images used in the template (e.g., `icmc_logo.png`, `lab_logo.jpeg`).
- `sections/` — section files (`section00.tex`, `section01.tex`, ...). Keep section content here to keep `main.tex` clean.
- `LICENSE` — repository license.
- `README.md` — Portuguese README.
- `README_en.md` — this English README.

## How to use

1. Copy this directory to start your work.
2. Edit `main.tex` to set the title, author and other metadata.
3. Add or edit files in `sections/` to structure your content.
4. Place figures into the `images/` folder and include them in the text with `\includegraphics` and `\ref`/`\label` as needed.
5. Manage references in `bibliography.bib` and cite in the text with `\cite{key}`.

## Compilation (basic example)

It is recommended to use an up-to-date TeX distribution (TeX Live, MiKTeX, etc.). A common compilation flow is:

1. pdflatex main.tex
2. bibtex main
3. pdflatex main.tex
4. pdflatex main.tex

You can also use tools like `latexmk` to automate this flow:

latexmk -pdf main.tex

If you prefer a graphical environment, editors such as TeXstudio, Overleaf or VS Code with LaTeX Workshop work well.

## Customization

- To add packages or customize existing packages, edit `main.tex` (or create a file in `config/` and include it).
- For code listing support, check `config/code_lang.tex`.

## Quick examples

- Insert a figure:

```tex
\begin{figure}[ht]
  \centering
  \includegraphics[width=0.5\textwidth]{images/icmc_logo.png}
  \caption{ICMC logo}
  \label{fig:logo}
\end{figure}
```

- Cite a reference:

```tex
As shown in \cite{author2020}, ...
```

## License

This template is provided under the license included in the `LICENSE` file.

## Contact / Contribution

Contributions are welcome. Open issues or pull requests with improvements, fixes or package updates. For questions, contact the repository maintainer.

---

If you want, I can also:

- Create a more complete example `main.tex`.
- Add specific compilation instructions for Windows (MiKTeX) or Linux (TeX Live).
- Add a GitHub Actions workflow to automatically build the PDF.

Tell me which of these extras you'd like me to add.
