MAIN_TEX = main.tex
OUTPUT_DIR = _build

build:
	makeglossaries main.; pdflatex -shell-escape $(MAIN_TEX)
	makeglossaries main.; pdflatex -shell-escape $(MAIN_TEX)
	makeglossaries main.; pdflatex -shell-escape $(MAIN_TEX)

clean:
	find . -type f -regex '.*\.\(log\|aux\|dvi\|toc\|out\|xdy\|glo\|glg\|gls\|ist\|lot\|lof\|acr\|acn\|acl\|alg\|ilg\|ind\|fls\|fdb_latexmk\|pytxcode\)' -print -delete
	rm -rf _minted-*

.PHONY: build clean
