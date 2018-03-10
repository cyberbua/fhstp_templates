TEX_MAIN_FILE=root

all: compile

compile:
	rubber -d -m xelatex $(TEX_MAIN_FILE)

clean:
	rubber --clean $(TEX_MAIN_FILE)
	rm $(TEX_MAIN_FILE).pdf

spellcheck:
	find . -name "*.tex" -exec aspell --lang=en_GB --mode=tex check "{}" \;
