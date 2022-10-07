# Nytt sanghefte med noter :)

Her har vi prøvd å få inn noter i sangheftet da en gjennomsnittlig IFI-student ikke er kjent med de tradisjonelle studentsangene som synges ved gallaer eller andre arrangementer.

## Kjøring

For å få kjørt scriptet som lager PDFen må man ha installert [lilypond](https://lilypond.org/doc/v2.21/Documentation/contributor/requirements-for-compiling-lilypond#ubuntu) og LaTex e.l.
Ved installasjon på Ubuntu kjør:

```bash
sudo apt install texlive-latex-extra
sudo apt-get install -y lilypond
```

For selve kjøringen gjør kallet ```make song``` at pdf-en produseres. Dette kaller videre på kommandoene:

```
lilypond-book --pdf sanghefte.lytex
pdflatex sanghefte.tex
```

### Problemer som kan oppstå ved kjøring
Kjøringen lager en god del midlertidige filer hvorav noen av disse gjør at det ikke er mulig å kjøre igjen uten at disse slettes. Disse kan (mest sannsynlig) fjernes ved å kjøre ```make clean```, men mulig det er noen endringer i filnavn og/eller mappenavn som da gjør at ```make clean``` ikke sletter det som trengs å slettes. 
