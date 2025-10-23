CC = gcc
CFLAGS = -Wall -Werror -Iinclude
all: mu_app
mu_app: src/main.o src/mu_lib.o
	$(CC) src/main.o src/ mu_lib.o -o mu_app
src/main.o: src/main.c
	$(CC) (CFLAGS) -c src/main.c -o src/main.o
src/mu_lib.o: src/mu_lib.c include/mu_lib.h
	$(CC) (CFLAGS) -c src/mu_lib.c -o src/mu_lib.o
clean:
	rm -f src/main.o src/mu_lib.o mu_app