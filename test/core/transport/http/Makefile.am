TESTS = test_http_transport
check_PROGRAMS = test_http_transport
noinst_PROGRAMS = test_http_transport
SUBDIRS =
test_http_transport_SOURCES = test_http_transport.c

test_http_transport_LDADD   =  \
                                $(LDFLAGS) \
		                    ../../../../util/src/libaxutil.la \
       						../../../../axiom/src/om/libaxis2_axiom.la \
						    $(top_builddir)/neethi/src/libneethi.la \
		                    ../../../../axiom/src/parser/$(WRAPPER_DIR)/libaxis2_parser.la \
							$(top_builddir)/src/core/engine/libaxis2_engine.la \
							$(top_builddir)/src/core/transport/http/sender/libaxis2_http_sender.la

INCLUDES = -I${CUTEST_HOME}/include \
            -I$(top_builddir)/include \
            -I ../../../../util/include \
            -I ../../../../axiom/include

if AXIS2_JSON_ENABLED
test_http_transport_LDADD += $(JSON_LIBS) \
							$(top_builddir)/src/core/transport/http/common/libaxis2_http_common.la

INCLUDES += $(JSON_CFLAGS)
endif
