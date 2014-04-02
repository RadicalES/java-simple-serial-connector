CXX=g++
CPPFLAGS=-fPIC
CPPFLAGS+=-I/usr/lib/jvm/jdk1.7.0_51/include
CPPFLAGS+=-I/usr/lib/jvm/jdk1.7.0_51/include/linux

all: jssc

jssc: jssc.o
	$(CXX) -shared -o libjSSC-2.8_x86.so jssc.o 

jssc.o: jssc.cpp ../jssc_SerialNativeInterface.h
	$(CXX) $(CPPFLAGS) -c jssc.cpp

