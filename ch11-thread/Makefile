################################################################################
# Makefile
# History:
#        2013/07/25 Dennis Create
################################################################################
include ../Make.defines

PROGS = thread-11-8 thread-11-9

all: ${PROGS}

thread-11-8: thread-11-8.c
	${CC} -c $^ 

thread-11-9: thread-11-9.c
	${CC} -c $^ 

.PHONY: clean
clean:
	rm -f ${PROGS} ${CLEANFILES}

