DIR_INC = ./include
DIR_BIN = ./bin
DIR_OBJ = ./obj
DIR_SRC = ./src

SRC = ${wildcard ${DIR_SRC}/*.cpp}
OBJ = $(patsubst %cpp, $(DIR_OBJ)/%o, $(notdir $(SRC)))

TARGET = main

BIN_TARGET = $(DIR_BIN)/$(TARGET)

CC = g++
CPPFLAGS = -g -Wall -I$(DIR_INC)

$(BIN_TARGET):$(OBJ)
	$(CC) $(OBJ) -o $@

${DIR_OBJ}/%.o:${DIR_SRC}/%.cpp
	${CC} ${CPPFLAGS} -c $< -o $@

.PHONY:clean
clean:
	find ${DIR_OBJ} -name '*.o' -exec rm -rf {} \;



