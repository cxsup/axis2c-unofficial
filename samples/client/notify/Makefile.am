prgbindir=$(prefix)/samples/bin
prgbin_PROGRAMS = notify
notify_SOURCES = notify_client.c

notify_LDADD   =  \
                    -L$(AXIS2C_HOME)/lib \
					-laxutil \
                    -laxis2_axiom \
                    -laxis2_engine \
                    -laxis2_parser \
                    -laxis2_http_sender \
                    -laxis2_http_receiver \
                    $(GUTHTHILA_LIBS)

INCLUDES = @AXIS2INC@

EXTRA_DIST=notify.mk
