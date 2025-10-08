# ICMC-TEMPLATE
ICMC-TEMPLATE  © 2025 by William Aisawa is licensed under Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International. To view a copy of this license, visit https://creativecommons.org/licenses/by-nc-sa/4.0/

# ICMC-TEMPLATE

Template LaTeX para trabalhos (relatórios, artigos ou documentos) desenvolvido para o ICMC.

Este repositório contém um template simples e organizado para texto em LaTeX, com estrutura de seções, configuração de linguagem e arquivos auxiliares (imagens e bibliografia).

## Estrutura do repositório

- `main.tex` — arquivo principal do projeto (ponteira para compilar o documento).
- `bibliography.bib` — arquivo BibTeX com referências bibliográficas.
- `config/` — arquivos de configuração (por exemplo `code_lang.tex` para configurações de listagem de código).
- `images/` — imagens usadas no template (ex.: `icmc_logo.png`, `lab_logo.jpeg`).
- `sections/` — arquivos de seção (`section00.tex`, `section01.tex`, ...). Use aqui o conteúdo das seções para manter o `main.tex` limpo.
- `LICENSE` — licença do repositório.
- `README.md` — este arquivo.

## Como usar

1. Faça uma cópia deste diretório para começar seu trabalho.
2. Edite `main.tex` definindo título, autor e demais metadados.
3. Adicione ou edite arquivos em `sections/` para estruturar o conteúdo.
4. Insira figuras na pasta `images/` e cite-as no texto com `\includegraphics` e `\ref`/`\label` conforme necessário.
5. Gerencie referências em `bibliography.bib` e cite no texto com `\cite{chave}`.

## Compilação (exemplo básico)

Recomenda-se usar uma distribuição TeX atualizada (TeX Live, MiKTeX, etc.). Um fluxo de compilação comum:

1. pdflatex main.tex
2. bibtex main
3. pdflatex main.tex
4. pdflatex main.tex

Você também pode usar ferramentas como `latexmk` para automatizar esse fluxo:

latexmk -pdf main.tex

Se preferir um ambiente gráfico, editores como TeXstudio, Overleaf ou VS Code com a extensão LaTeX Workshop funcionam bem.

## Personalização

- Para adicionar pacotes ou customizar pacotes existentes, edite `main.tex` (ou crie um arquivo em `config/` e o inclua).
- Para adicionar suporte de listagem de código, verifique `config/code_lang.tex`.

## Exemplos rápidos

- Inserir uma figura:

```tex
\begin{figure}[ht]
	\centering
	\includegraphics[width=0.5\textwidth]{images/icmc_logo.png}
	\caption{Logo do ICMC}
	\label{fig:logo}
\end{figure}
```

- Citar uma referência:

```tex
Como mostrado em \cite{autor2020}, ...
```

## Licença

Este template está disponibilizado sob a licença presente no arquivo `LICENSE`.

## Contato / Contribuição

Contribuições são bem-vindas. Abra issues ou pull requests com melhorias, correções ou atualizações de pacotes. Para dúvidas, contacte o mantenedor do repositório.

---

Se quiser, posso também:

- Gerar um exemplo de `main.tex` mais completo.
- Adicionar instruções específicas para compilar no Windows (MiKTeX) ou Linux (TeX Live).
- Incluir um workflow do GitHub Actions para compilar automaticamente PDFs.

Diga qual(is) desses extras prefere que eu adicione.

## English version

If you prefer an English copy, here is the same information in English.

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
- `README.md` — this file (Portuguese + English).
- `README_en.md` — separate English README (optional).

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
