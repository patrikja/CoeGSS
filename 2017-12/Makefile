NAME = Jansson_GSS_Applications

default: ${NAME}.pdf

clean:
	latexmk -C ${NAME}

${NAME}.pdf: ${NAME}.md template.tex
	pandoc -t beamer -H template.tex ${NAME}.md -o ${NAME}.pdf

${NAME}.tex: ${NAME}.md template.tex
	pandoc -t beamer -H template.tex ${NAME}.md -o ${NAME}.tex

${NAME}.html: ${NAME}.md
	pandoc --self-contained -S --latexmathml -t slidy ${NAME}.md -o ${NAME}.html

# Dependencies:
# * http://pandoc.org/ - a universal document converter
# * http://pandoc.org/demo/example9/producing-slide-shows-with-pandoc.html
