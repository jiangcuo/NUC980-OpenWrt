include $(TOPDIR)/rules.mk

PKG_NAME:=aic8800fw
PKG_VERSION:=20230117
PKG_RELEASE:=1

PKG_MAINTAINER:=Jiangcuo <jiangcuo@bingsin.com>

include $(INCLUDE_DIR)/package.mk

define Package/aic8800fw
  PKGARCH:=all
  SECTION:=firmware
  CATEGORY:=Firmware
  TITLE:=aic8800 WIFI BT firmware
endef

define Build/Compile
endef

define Package/aic8800fw/install
	$(INSTALL_DIR) $(1)/vendor/etc/firmware/
	$(CP) ./fw/* $(1)/vendor/etc/firmware/
endef

$(eval $(call BuildPackage,aic8800fw))
