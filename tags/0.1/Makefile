
GFORTRAN=gfortran
FFLAGS=
VERSION=0.1
SOURCES=lithflex1.f lithflex2.f
OBJS=${SOURCES:.f=.o}

all: lithflex1 lithflex2

lithflex1: lithflex1.f
	${GFORTRAN} ${FFLAGS} -o lithflex1 lithflex1.f

lithflex2: lithflex2.f
	${GFORTRAN} ${FFLAGS} -o lithflex2 lithflex2.f

dist:
	@mkdir lithflex-${VERSION}
	@cp ${SOURCES} lithflex-${VERSION}
	@cp Makefile lithflex-${VERSION}
	@tar cvfz lithflex-${VERSION}.tar.gz lithflex-${VERSION} 
	@rm -rf lithflex-${VERSION}

clean:
	@rm -f lithflex1 lithflex2 ${OBJS} core

