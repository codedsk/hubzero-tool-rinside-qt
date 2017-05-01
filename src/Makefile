SRCDIR = qtdensity
BINDIR = ../bin
APP = qtdensity

all:
	. /etc/environ.sh; \
	    use -e -r R-3.4.0; \
	    cd ${SRCDIR}; \
	    qmake; \
	    make all

install:
	cd ${SRCDIR}; \
	    install --mode 0755 -D ${APP} ../${BINDIR}/${APP}

clean:
	cd ${SRCDIR}; \
	    if [ -e Makefile ] ; then \
	        make clean; \
	    fi;

distclean: clean
	rm -f ${BINDIR}/${APP}
