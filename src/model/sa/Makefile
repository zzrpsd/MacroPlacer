CC = g++
PATH_TO_SRC = ./../../
INC = -I ${PATH_TO_SRC}

HEADERS_COUNTOFMOVABLEMACROSOUTSIDEDESIREDREGION = \
	${PATH_TO_SRC}sa/CostFunction.h\
	${PATH_TO_SRC}model/sa/CountOfMovableMacrosOutsideDesiredRegion.h\
	${PATH_TO_SRC}model/Floorplan.h\
	${PATH_TO_SRC}model/sa/FloorplanState.h

HEADERS_FLOORPLANSTATE = \
	${PATH_TO_SRC}sa/State.h\
	${PATH_TO_SRC}model/sa/FloorplanState.h\
	${PATH_TO_SRC}model/Floorplan.h\
	${PATH_TO_SRC}tree/icptree/ICPTree.h

HEADERS_MACROSDISPLACEMENT = \
	${PATH_TO_SRC}sa/CostFunction.h\
	${PATH_TO_SRC}model/sa/MacrosDisplacement.h\
	${PATH_TO_SRC}model/Floorplan.h\
	${PATH_TO_SRC}model/sa/FloorplanState.h

all:
	make CountOfMovableMacrosOutsideDesiredRegion.o
	make FloorplanState.o
	make MacrosDisplacement.o
CountOfMovableMacrosOutsideDesiredRegion.o: CountOfMovableMacrosOutsideDesiredRegion.cpp ${HEADERS_COUNTOFMOVABLEMACROSOUTSIDEDESIREDREGION}
	${CC} -c CountOfMovableMacrosOutsideDesiredRegion.cpp ${INC}
FloorplanState.o: FloorplanState.cpp ${HEADERS_FLOORPLANSTATE}
	${CC} -c FloorplanState.cpp ${INC}
MacrosDisplacement.o: MacrosDisplacement.cpp ${HEADERS_MACROSDISPLACEMENT}
	${CC} -c MacrosDisplacement.cpp ${INC}
clean:
	rm *.o