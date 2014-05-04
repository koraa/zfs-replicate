# zfs-replicate - Robustly replicate ZFS file systems.
# Copyright (c) 2014 Neal H. Walfield <neal@walfield.org>
#
# zfs-replicate is free software; you can redistribute it and/or
# modify it under the terms of the GNU General Public License as
# published by the Free Software Foundation; either version 3 of the
# License, or (at your option) any later version.
#
# zfs-replicate is distributed in the hope that it will be useful, but
# WITHOUT ANY WARRANTY; without even the implied warranty of
# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
# General Public License for more details.
#
# You should have received a copy of the GNU General Public License
# along with this program.  If not, see <http://www.gnu.org/licenses/>.

dist_bin_SCRIPTS = zfs-replicate

man8_MANS = zfs-replicate.8
CLEANFILES = $(man8_MANS)

zfs-replicate.8: $(srcdir)/zfs-replicate
	-$(HELP2MAN) --output=$@ \
	  --name='replicate ZFS datasets' \
	  --section=8 \
	  --no-info \
	  --version-string=$(PACKAGE_VERSION) \
	  $(top_srcdir)/zfs-replicate

EXTRA_DIST = debian/rules debian/compat debian/changelog debian/source \
	debian/source/format debian/control debian/copyright debian/docs
