# Makefile
CXX=g++
CPPFLAGS=--std=c++17

mariokart: kart.o bike.o monsterTruck.o mariokart.o
	${CXX} ${CPPFLAGS} -o mariokart $^ 

%.o : %.cpp %.h
	${CXX} ${CPPFLAGS} -c $<

# $^ gives all prerequisites
# omitting target for each *.o file, as they will be generated from the implicit rule
# check the Tip box in lab00.pdf (pg. 14)

clean:
	rm -f *.o mariokart
