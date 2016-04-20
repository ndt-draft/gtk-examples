
CC = g++

CFLAGS = -Wall			 	\
	-DG_DISABLE_DEPRECATED 	 	\
	-DGDK_DISABLE_DEPRECATED 	\
	-DGDK_PIXBUF_DISABLE_DEPRECATED \
	-DGTK_DISABLE_DEPRECATED \
	-std=c++11

simple: simple.cc 
	$(CC) simple.cc -o simple $(CFLAGS) `pkg-config gtkmm-3.0 --cflags --libs`

clean: 
	rm -f *.o simple
