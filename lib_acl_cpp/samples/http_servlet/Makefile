include ../Makefile.in
#EXTLIBS = -lpolarssl
#EXTLIBS = -lz -liconv
#EXTLIBS = -lz
#Path for SunOS
ifeq ($(findstring SunOS, $(UNIXNAME)), SunOS)
	EXTLIBS = -lz -liconv
else
	EXTLIBS = -lz
endif
ifeq ($(findstring FreeBSD, $(UNIXNAME)), FreeBSD)
	EXTLIBS += -L/usr/local/lib -liconv
endif
PROG = http_servlet
