INCLUDES = $(STLPORT_CFLAGS) -I$(top_srcdir)/OgreMain/include -I$(top_srcdir)/Samples/Common/CEGUIRenderer/include -I$(top_srcdir)/Samples/Common/include @CEGUI_CFLAGS@

noinst_PROGRAMS = Gui
Gui_SOURCES = Gui.cpp
Gui_LDFLAGS = -L$(top_builddir)/OgreMain/src -L$(top_builddir)/Samples/Common/CEGUIRenderer/src
Gui_LDADD = -lOgreMain @CEGUI_LIBS@ -lCEGUIOgreRenderer

install-exec-local:
	$(INSTALL_PROGRAM) .libs/Gui $(top_builddir)/Samples/Common/bin/Gui
