# SU^2 Makefile.am for GDC
# Stanford University Aerospace Design Lab
#
# Created: 		3/16/13
# Last updated: 	4/09/13
#
# Created by: 	M. Colonno
# Updated by: 	T. Economon
#
##########################

ACLOCAL_AMFLAGS = ${ACLOCAL_FLAGS}

bin_PROGRAMS = ../bin/SU2_GDC

___bin_SU2_GDC_SOURCES = ../include/SU2_GDC.hpp \
		../src/SU2_GDC.cpp

___bin_SU2_GDC_CXXFLAGS =
___bin_SU2_GDC_LDADD = ../../Common/lib/libSU2.a

# always link to built dependencies from ./externals
___bin_SU2_GDC_CXXFLAGS += @su2_externals_INCLUDES@
___bin_SU2_GDC_LDADD += @su2_externals_LIBS@

# if BUILD_CGNS
___bin_SU2_GDC_CXXFLAGS += @CGNS_CXX@
___bin_SU2_GDC_LDADD += @CGNS_LD@
# endif

# if BUILD_MUTATIONPP
___bin_SU2_GDC_CXXFLAGS += @MUTATIONPP_CXX@
___bin_SU2_GDC_LDADD += @MUTATIONPP_LD@
# endif

# if BUILD_JSONCPP
___bin_SU2_GDC_CXXFLAGS += @JSONCPP_CXX@
___bin_SU2_GDC_LDADD += @JSONCPP_LD@
# endif
