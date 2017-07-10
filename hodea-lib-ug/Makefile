
MAINDOC = hodea-lib-ug.tex
TEXFILES = $(wildcard *.tex)

PDF = $(MAINDOC:.tex=.pdf)

DOC_DIR = ../doc


all: $(PDF)

$(PDF): $(TEXFILES)
	pdflatex -halt-on-error $(MAINDOC)
	pdflatex -halt-on-error $(MAINDOC)

.PHONY: clean release

clean:
	rm -f *.aux *.log *.toc *.hst *.ver
	rm -f $(PDF)

release: $(PDF)
	cp $(PDF) $(DOC_DIR)/$(PDF)
