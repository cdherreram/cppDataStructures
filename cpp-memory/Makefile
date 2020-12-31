EXE = main
OBJS = main.o Cube.o
CLEAN_RM = rm -d -r

include ../_make/generic.mk

# Directory-specific rules:
addressOf: addressOf.cpp
	$(LD) $^ $(LDFLAGS) -o $@

foo: foo.cpp
	$(LD) $^ $(LDFLAGS) -o $@

puzzle: puzzle.cpp
	$(LD) $^ $(LDFLAGS) .objs/Cube.o -o $@

all: addressOf foo puzzle
CLEAN_RM += addressOf foo puzzle
