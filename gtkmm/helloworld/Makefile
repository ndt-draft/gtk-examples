
CC = g++

CFLAGS = -Wall			 	\
	-DG_DISABLE_DEPRECATED 	 	\
	-DGDK_DISABLE_DEPRECATED 	\
	-DGDK_PIXBUF_DISABLE_DEPRECATED \
	-DGTK_DISABLE_DEPRECATED \
	-std=c++11

GTKMM = `pkg-config gtkmm-3.0 --cflags --libs`

helloworld: main.o helloworld.o
	$(CC) main.o helloworld.o -o helloworld $(GTKMM)

main.o: main.cc
	$(CC) -c main.cc -o main.o $(CFLAGS) $(GTKMM)

helloworld.o: helloworld.cc
	$(CC) -c helloworld.cc -o helloworld.o $(CFLAGS) $(GTKMM)

clean: 
	rm -f *.o helloworld
