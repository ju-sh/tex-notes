build: pss1.tex pss3.tex pss4.tex
	xelatex --shell-escape pss1.tex
	xelatex --shell-escape pss3.tex
	xelatex --shell-escape pss4.tex

watch:
	latexmk -pvc -xelatex -shell-escape pss1.tex

clean:
	rm -f *.lo[a,f,l,t,g] *.bb[l,g] *.blg *.out *.pdf *.nlo *.toc \
		 *.aux *-blx.bib *.run.xml *.sw[op] *~ *.bib.bak *.bib.sav \
		 *.fls *.fdb_latexmk *.md5 *.dpth *.run.xml *.auxlock *.bcf \
		 *.acn *.acr *.alg *.glg *.glo *.gls *.ist \
		 *.snm *.nav *.xdv *_bibertool.bib *.dep *.*-SAVE-ERROR \
		 *.sbl *.ilg *.nlo *.nls *.nlg *.sym
	rm -rf _minted-*/
