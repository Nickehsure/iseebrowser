noinst_LTLIBRARIES = libpixman.la

libpixman_la_SOURCES = \
	pixman.h \
	pixmanint.h \
	pixman-remap.h \
	pixman-xserver-compat.h \
	pixregion.c \
	pixregionint.h \
	fbpict.h \
	fbpict.c \
	icblt.c \
	icbltone.c \
	iccolor.c \
	icformat.c \
	icimage.c \
	icimage.h \
	icpixels.c \
	icrect.c \
	icrop.h \
	icstipple.c \
	ictrap.c \
	ictransform.c \
	ictri.c \
	icutil.c \
	fbedge.c \
	fbedgeimp.h \
	fbtrap.c \
	fbcompose.c \
	renderedge.c \
	renderedge.h
libpixman_la_CFLAGS = $(PIXMAN_CFLAGS)
libpixman_la_LIBADD = $(PIXMAN_LDADD)

if USE_MMX
noinst_LTLIBRARIES += libpixman-mmx.la
libpixman_mmx_la_SOURCES = \
	fbmmx.c		\
	fbmmx.h
libpixman_mmx_la_CFLAGS = $(PIXMAN_CFLAGS)
libpixman_mmx_la_LIBADD = $(PIXMAN_LDADD)
libpixman_la_LIBADD += libpixman-mmx.la
endif

TESTS = check-pixmanint.sh
EXTRA_DIST = $(TESTS)
