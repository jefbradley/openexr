## Process this file with automake to produce Makefile.in

bin_PROGRAMS = exrenvmap

INCLUDES = -I$(top_builddir) \
           -I$(top_srcdir)/IlmImf -I$(top_srcdir)/config \
           @ILMBASE_CXXFLAGS@ $(ILMBASE_CFLAGS) $(ZLIB_CFLAGS)

LDADD = @ILMBASE_LDFLAGS@ $(ILMBASE_LIBS) \
	$(top_builddir)/IlmImf/libIlmImf.la \
	$(ZLIB_LIBS)

exrenvmap_SOURCES = main.cpp EnvmapImage.cpp EnvmapImage.h \
		    readInputImage.cpp readInputImage.h \
		    resizeImage.cpp resizeImage.h \
		    blurImage.cpp blurImage.h \
		    makeCubeMap.cpp makeCubeMap.h \
		    makeLatLongMap.cpp makeLatLongMap.h \
		    namespaceAlias.h

noinst_HEADERS = EnvmapImage.h makeCubeMap.h makeLatLongMap.h

EXTRA_DIST = main.cpp EnvmapImage.cpp EnvmapImage.h \
	     readInputImage.cpp readInputImage.h \
	     resizeImage.cpp resizeImage.h \
	     blurImage.cpp blurImage.h \
	     makeCubeMap.cpp makeCubeMap.h \
	     makeLatLongMap.cpp makeLatLongMap.h \
	     namespaceAlias.h \
             CMakeLists.txt
        
