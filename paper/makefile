MAIN=paper
BIB=$(MAIN)
LATEX=latexmk -pdf

$(MAIN).pdf: $(MAIN).tex $(BIB).bib
	$(LATEX) $(MAIN)

open: $(MAIN).pdf
	open $(MAIN).pdf

clean:
	$(LATEX) -C

live:
	$(LATEX) -pvc $(MAIN) &>/dev/null
