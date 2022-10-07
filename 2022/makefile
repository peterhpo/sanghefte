clean:
	rm *.sxd
	rm *.aux
	rm *.dep
	rm *.ly
	rm *.out
	rm *.sxc
	rm *.log
	rm -r 4c
	rm -r eb
	rm -r tmp*.pdf


# For å kjøre scriptet som lager pdf-en 
# (må ha installert lilypond og latex for å kjøre)
song:
	lilypond-book --pdf sanghefte.latex
	pdflatex sanghefte.tex

