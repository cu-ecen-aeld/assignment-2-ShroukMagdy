# Variables
#CC = aarch64-none-linux-gnu-gcc
CC = gcc
CFLAGS = -Wall -Wextra -I.
#DEPS = foo.h
OBJ = writer.o 
TARGET = writer

# Rule to create the final executable
$(TARGET): $(OBJ)
	$(CC) -o $@ $^

# Rule to compile .c files to .o files
%.o: %.c $(DEPS)
	$(CC) -c -o $@ $< $(CFLAGS)

# Clean up
.PHONY: clean
clean:
	rm -f $(OBJ) $(TARGET)

