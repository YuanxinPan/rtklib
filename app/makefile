#
# make all cui applications by gcc
#

BINDIR = /usr/local/bin
DIRS   = rnx2rtkp # pos2kml str2str convbin rtkrcv

all:
	@for i in $(DIRS); do make -C $$i/gcc; done

install:
	@echo installing...
	@for i in $(DIRS); do cp $$i/gcc/$$i $(BINDIR); done

clean:
	@echo cleaning up...
	@for i in $(DIRS); do make -C $$i/gcc clean; done

