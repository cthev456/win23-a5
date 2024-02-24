CC = gcc

SOURCES = main.c addition.c subtraction.c multiplication.c division.c

OBJECTS = $(SOURCES:.c=.o)

HEADER = operations.h

EXECUTABLE = calculator

all: $(EXECUTABLE)

# Rule to compile the object files
%.o: %.c $(HEADER)
	$(CC) -c $< -o $@

# Rule to link the object files into the executable
$(EXECUTABLE): $(OBJECTS)
	$(CC) $(OBJECTS) -o $@

# Clean target to remove object files and executable
clean:
	rm -f $(OBJECTS) $(EXECUTABLE)
