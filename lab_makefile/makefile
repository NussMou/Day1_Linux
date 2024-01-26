CC=gcc
CFLAGS=-Wall -Werror -O3
TARGET=program
SOURCES=main.c module1.c module2.c
OBJECTS=$(SOURCES:.c=.o)

all: $(TARGET)
$(TARGET): $(OBJECTS)
	$(CC) $(CFLAGS) -o $@ $^

%.o: %.c
	$(CC) $(CFLAGS) -c $<

clean:
	rm -f $(TARGET) $(OBJECTS)

.PHONY: all clean
