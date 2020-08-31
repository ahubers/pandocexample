PY=python
PANDOC=pandoc

BASEDIR=$(CURDIR)
INPUTDIR=$(BASEDIR)
OUTPUTDIR=$(BASEDIR)/../output
STYLEDIR=$(INPUTDIR)/../style

pdf:
	pandoc -s \
	"$(INPUTDIR)"/example.md \
	-o "$(OUTPUTDIR)/example.pdf" \
	--template="$(STYLEDIR)/example.tex" \
	--latex-engine=xelatex

tex:
	pandoc -s \
	"$(INPUTDIR)"/*.md \
	-o "$(OUTPUTDIR)/example.tex" \
	--template="$(STYLEDIR)/example.tex" \
	--latex-engine=xelatex

docx:
	pandoc "$(INPUTDIR)"/*.md \
	-o "$(OUTPUTDIR)/example.docx" \

html:
	pandoc "$(INPUTDIR)"/*.md \
	-o "$(OUTPUTDIR)/example.html"

.PHONY: help pdf docx html tex
