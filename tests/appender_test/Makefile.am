# This is the only program that uses '=' to assign to
# noinst_PROGRAMS. All other test cases and loggingserver use '+='.
noinst_PROGRAMS = appender_test

appender_test_sources = %D%/main.cxx
appender_test_SOURCES = $(appender_test_sources)

appender_test_LDADD = $(liblog4cplus_la_file)

if BUILD_WITH_WCHAR_T_SUPPORT
noinst_PROGRAMS += appender_testU
appender_testU_CPPFLAGS = $(AM_CPPFLAGS) -DUNICODE=1
appender_testU_SOURCES = $(appender_test_sources)
appender_testU_LDADD = $(liblog4cplusU_la_file)
endif
