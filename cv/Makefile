LATEX= pdflatex --shell-escape

MAINDOC= main
OUTPDF=../downloads/CV_KrijnDoekemeijer_2025.pdf

all: clean
	${LATEX} ${MAINDOC}.tex
	mv ${MAINDOC}.pdf ${OUTPDF}

clean:
	rm -f *out *aux *bbl *blg *log *.tex~ *.dvi *.fdb_lat* *.fls
	rm -f ${OUTPDF}
