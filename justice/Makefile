SOURCES := ${wildcard *.tex}
TARGETS := $(SOURCES:%.tex=%)

all: $(TARGETS)

%: %.tex
	lualatex --jobname=$@-$(notdir $(CURDIR)) $<

clean:
	rm -rf *.aux
	rm -rf *.log
