
MAINDOC = hodea-lib-ug.tex
TEXFILES = $(wildcard *.tex)

PDF = $(MAINDOC:.tex=.pdf)


all: $(PDF)

$(PDF): $(TEXFILES)
	pdflatex -halt-on-error $(MAINDOC)
	pdflatex -halt-on-error $(MAINDOC)

.PHONY: clean

clean:
	rm -f *.aux *.log *.toc
	rm -f $(PDF)

