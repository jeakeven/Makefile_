CC = g++
CPPFLAGS = -g -Wall

main:main.o HelloWorld.o
	$(CC) main.o HelloWorld.o -o main

main.o:Main.cpp
	${CC} ${CPPFLAGS} -c Main.cpp -o main.o

HelloWorld.o:HelloWorld.cpp
	${CC} ${CPPFLAGS} -c HelloWorld.cpp -o HelloWorld.o

clean:
	rm -rf *.o

