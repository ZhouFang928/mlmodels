########################################################################
#
# Makefile for rain-tomorrow pre-built ML model
#
########################################################################

# List the files to be included in the .mlm package.

MODEL_FILES = 			\
	rain-tomorrow.RData	\
	configure.sh		\
	train.R			\
	demo.R 			\
	print.R			\
	display.R		\
	score.R			\
	rattle.R		\
	weatherAUS.RData	\
	README.txt		\
	DESCRIPTION.yaml

# Include standard Makefile templates.

include ../mlhub.mk
include ../git.mk
include ../pandoc.mk

$(MODEL).RData: train.R
	Rscript $<

clean::
	rm -rf README.txt output

realclean:: clean
	rm -rf rain-tomorrow_*.mlm
