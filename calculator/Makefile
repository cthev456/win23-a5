CC = gcc

CFLAGS = -Wall -Wextra -Werror

SOURCES = main.c addition.c subtraction.c multiplication.c division.c

OBJECTS = $(SOURCES:.c=.o)

HEADER = operations.h

EXECUTABLE = calculator

all: $(EXECUTABLE)

# Rule to compile the object files
%.o: %.c $(HEADER)
	$(CC) $(CFLAGS) -c $< -o $@

# Rule to link the object files into the executable
$(EXECUTABLE): $(OBJECTS)
	$(CC) $(CFLAGS) $(OBJECTS) -o $@

# Clean target to remove object files and executable
clean:
	rm -f $(OBJECTS) $(EXECUTABLE)
