CC := g++
CPPFLAGS := -std=c++11
objects := test.o
libs := -pthread

all: my_exec

my_exec: $(objects)
	$(CC) $^ $(libs) -o $@
	#g++ test.o -lpthread -o my_exec

#test.o: test.cc
%.o: %.c
	$(CC) $(CPPFLAGS) -c $<
	#g++ -std=c++11 -c test.cc
	
.PHONY: clean help
clean:
	rm my_exec $(objects)

help:
	@echo "make"
	@echo "make clean"
