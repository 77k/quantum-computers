PDFLATEX        =       pdflatex
PANDOC          =       pandoc

all: modular_trap_proposal.pdf modular_map_proposal.doc

modular_trap_proposal.doc:	modular_trap_proposal.tex stat.eps
	${PANDOC} -o $@ $^
modular_trap_proposal.pdf:	modular_trap_proposal.tex
	${PDFLATEX} $^
	
stat.eps:	stat.csv
	./gen-stats.r


