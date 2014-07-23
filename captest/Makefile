# simple makefile to make quick development life easier (and avoid
# pain with cmake)

SRC = ../src
LIBOBJ = $(SRC)/ctrl.o $(SRC)/ctrl-gen.o $(SRC)/device.o $(SRC)/diag.o $(SRC)/frame.o $(SRC)/frame-mjpeg.o $(SRC)/init.o $(SRC)/misc.o $(SRC)/stream.o
OBJS = captest.o 

CFLAGS = -Wall -g -O0 -I ../include

captest: $(OBJS) $(LIBOBJ)
	gcc -g -o captest $(OBJS) $(LIBOBJ) -lusb-1.0 -lpthread -ljpeg

clean:
	rm -f *.o captest
