pluginlib_LTLIBRARIES = \
	libfacebook-plugin.la

COMMON_CFLAGS = $(ACCOUNTS_CFLAGS) $(GLADE_CFLAGS) \
		-DG_LOG_DOMAIN=\"$(PACKAGE)\" \
		-DPLUGIN_XML_DIR=\"$(pluginlibdir)/xml\"

COMMON_LDFLAGS = -Wl,--as-needed $(ACCOUNTS_LIBS) $(GLADE_LIBS) \
		 -Wl,--no-undefined -module -avoid-version

libfacebook_plugin_la_SOURCES = facebook-plugin.c
libfacebook_plugin_la_CFLAGS = $(COMMON_CFLAGS)
libfacebook_plugin_la_LDFLAGS = $(COMMON_LDFLAGS)

MAINTAINERCLEANFILES = Makefile.in

