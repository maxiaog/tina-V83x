#
# Copyright (C) 2016-2018 OpenWrt.org
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-attrs
PKG_VERSION:=20.2.0
PKG_RELEASE:=1

PYPI_NAME:=attrs
PKG_HASH:=26b54ddbbb9ee1d34d5d3668dd37d6cf74990ab23c828c2888dccdceee395594

PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE
PKG_MAINTAINER:=Jeffery To <jeffery.to@gmail.com>

include ../pypi.mk
include $(BUILD_DIR)/package.mk
include ../python3-package.mk

define Package/python3-attrs
  SECTION:=lang
  CATEGORY:=Languages
  SUBMENU:=Python
  TITLE:=Classes Without Boilerplate
  URL:=https://www.attrs.org/
  DEPENDS:=+python3-light
endef

define Package/python3-attrs/description
attrs is an MIT-licensed Python package with class decorators that ease
the chores of implementing the most common attribute-related object
protocols.
endef

$(eval $(call Py3Package,python3-attrs))
$(eval $(call BuildPackage,python3-attrs))
$(eval $(call BuildPackage,python3-attrs-src))
