# Makefile for LaTeX academic report

# Main document
MAIN = report

# Output directory
OUTDIR = .

# Compiler
LATEX = pdflatex
BIBTEX = bibtex

# Flags
LATEXFLAGS = -interaction=nonstopmode -halt-on-error

# Default target
all: $(MAIN).pdf

# Build PDF
$(MAIN).pdf: $(MAIN).tex references.bib
	$(LATEX) $(LATEXFLAGS) $(MAIN)
	$(BIBTEX) $(MAIN)
	$(LATEX) $(LATEXFLAGS) $(MAIN)
	$(LATEX) $(LATEXFLAGS) $(MAIN)

# Quick build (no bibliography)
quick:
	$(LATEX) $(LATEXFLAGS) $(MAIN)

# Clean auxiliary files
clean:
	rm -f $(MAIN).aux $(MAIN).log $(MAIN).out $(MAIN).toc
	rm -f $(MAIN).bbl $(MAIN).blg
	rm -f *.aux *.log *.out *.toc *.bbl *.blg

# Clean everything including PDF
distclean: clean
	rm -f $(MAIN).pdf

# View PDF (macOS)
view: $(MAIN).pdf
	open $(MAIN).pdf

# View PDF (Linux)
view-linux: $(MAIN).pdf
	xdg-open $(MAIN).pdf

# Word count (approximate)
wordcount:
	@echo "Approximate word count:"
	@detex $(MAIN).tex | wc -w

# Check for undefined references
check:
	@grep -i "undefined" $(MAIN).log || echo "No undefined references"
	@grep -i "warning" $(MAIN).log || echo "No warnings"

# Help
help:
	@echo "Available targets:"
	@echo "  all        - Build PDF with bibliography (default)"
	@echo "  quick      - Quick build without bibliography"
	@echo "  clean      - Remove auxiliary files"
	@echo "  distclean  - Remove all generated files including PDF"
	@echo "  view       - Open PDF (macOS)"
	@echo "  view-linux - Open PDF (Linux)"
	@echo "  wordcount  - Approximate word count"
	@echo "  check      - Check for warnings and errors"
	@echo "  help       - Show this help message"

.PHONY: all quick clean distclean view view-linux wordcount check help
