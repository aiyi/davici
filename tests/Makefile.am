AM_CPPFLAGS = \
	-I$(top_srcdir)

AM_CFLAGS = -Wall

noinst_LTLIBRARIES = libtester.la

libtester_la_SOURCES = \
	tester.c tester.h

LDADD = \
	$(top_builddir)/libdavici.la \
	libtester.la

TESTS = \
	cmd.tst \
	dump.tst \
	many.tst \
	event.tst \
	stream.tst \
	badsock.tst \
	cmdunknown.tst \
	eventunknown.tst

cmd_tst_SOURCES = cmd.c
dump_tst_SOURCES = dump.c
many_tst_SOURCES = many.c
event_tst_SOURCES = event.c
stream_tst_SOURCES = stream.c
badsock_tst_SOURCES = badsock.c
cmdunknown_tst_SOURCES = cmdunknown.c
eventunknown_tst_SOURCES = eventunknown.c

check_PROGRAMS = $(TESTS)
