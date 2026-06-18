# Post-Quantum Cryptography Notes

Lecture notes for the **Post-Quantum Cryptography** course of the Master's Degree in Cybersecurity at **Politecnico di Torino**.

These notes collect definitions, theorem statements, examples, and visual summaries used while studying quantum-resistant cryptographic constructions. The material is written in LaTeX and follows the Politecnico di Torino Cybersecurity template included in this repository.

## Contents

The document currently covers:

- an introduction to the quantum threat model and the limits of classical public-key cryptography;
- the main families of post-quantum assumptions, including code-based, lattice-based, multivariate, hash-based, and isogeny-based cryptography;
- NIST post-quantum cryptography standardization notes;
- mathematical background and dedicated sections on lattice problems such as SVP and CVP;
- custom theorem, definition, and proposition boxes for cleaner lecture notes.

The compiled PDF is available as [`main.pdf`](main.pdf), while the source is organized across [`main.tex`](main.tex) and the files in [`sections/`](sections/).

## Repository Structure

```text
.
├── main.tex                  # Main LaTeX entry point
├── main.pdf                  # Compiled notes
├── sections/                 # Individual lecture-note sections
├── images/                   # Figures used in the notes
├── slides/                   # Referenced course slide PDFs
└── latex-templates/styles/   # Politecnico di Torino LaTeX style
```

## Building the Notes

To compile the document, make sure you have a working LaTeX distribution installed, such as TeX Live or MiKTeX.

From the repository root, run:

```bash
latexmk -pdf main.tex
```

Alternatively, you can compile with `pdflatex`:

```bash
pdflatex main.tex
pdflatex main.tex
```

Running the command twice helps LaTeX resolve the table of contents and cross-references correctly.

## Custom LaTeX Environments

The notes define three custom `tcolorbox` environments:

- `defBox` for definitions and theoretical remarks;
- `thmBox` for theorems and formal results;
- `propBox` for propositions and observations.

Example:

```latex
\begin{defBox}{Definition title}
Text of the definition.
\end{defBox}

\begin{thmBox}{Theorem title}
Text of the theorem.
\end{thmBox}

\begin{propBox}{Proposition title}{label}
Text of the proposition.
\end{propBox}
```

For `propBox`, both brace arguments are required: the title and the internal label.

## Disclaimer

These notes are intended as a personal study aid and summary for the Post-Quantum Cryptography course. They do not replace lectures, exercises, or any official course material.

Although care has been taken to keep the content accurate, the notes may still contain typos, omissions, or personal interpretations.

## Author

**Stefano Pietro Sternativo**  
Master's Degree in Cybersecurity, Politecnico di Torino  
Academic year: **2025/2026**

