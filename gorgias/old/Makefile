
SOURCES := $(wildcard *.tex)
TARGETS := $(SOURCES:%.tex=%)

all: $(TARGETS)

%: %.tex
	@lualatex --jobname=$@ $<

clean:
	@rm -fv *.aux *.log *.out

distclean: clean
	@rm -fv *.pdf
