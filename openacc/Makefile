#
# Makefile to build example OpenACC programs 
#

CC=pgcc
CFLAGS=-acc -fast -Minfo

EXE1=saxpy.exe
EXES=$(EXE1)

all: $(EXES)

$(EXES): %.exe : %.c
	$(CC) $(CFLAGS) -o $@ $^

.PHONY: clean all

clean:
	\rm -f $(EXES) 
	\rm -f *.o



# Makefile
SHELL:=/bin/bash

CC=pgcc
CFLAGS=-acc -fast -Minfo

MODULE_1 =module add pgi/64/13.5
MODULE_2 =module load languages/python-2.7.6

EXE1=saxpy.exe
EXES=$(EXE1)



all: $(EXES)

$(EXES): 
	$(MODULE_1) && \
	$(CC) $(CFLAGS) -o $@ $^

.PHONY: clean all

clean:
	\rm -f $(EXES)
	\rm -f *.o
