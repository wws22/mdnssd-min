CC = gcc
CXX = g++
INCLUDES =
CFLAGS = -g -Wall $(INCLUDES)
CXXFLAGS = -g -Wall $(INCLUDES)
LDFLAGS = -g -lstdc++

all: NsdHelper


NsdHelper: NsdHelper.o
	$(CC) $(LDFLAGS) -Wall -o NsdHelper $^

%.o: %.cpp %.h
	$(CC) $(CFLAGS) $(EXTRA_CFLAGS) -c -I. -o $@ $<

clean:
	rm -f NsdHelper *.o
