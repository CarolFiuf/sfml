CXX = g++

PROJECT=demo
CFLAGS=
SRC=src
BUILD:=build

OBJFILES=Object.o

MAIN:=main.cpp
TARGET:=${BUILD}/${PROJECT}
SFML_PATH:=/opt/homebrew/Cellar/sfml/2.5.1_2
SFML_LINK:=-lsfml-graphics -lsfml-window -lsfml-system
INCLUDE=-I${SFML_PATH}/include
LIBINCLUDES=-L${SFML_PATH}/lib

LDFLAGS=${SFML_LINK}

all:
	${CXX} ${CFLAGS} ${INCLUDE} ${LIBINCLUDES} -o ${TARGET} ${SRC}/${MAIN} ${SFML_LINK} 

clean:
	rm -rf build/*

run:
	${TARGET}