SOURCE_TEX=morrowind.tex
PRETTY_TEX=_final.tex

LATEX=pdflatex
LFLAGS=

XELATEX=xelatex
XFLAGS=

default: $(SOURCE_TEX) pdflatex cleanaux

pdflatex:
	$(LATEX) $(LFLAGS) $(SOURCE_TEX)

xelatex:
	$(XELATEX) $(XFLAGS) $(SOURCE_TEX)

fancy: $(SOURCE_TEX) xelatex cleanaux

# TODO Remove, for purposes of experiment only
testpdf:
	$(LATEX) $(LFLAGS) foo.tex

# TODO Remove, for purposes of experiment only
testfancy:
	$(XELATEX) $(XFLAGS) foo.tex

clean: cleanaux
	rm -rf *.log *.pdf *.toc

cleanaux:
	rm -rf *.aux
