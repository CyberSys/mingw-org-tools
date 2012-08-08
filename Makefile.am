bin_PROGRAMS = gendef genidl widl
gendef_SOURCES = \
  gendef/fsredir.c \
  gendef/fsredir.h \
  gendef/compat_string.c \
  gendef/compat_string.h \
  gendef/gendef.c \
  gendef/gendef.h \
  gendef/gendef_def.c

gendef_CFLAGS = $(AM_CFLAGS) -O3 -g -std=gnu99 -Werror -Wall -Wextra -pedantic  -Wno-pedantic-ms-format

genidl_SOURCES = \
  genidl/fsredir.c \
  genidl/fsredir.h \
  genidl/genidl.c \
  genidl/genidl_cfg.h \
  genidl/genidl_config.c \
  genidl/genidl_typinfo.c \
  genidl/genidl_typinfo.h \
  genidl/genidl_typeinfo.c \
  genidl/genidl_typeinfo.h \
  genidl/genidl_readpe.c \
  genidl/genidl_readpe.h \
  genidl/genidl_dumpidl.c

genidl_CFLAGS = $(AM_CFLAGS) -O3 -g -std=gnu99 -Werror -Wall -Wextra -pedantic  -Wno-pedantic-ms-format

widl_SOURCES = \
  widl/client.c \
  widl/expr.c \
  widl/hash.c \
  widl/header.c \
  widl/parser.tab.c \
  widl/parser.yy.c \
  widl/port/port.c \
  widl/proxy.c \
  widl/register.c \
  widl/server.c \
  widl/typegen.c \
  widl/typelib.c \
  widl/typetree.c \
  widl/utils.c \
  widl/widl.c \
  widl/write_msft.c \
  widl/wpp/ppl.yy.c \
  widl/wpp/ppy.tab.c \
  widl/wpp/preproc.c \
  widl/wpp/wpp.c

widl_CFLAGS = $(AM_CFLAGS) -I$(top_srcdir)/widl/include -O3 -g -std=gnu99 -Werror -Wall -Wformat -pedantic  -Wno-pedantic-ms-format
