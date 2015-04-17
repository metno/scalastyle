
bin_SCRIPTS = scalastyle

scalastyle: src/scalastyle.in
	sed 's,__DATAROOT__,$(datarootdir),' $< > $@
	chmod 775 $@

EXTRA_DIST = src/scalastyle.in

CLEANFILES = scalastyle

dist_sysconf_DATA = etc/scalastyle-config.xml
javadir = $(datarootdir)/java
dist_java_DATA = lib/scalastyle_2.11-0.6.0-batch.jar
