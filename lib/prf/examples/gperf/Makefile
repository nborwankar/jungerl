ERLC = $(OTP_ROOT)/bin/erlc
EFLAGS = +debug_info
ERLS = $(wildcard *.erl)
BEAMS = $(patsubst %.erl, %.beam, $(ERLS))

#.PHONY: default all 

default: all
all: $(BEAMS)

clean:
	rm -f *.beam

%.beam : %.erl
	$(ERLC) $(EFLAGS) $<
