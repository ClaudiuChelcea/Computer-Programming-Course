# compiler setup
CC=gcc
CFLAGS=-Wall -Wextra

# targets
TARGETS=codeinvim

# make
build: $(TARGETS)

codeinvim: codeinvim.c
	$(CC) $(CFLAGS) -o codeinvim codeinvim.c 

clean:
	rm -f $(TARGETS)

.PHONY: clean
