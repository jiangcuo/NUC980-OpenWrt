include $(TOPDIR)/rules.mk

PKG_NAME:=openGw

PKG_VERSION:=20240116
PKG_RELEASE:=1
PKG_MAINTAINER:=JiangCuo

PKG_BUILD_DIR:=$(BUILD_DIR)/$(PKG_NAME)
include $(INCLUDE_DIR)/package.mk

define Package/$(PKG_NAME)
	SECTION:=net
	CATEGORY:=Utilities
	PKGARCH:=all
	TITLE:=openGW
endef

define Package/$(PKG_NAME)/description
	opengw
endef


define Package/$(PKG_NAME)/postinst
endef


define Package/$(PKG_NAME)/preinst
endef


define Build/Prepare
endef



define Build/Configure
endef



define Build/Compile
endef



define Package/$(PKG_NAME)/install
	$(INSTALL_DIR) $(1)/usr/share/opengw/
	$(INSTALL_DIR) $(1)/etc/init.d/
	$(INSTALL_BIN) ./root/usr/share/opengw/opengw $(1)/usr/share/opengw/
	cp -r ./root/usr/share/opengw/webroot $(1)/usr/share/opengw/
	cp -r ./root/usr/share/opengw/config $(1)/usr/share/opengw/
	$(INSTALL_BIN) ./root/etc/init.d/opengw $(1)/etc/init.d/
endef


$(eval $(call BuildPackage,$(PKG_NAME)))
