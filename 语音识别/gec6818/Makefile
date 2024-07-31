CC = arm-linux-gcc

CPPFLAGS += -I ./inc
CPPFLAGS += -I ./inc/libxml2
LDFLAGS  += -L ./lib

LDFLAGS += -lxml2
LDFLAGS += -lz


voicectl:voicectl.c common.c
	$(CC) $^ -o $@ $(CPPFLAGS) $(LDFLAGS) -Wall -pthread

clean:
	rm voicectl -rf
