include $(TOPDIR)/rules.mk

PKG_NAME:=network-quality-server
PKG_RELEASE:=$(AUTORELEASE)

PKG_SOURCE_PROTO:=git
PKG_SOURCE_URL:=https://github.com/network-quality/server
PKG_SOURCE_DATE:=2021-12-16
PKG_SOURCE_VERSION:=00e49e7f999a7da2d0b6f12f98f0a454bbfab592
PKG_MIRROR_HASH:=77061778ad1af7c2984693cc01e6cbcec0f87c99b7a02cc5240e2d9d2e43d6f9

PKG_MAINTAINER:=FIXME
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE.md

PKG_BUILD_DEPENDS:=golang/host
PKG_BUILD_PARALLEL:=1
PKG_USE_MIPS16:=0
GO_PKG:=github.com/network-quality/server/go

include $(INCLUDE_DIR)/package.mk
include ../../lang/golang/golang-package.mk

define Package/network-quality-server
  SECTION:=net
  CATEGORY:=Network
  TITLE:=The Network Quality Server
  URL:=https://github.com/network-quality/server
  DEPENDS:=$(GO_ARCH_DEPENDS)
endef

define Package/network-quality-server/description
  The Network Quality Server project is Go example server that can be used by
  the networkQuality command line tool available in macOS 12.
endef

$(eval $(call GoBinPackage,network-quality-server))
$(eval $(call BuildPackage,network-quality-server))
