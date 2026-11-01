# Modified 2026-10-29 for pietoolchain: Removed unused tools.
bin_PROGRAMS =  \
	lipo \
	size \
	strings \
	nm \
	libtool \
	install_name_tool \
	strip \
	nmedit \
	ranlib \
	codesign_allocate \
	ctf_insert \
	vtool

LDADD =  \
        $(top_builddir)/libmacho/libmacho.la \
	$(top_builddir)/libstuff/libstuff.la \
	$(DL_LIB) \
	$(LTO_RPATH) \
	$(MATH_LIB) \
	$(REALLOCF_LIB)

AM_CFLAGS = -I$(top_srcdir)/include -I$(top_srcdir)/include/foreign -I$(top_srcdir)/libstuff $(WARNINGS) $(LTO_DEF) -D__DARWIN_UNIX03 $(ENDIAN_FLAG)

lipo_SOURCES = lipo.c
size_SOURCES = size.c
strings_SOURCES = strings.c
nm_SOURCES = nm.c
libtool_SOURCES = libtool.c
install_name_tool_SOURCES = install_name_tool.c
strip_SOURCES = strip.c
nmedit_SOURCES = strip.c
nmedit_CFLAGS = -DNMEDIT $(AM_CFLAGS)
ranlib_SOURCES = libtool.c
ranlib_CFLAGS = -DRANLIB $(AM_CFLAGS)
codesign_allocate_SOURCES = codesign_allocate.c
ctf_insert_SOURCES= ctf_insert.c
vtool_SOURCES= vtool.c
