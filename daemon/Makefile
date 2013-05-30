###########################################################
# Makefile
# History:
#     2013-05-30  Dennis  Create
###########################################################

CC     = gcc
FLAGS += -Wall -I../
LIBS   =

TARGET = daemonize
OBJ_SRC= daemonize.c
OBJ_INC=
OBJS  := $(OBJ_SRC:.c=.o)
OBJS_SRC_OTHER = ../error.c
OBJS_OTHER = error.o

all: $(TARGET)

$(TARGET): $(OBJS) $(OBJS_OTHER)
	$(CC) $(FLAGS) -o $@ $^ $(LIBS)
	
#$(OBJS): $(OBJ_SRC)
$(OBJS): %.o: %.c
	$(CC) $(FLAGS) -c $^

$(OBJS_OTHER):$(OBJS_SRC_OTHER)
	$(CC) $(FLAGS) -c $^

.PHONY: clean
clean:
	rm -f *.o $(TARGET)

