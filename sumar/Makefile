.PHONY: clean

CC=gcc
CFLAGS=-g -Wall

programa: principal.o sumar.o
	$(CC) $(CFLAGS) principal.o sumar.o -o programa

principal.o: principal.c suma.h
	$(CC) $(CFLAGS) -c principal.c -o principal.o

sumar.o: sumar.c suma.h
	$(CC) $(CFLAGS) -c sumar.c -o sumar.o

clean:
	rm -rf *.o programa

