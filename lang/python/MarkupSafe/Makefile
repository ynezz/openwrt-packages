# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=MarkupSafe
PKG_VERSION:=1.1.1
PKG_RELEASE:=2

PKG_SOURCE:=$(PKG_NAME)-$(PKG_VERSION).tar.gz
PKG_SOURCE_URL:=https://files.pythonhosted.org/packages/source/M/MarkupSafe
PKG_HASH:=29872e92839765e546828bb7754a68c418d927cd064fd4708fab9fe9c8bb116b

PKG_MAINTAINER:=Daniel Golle <daniel@makrotopia.org>
PKG_LICENSE:=BSD-3-Clause
PKG_LICENSE_FILES:=LICENSE.rst

PKG_BUILD_DIR:=$(BUILD_DIR)/$(PKG_NAME)-$(PKG_VERSION)

include $(INCLUDE_DIR)/package.mk
include ../python3-package.mk

define Package/python3-markupsafe
  SECTION:=lang
  CATEGORY:=Languages
  SUBMENU:=Python
  TITLE:=MarkupSafe
  URL:=https://palletsprojects.com/p/markupsafe/
  DEPENDS:=+python3-light
  VARIANT:=python3
endef

define Package/python3-markupsafe/description
  MarkupSafe implements a text object that escapes characters so it is safe to use in HTML and XML.
endef

$(eval $(call Py3Package,python3-markupsafe))
$(eval $(call BuildPackage,python3-markupsafe))
$(eval $(call BuildPackage,python3-markupsafe-src))
