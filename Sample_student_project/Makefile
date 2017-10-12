CC = g++
OBS = main.o game.o othello.o
MAIN = main.cc game.h othello.h
OTHELLO = othello.cc othello.h game.h piece.h colors.h

all: main

main: $(OBS)
	$(CC) $(OBS) -o output

main.o: $(MAIN)
	$(CC) $(MAIN) -c

game.o: game.cc game.h
	$(CC) game.cc -c

othello.o: $(OTHELLO)
	$(CC) $(OTHELLO) -c

arhcive:
	tar archive.tar.gz -cvf colors.h game.cc game.h main.cc Makefile othello.cc othello.h piece.h

# removing all object files
clean: 
	rm *.o output
