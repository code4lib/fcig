#
# generate report in various formats
#
# required packages on Ubuntu Xenial: pandoc, texlive-latex-base, texlive-fonts-recommended
# need at pandoc 1.16 for the wide table to not overflow the page
#
SRCDOC=../Report_of_the_Code4Lib_Fiscal_Continuity_Interest_Group.md

all: fcig_report.pdf fcig_report.mediawiki.txt

fcig_report.pdf: $(SRCDOC)
	pandoc -V papersize=landscape -V geometry:margin=1in -t latex -o fcig_report.pdf $(SRCDOC)
fcig_report.mediawiki.txt: $(SRCDOC)
	pandoc -t mediawiki -o fcig_report.mediawiki.txt $(SRCDOC)
