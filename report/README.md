# Academic Report: LaTeX Version

This folder contains the academic paper version of the Wikipedia vs Grokipedia quality comparison analysis.

## Files

- **report.tex** - Main LaTeX document
- **references.bib** - BibTeX bibliography file
- **README.md** - This file

## Compilation Instructions

### Using pdflatex (Recommended)

```bash
cd academic-report
pdflatex report.tex
bibtex report
pdflatex report.tex
pdflatex report.tex
```

The double compilation after bibtex ensures all references and citations are properly resolved.

### Using latexmk (Automated)

```bash
cd academic-report
latexmk -pdf report.tex
```

This automatically handles all compilation steps.

### Online Compilation (Overleaf)

1. Upload all files to a new Overleaf project
2. Set compiler to pdfLaTeX
3. Click "Recompile"

## Document Structure

The academic report includes:

1. **Title Page** - Author, affiliation, date
2. **Abstract** - 200-word summary with keywords
3. **Table of Contents** - Auto-generated
4. **Introduction** - Research context and questions
5. **Related Work** - Literature review
6. **Methodology** - Topic selection, dimensions, protocol
7. **Results** - Overall and dimension-by-dimension analysis
8. **Discussion** - Interpretation and implications
9. **Limitations and Future Work** - Methodological constraints
10. **Conclusion** - Key findings and strategic insights
11. **References** - Academic citations

## Key Features

### Tables
- Table 1: Overall quality scores by topic
- Table 2: Quality dimension comparison
- Table 3: Citation density analysis

### Professional Formatting
- APA-style citations using natbib
- Structured sections with clear hierarchy
- Academic writing style throughout
- Proper mathematical notation where applicable

### Academic Rigor
- Research questions explicitly stated
- Methodology described in detail
- Limitations acknowledged
- Future work directions proposed
- Proper literature citations

## Output

The compilation produces `report.pdf` - a publication-ready academic paper suitable for:
- Conference submissions
- Journal articles
- Technical reports
- Academic presentations
- Institutional repositories

## Requirements

### LaTeX Distribution
- **TeX Live** (Linux/macOS/Windows)
- **MiKTeX** (Windows)
- **MacTeX** (macOS)

### Required Packages
All standard packages included in modern LaTeX distributions:
- inputenc, fontenc (character encoding)
- graphicx (images)
- booktabs (professional tables)
- hyperref (clickable links)
- natbib (citations)
- geometry (page layout)

## Customization

### Modify Author Information
Edit lines 23-28 in report.tex:
```latex
\author{
    Your Name\\
    \textit{Your Institution}\\
    \texttt{your@email.com}
}
```

### Adjust Page Layout
Edit geometry settings (lines 17-23):
```latex
\geometry{
    a4paper,
    left=2.5cm,
    right=2.5cm,
    ...
}
```

### Add Your Own Citations
Edit references.bib and cite in text:
```latex
\citep{authorYEAR}  % (Author, YEAR)
\citet{authorYEAR}  % Author (YEAR)
```

## Word Count

Approximate sections:
- Abstract: 200 words
- Introduction: 600 words
- Related Work: 500 words
- Methodology: 800 words
- Results: 1,200 words
- Discussion: 1,000 words
- Conclusion: 400 words
- **Total: ~4,700 words**

## Conversion to Other Formats

### Convert to Word
```bash
pandoc report.tex -o report.docx --bibliography=references.bib
```

### Convert to HTML
```bash
pandoc report.tex -o report.html --bibliography=references.bib --mathjax
```

## Citation

If citing this work in academic contexts:

```bibtex
@techreport{orban2025wikipedia,
  title={A Comparative Quality Assessment of AI-Generated and Community-Edited
         Encyclopedic Content: Wikipedia versus Grokipedia},
  author={Orban, David},
  year={2025},
  institution={Independent Research},
  url={https://github.com/davidorban/pedia}
}
```

## License

This academic report is part of the Wikipedia vs Grokipedia comparison project.

**License:** Creative Commons Attribution 4.0 International (CC BY 4.0)

## Contact

**David Orban**
- Website: https://davidorban.com
- GitHub: https://github.com/davidorban/pedia

---

**Last Updated:** 2025-11-01
**Version:** 1.0
**Format:** LaTeX (pdfLaTeX)
