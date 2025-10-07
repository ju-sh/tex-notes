build: index.tex bib.bib
	xelatex --shell-escape index.tex
	xelatex --shell-escape index.tex
	#makeglossaries classicthesis
	#makeindex classicthesis.nlo -s nomencl.ist -o classicthesis.nls
	biber classicthesis
	xelatex --shell-escape index.tex
	xelatex --shell-escape index.tex

watch:
	latexmk -pvc -xelatex -shell-escape index.tex

clean:
	rm -f *.lo[a,f,l,t,g] *.bb[l,g] *.blg *.out *.pdf *.nlo *.toc \
		 *.aux *-blx.bib *.run.xml *.sw[op] *~ *.bib.bak *.bib.sav \
		 *.fls *.fdb_latexmk *.md5 *.dpth *.run.xml *.auxlock *.bcf \
		 *.acn *.acr *.alg *.glg *.glo *.gls *.ist \
		 *.snm *.nav *.xdv *_bibertool.bib *.dep *.*-SAVE-ERROR \
		 *.sbl *.ilg *.nlo *.nls *.nlg *.sym
	rm -rf _minted-*/
