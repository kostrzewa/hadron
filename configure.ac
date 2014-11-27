
AC_INIT([src/sumit.c])
AC_PROG_CXX
AC_CHECK_LIB(gsl, gsl_sf_airy_Ai_e,
             [LIBS="${LIBS} -lgsl -lgslcblas"], 
             [AC_MSG_ERROR([Cannot find Gnu Scientific Library.])],
             [-lgslcblas])
AC_CHECK_HEADER([gsl/gsl_version.h], ,
             [AC_MSG_ERROR([Cannot find GSL headers.])])
AX_PATH_GSL(1.8,
           [],
           [AC_MSG_ERROR([Need GSL Version >= 1.8])])

AC_OUTPUT()

