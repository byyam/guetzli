LDLIBS += $(shell pkg-config --libs libpng libjpeg)
CXXFLAGS += -std=c++11 -I.. $(shell pkg-config --cflags libpng libjpeg)
LINK.o = $(LINK.cc)

EXECUTABLES = butteraugli

all: butteraugli.o butteraugli_main.o $(EXECUTABLES)

butteraugli: butteraugli.o butteraugli_main.o

.PHONY: clean
clean: 
	rm *.o $(EXECUTABLES)
