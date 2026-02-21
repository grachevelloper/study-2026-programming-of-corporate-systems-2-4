CXX = g++
CXXFLAGS = -Wall -std=c++11

all: hello_program

hello_program: main.o hello.o
	$(CXX) $(CXXFLAGS) -o hello_program main.o hello.o

main.o: main.cpp hello.h
	$(CXX) $(CXXFLAGS) -c main.cpp

hello.o: hello.cpp hello.h
	$(CXX) $(CXXFLAGS) -c hello.cpp

clean:
	rm -f *.o hello_program

run: hello_program
	./hello_program
