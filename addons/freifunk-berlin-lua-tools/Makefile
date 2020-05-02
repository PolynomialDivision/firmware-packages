
include $(TOPDIR)/rules.mk

LUCI_TITLE:=Freifunk Berlin lua tools
LUCI_DEPENDS:=luci-lib-base
PKG_RELEASE:=1

include ../../freifunk-berlin-generic.mk

#  URL:=http://berlin.freifunk.net

# call BuildPackage - OpenWrt buildroot signature
$(eval $(call BuildPackage,$(PKG_NAME)))
