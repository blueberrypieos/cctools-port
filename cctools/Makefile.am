# Modified 2026-10-29 for pietoolchain: Removed unused tools.
SUBDIRS=libstuff libmacho ar misc as ld64 man

ACLOCAL_AMFLAGS = -I m4

DSTROOT=
RC_OS=macos

installhdrs:
	cd include; $(MAKE) DSTROOT=$(DSTROOT) RC_OS=$(RC_OS) install
