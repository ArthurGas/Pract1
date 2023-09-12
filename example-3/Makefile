# make-file для третьего примера

.PHONY: all debug release clean

TARGET = Kazino-Royal.cpp
RELEASE_FLAGS = -O2 -Wall -DNDEBUG
DEBUG_FLAGS   = -g -O0 -Wall
RELEASE_EXEC  = Kazino-Royal
DEBUG_EXEC    = Kazino-Royal-dbg
#SOURCE        =

all: debug release

debug: $(DEBUG_EXEC)

$(DEBUG_EXEC): $(TARGET)
	g++ $(DEBUG_FLAGS) $(TARGET) -o $(DEBUG_EXEC) 

release: $(RELEASE_EXEC)

$(RELEASE_EXEC): $(TARGET)
	g++ $(RELEASE_FLAGS) $(TARGET) -o $(RELEASE_EXEC)

clean:
	rm -f $(RELEASE_EXEC) $(DEBUG_EXEC)
