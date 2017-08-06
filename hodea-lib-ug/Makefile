
MAINDOC = hodea-lib-ug.tex
TEXFILES = $(wildcard *.tex)

PDF = $(MAINDOC:.tex=.pdf)

ROOT_DIR = ../


all: $(PDF)

$(PDF): $(TEXFILES)
	pdflatex -halt-on-error $(MAINDOC)
	pdflatex -halt-on-error $(MAINDOC)

.PHONY: clean release

clean:
	rm -f *.aux *.log *.toc *.hst *.ver *.out
	rm -f $(PDF)

release: $(PDF)
	cp $(PDF) $(ROOT_DIR)/hodea-lib/doc/$(PDF)
