# Makefile for ClonalFrameML
CC = $(CXX)
CXXFLAGS += -O3 -fopenmp
LDFLAGS += -fopenmp
OBJECTS = main.o
HEADERS = main.h brent.h powell.h

.PHONY: clean 

all: ClonalFrameML

ClonalFrameML: $(OBJECTS)
	$(CC) $(LDFLAGS) -o ClonalFrameML $(OBJECTS)

main.o: main.cpp $(HEADERS)
	$(CC) $(CXXFLAGS) -c -o main.o main.cpp

clean:
	rm -f $(OBJECTS)
