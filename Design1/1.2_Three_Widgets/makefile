CC       = gcc
CFLAGS   =  
LDFLAGS  =  `pkg-config gtk+-2.0 --cflags --libs`

SRCS = ShowNum.c Sum.c TimeShow.c main.c
TARGETS = $(patsubst %.c, %, $(SRCS))

all:$(TARGETS)

$(TARGETS):$(SRCS)
	$(CC) $@.c -o $@.o $(LDFLAGS) $(CFLAGS)

clean:
	-rm -rf $(TARGETS) 

.PHONY: clean all