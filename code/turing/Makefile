#
# Makefile -- build turing machine simulator
#
# For additional information, check the README file
#
# (c) 2010 Prof Dr Andreas Mueller, Hochschule Rapperswil
# $Id$
#
all:	turing

turing:	turing.c Makefile
	gcc -o turing -g -Wall -O -std=c99 turing.c

subtract:	turing
	time ./turing -v -o 5 -s 78 -t data/subtracttape pgm/subtract

beaver4:	turing 
	./turing -o 20 -s 70 pgm/beaver4

beaver3:	turing
	./turing -c -p 100000 -v -o 20 -s 70 pgm/beaver3

beaver5:	turing	
	time ./turing -o 15000 -s 30000 pgm/beaver5

add:	turing
	./turing -c -p 100000 -v -o 2 -s 40 -t data/addtape pgm/add

add1:	turing
	./turing -c -p 10000 -v -o 2 -s 50 -t data/addtape1 pgm/add

add2:	turing
	./turing -c -p 10000 -v -o 2 -s 50 -t data/addtape2 pgm/add

add3:	turing
	./turing -c -p 10000 -v -o 2 -s 50 -t data/addtape3 pgm/add

