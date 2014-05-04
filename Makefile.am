bin_SCRIPTS = zfs-replicate

man8_MANS = zfs-replicate.8
CLEANFILES = $(man8_MANS)

zfs-replicate.8: $(srcdir)/zfs-replicate
	-$(HELP2MAN) --output=$@ \
	  --name='replicate ZFS datasets' \
	  --section=8 \
	  --no-info \
	  --version-string=$(PACKAGE_VERSION) \
	  $(top_srcdir)/zfs-replicate
