# Capstone Report

## Table of Contents
- [Overview](#overview)
- [Files and Structure](#files-and-structure)
- [How to Access the Report](#how-to-access-the-report)
- [LaTeX Document Class: `extreport`](#latex-document-class-extreport)
- [Sectioning Hierarchy](#sectioning-hierarchy)

---

## Overview

This repository contains our capstone report written in LaTeX. The report is divided into several sections, each available as individual PDF files. Additionally, there is a main PDF that combines all sections together.

---

## Files and Structure

The repository is organized as follows:

### Main Files
- **main.pdf**: This is the complete report rendered together.
- **intro.pdf**: Contains the Abstract, Introduction, and Acknowledgements sections.
- **outro.pdf**: Includes the Cost section.

### Sublatex Folder
Each individual section of the report is stored in the `sublatex` folder. The structure within this folder is as follows:
- Each section has its own subfolder named after the author or section name.
- Within each subfolder, you will find a PDF file named after the author or section.

For example:

/sublatex/author_name/author_name.pdf


---

## How to Access the Report

1. **Main Report**: To read the entire report, download and open the `main.pdf` file.
2. **Individual Sections**:
   - For the introduction and acknowledgements, open the `intro.pdf` file.
   - For the cost section, open the `outro.pdf` file.
   - For other individual sections, navigate to the `sublatex` folder, find the appropriate subfolder, and open the corresponding PDF file.

---

## Contact Information

- GitHub Issues: You can also open an issue in this repository.

---

## LaTeX Document Class: `extreport`

This project uses the `extreport` document class, which is an extended version of the standard `report` class provided by the `extsizes` package. The `extreport` class allows for additional font size options (e.g., 8pt, 9pt, 10pt, 11pt, 12pt, 14pt, 17pt, and 20pt) that are not available in the standard LaTeX classes.

---

## Sectioning Hierarchy

The `extreport` class follows the same sectioning hierarchy as the `report` class, but with the added flexibility of larger font sizes. Below is the hierarchy of sectioning commands and their corresponding levels in Microsoft Word:

| LaTeX Command       | Word Equivalent   | Description                          |
|---------------------|-------------------|--------------------------------------|
| `\part`             | **No direct equivalent** | A high-level division, often used for major sections like "Part I". |
| `\chapter`          | **Heading 1**     | A major division of the document, typically used for chapters. |
| `\section`          | **Heading 2**     | A primary subdivision within a chapter or part. |
| `\subsection`       | **Heading 3**     | A secondary subdivision within a section. |
| `\subsubsection`    | **Heading 4**     | A tertiary subdivision within a subsection. |
| `\paragraph`        | **Heading 5**     | A smaller subdivision, often used for paragraphs with titles. |
| `\subparagraph`     | **Heading 6**     | An even finer subdivision, rarely used but available. |

### Example Usage

Here’s an example of how the sectioning commands are used in the `extreport` class:

```latex
\documentclass[14pt]{extreport}

\begin{document}

\part{Introduction to LaTeX}
\chapter{Getting Started with extreport}  % Heading 1 in Word
\section{Installation}                    % Heading 2 in Word
\subsection{Windows Installation}         % Heading 3 in Word
\subsubsection{Using MiKTeX}              % Heading 4 in Word
This is a subsubsection discussing MiKTeX installation.
\paragraph{Downloading MiKTeX}            % Heading 5 in Word
Download the installer from the official website.
\subparagraph{Running the Installer}      % Heading 6 in Word
Follow the on-screen instructions.

\end{document}
