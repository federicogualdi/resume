.PHONY: install export clean

FILENAME ?= Federico Gualdi - Resume

install:
	sudo apt install texlive-xetex texlive-latex-extra texlive-fonts-extra

export:
	mkdir -p build
	xelatex -interaction=nonstopmode -halt-on-error \
		-jobname="$(FILENAME)" \
		-output-directory=build \
		resume.tex
	mv -f "build/$(FILENAME).pdf" ../

clean:
	rm -rf build