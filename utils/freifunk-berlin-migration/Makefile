include $(TOPDIR)/rules.mk

PKG_NAME:=freifunk-berlin-migration
PKG_VERSION:=0.6.2
PKG_RELEASE:=2

PKG_BUILD_DIR:=$(BUILD_DIR)/$(PKG_NAME)

include $(INCLUDE_DIR)/package.mk

define Package/freifunk-berlin-migration
  SECTION:=freifunk-berlin
  CATEGORY:=freifunk-berlin
  TITLE:=Freifunk Berlin configuration migration script
  URL:=http://github.com/freifunk-berlin/packages_berlin
  DEPENDS+= +freifunk-berlin-lib-guard
  PKGARCH:=all
endef

define Package/freifunk-berlin-migration/description
  Freifunk Berlin configuration migration script
endef

define Build/Prepare
	mkdir -p $(PKG_BUILD_DIR)
endef

define Build/Configure
endef

define Build/Compile
endef

define Package/freifunk-berlin-migration/install
	$(INSTALL_DIR) $(1)/etc/uci-defaults
	$(CP) ./uci-defaults/* $(1)/etc/uci-defaults
	$(INSTALL_DIR) $(1)/lib/functions
	$(CP) ./files/* $(1)/
endef

$(eval $(call BuildPackage,freifunk-berlin-migration))

