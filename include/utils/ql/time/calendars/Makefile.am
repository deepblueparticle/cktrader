
AM_CPPFLAGS = -I${top_srcdir} -I${top_builddir}

this_includedir=${includedir}/${subdir}
this_include_HEADERS = \
	all.hpp \
	argentina.hpp \
	australia.hpp \
	bespokecalendar.hpp \
	brazil.hpp \
	canada.hpp \
	china.hpp \
	czechrepublic.hpp \
	denmark.hpp \
	finland.hpp \
	germany.hpp \
	hongkong.hpp \
	hungary.hpp \
	iceland.hpp \
	india.hpp \
	indonesia.hpp \
	israel.hpp \
	italy.hpp \
	japan.hpp \
	jointcalendar.hpp \
	mexico.hpp \
	newzealand.hpp \
	norway.hpp \
	nullcalendar.hpp \
	poland.hpp \
	romania.hpp \
	russia.hpp \
	saudiarabia.hpp \
	singapore.hpp \
	slovakia.hpp \
	southafrica.hpp \
	southkorea.hpp \
	sweden.hpp \
	switzerland.hpp \
	taiwan.hpp \
	target.hpp \
	turkey.hpp \
	ukraine.hpp \
	unitedkingdom.hpp \
	unitedstates.hpp \
	weekendsonly.hpp

libCalendars_la_SOURCES = \
	argentina.cpp \
	australia.cpp \
	bespokecalendar.cpp \
	brazil.cpp \
	canada.cpp \
	china.cpp \
	czechrepublic.cpp \
	denmark.cpp \
	finland.cpp \
	germany.cpp \
	hongkong.cpp \
	hungary.cpp \
	iceland.cpp \
	india.cpp \
	indonesia.cpp \
	israel.cpp \
	italy.cpp \
	japan.cpp \
	jointcalendar.cpp \
	mexico.cpp \
	newzealand.cpp \
	norway.cpp \
	poland.cpp \
	romania.cpp \
	russia.cpp \
	saudiarabia.cpp \
	singapore.cpp \
	slovakia.cpp \
	southafrica.cpp \
	southkorea.cpp \
	sweden.cpp \
	switzerland.cpp \
	taiwan.cpp \
	target.cpp \
	turkey.cpp \
	ukraine.cpp \
	unitedkingdom.cpp \
	unitedstates.cpp \
	weekendsonly.cpp

noinst_LTLIBRARIES = libCalendars.la

all.hpp: Makefile.am
	echo "/* This file is automatically generated; do not edit.     */" > $@
	echo "/* Add the files to be included into Makefile.am instead. */" >> $@
	echo >> $@
	for i in $(filter-out all.hpp, $(this_include_HEADERS)); do \
		echo "#include <${subdir}/$$i>" >> $@; \
	done
	echo >> $@
	subdirs='$(SUBDIRS)'; for i in $$subdirs; do \
		echo "#include <${subdir}/$$i/all.hpp>" >> $@; \
	done

