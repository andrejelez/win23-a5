CC = gcc
CFLAGS = -Wall -g

SRC = $(wildcard *.c)
OBJ = $(SRC:.c=.o)
DEPS = $(wildcard *.h)

calculator: $(OBJ)
	$(CC) $(CFLAGS) -o $@ $^

%.o: %.c $(DEPS)
	$(CC) $(CFLAGS) -c -o $@ $<

.PHONY: clean

clean:
	rm -f $(OBJ) calculator
