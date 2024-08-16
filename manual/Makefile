ASCIIDOCTOR_FLAGS = -a pdf-page-size=A5
# all: freedoom-manual.pdf freedoom-manual-es.pdf
all: libtech1-manual.pdf

libtech1-manual.pdf: manual.adoc
	-asciidoctor-pdf $(ASCIIDOCTOR_FLAGS) manual.adoc -o $@

#freedoom-manual-es.pdf: manual-es.adoc
#	-asciidoctor-pdf $(ASCIIDOCTOR_FLAGS) manual-es.adoc -o $@

clean:
#	$(RM) freedoom-manual.pdf freedoom-manual-es.pdf
	$(RM) libtech1-manual.pdf
