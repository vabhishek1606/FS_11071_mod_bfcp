include $(switch_srcdir)/build/modmake.rulesam
MODNAME = mod_bfcp

mod_LTLIBRARIES = mod_bfcp.la

mod_bfcp_la_SOURCES  = mod_bfcp.c mod_bfcp.h bfcp_interface.c bfcp_interface.h bfcp_media.c bfcp_thread.h
mod_bfcp_CFLAGS   = $(AM_CFLAGS)
mod_bfcp_LIBADD   = $(switch_builddir)/libfreeswitch.la
mod_bfcp_LDFLAGS  = -avoid-version -module -no-undefined -shared -bfcprel

LOCAL_CFLAGS = -I$(switch_srcdir)/libs/libbfcp/bfcpmsg -I$(switch_srcdir)/libs/libbfcp/bfcpsrvclt/bfcpsrv -I$(switch_srcdir)/libs/libbfcp/bfcpsrvclt/bfcpclt -I$(switch_srcdir)/src/mod/applications/mod_bfcp -I$(switch_srcdir)/src/include  -I$(switch_srcdir)/libs/libbfcp -lbfcpmsg -I$(switch_srcdir)/libs/libbfcp -lbfcpsrv -I$(switch_srcdir)/libs/libbfcp -lbfcpclt
LOCAL_LDFLAGS = -L$(switch_srcdir)/libs/libbfcp/bfcpmsg -L$(switch_srcdir)/libs/libbfcp/bfcpsrvclt/bfcpsrv -L$(switch_srcdir)/libs/libbfcp/bfcpsrvclt/bfcpclt