#
# Openwrt feed Makefile for ltq-gphy-firmware
#

include $(TOPDIR)/rules.mk

PKG_NAME:=ltq_fw_PHY_IP
PKG_VERSION:=2.9
PKG_SOURCE_PROTO:=git
PKG_SOURCE_URL:=https://github.com/paldier/ltq_fw_phy_ip.git
PKG_SOURCE_DATE:=2020-03-09
PKG_SOURCE_VERSION:=2a0cb7c6daf66f5071044cdc62c2b423b34edd45


include $(INCLUDE_DIR)/package.mk


define Package/ltq_fw_PHY_IP/Default
  SECTION:=firmware
  CATEGORY:=Lantiq
  URL:=http://www.lantiq.com/
  MAINTAINER:=Lantiq Beteiligungs GmbH
endef

define Package/ltq-gphy-fw-xrx2xx-a1x-f
  $(call Package/ltq_fw_PHY_IP/Default)
  TITLE:=GPHY Firmware XRX2xx A1X Fast Ethernet
endef

define Package/ltq-gphy-fw-xrx2xx-a1x-g
  $(call Package/ltq_fw_PHY_IP/Default)
  TITLE:=GPHY Firmware XRX2xx A1X Gigabit Ethernet
endef

define Package/ltq-gphy-fw-xrx2xx-a2x-f
  $(call Package/ltq_fw_PHY_IP/Default)
  TITLE:=GPHY Firmware XRX2xx A2X Fast Ethernet
endef

define Package/ltq-gphy-fw-xrx2xx-a2x-g
  $(call Package/ltq_fw_PHY_IP/Default)
  TITLE:=GPHY Firmware XRX2xx A2X Gigabit Ethernet
endef

define Package/ltq-gphy-fw-xrx3xx-f
  $(call Package/ltq_fw_PHY_IP/Default)
  TITLE:=GPHY Firmware XRX3xx Fast Ethernet
endef

define Package/ltq-gphy-fw-xrx3xx-g
  $(call Package/ltq_fw_PHY_IP/Default)
  TITLE:=GPHY Firmware XRX3xx Gigabit Ethernet
endef

define Package/ltq-gphy-fw-xrx5xx
  $(call Package/ltq_fw_PHY_IP/Default)
  TITLE:=GPHY Firmware XRX5xx Gigabit Ethernet
endef

define Package/ltq-gphy-fw-prx3xx
  $(call Package/ltq_fw_PHY_IP/Default)
  TITLE:=GPHY Firmware PRX3xx Gigabit Ethernet
endef

define Build/Compile
endef

define Package/ltq-gphy-fw-xrx2xx-a1x-f/install
	$(INSTALL_DIR) $(1)/lib/firmware
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/xRx2xx/ltq_fw_PHY22F_IP_1v4_xRx2xx_A14_T0109.bin \
		$(1)/lib/firmware/ltq_fw_PHY22F_IP_xRx2xx_A14.bin
endef

define Package/ltq-gphy-fw-xrx2xx-a1x-g/install
	$(INSTALL_DIR) $(1)/lib/firmware
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/xRx2xx/ltq_fw_PHY11G_IP_1v4_xRx2xx_A14_R8304.bin \
		$(1)/lib/firmware/ltq_fw_PHY11G_IP_xRx2xx_A14.bin
endef

define Package/ltq-gphy-fw-xrx2xx-a2x-f/install
	$(INSTALL_DIR) $(1)/lib/firmware
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/xRx2xx/ltq_fw_PHY22F_IP_1v5_xRx2xx_A22_RC434.bin \
		$(1)/lib/firmware/ltq_fw_PHY22F_IP_xRx2xx_A22.bin
endef

define Package/ltq-gphy-fw-xrx2xx-a2x-g/install
	$(INSTALL_DIR) $(1)/lib/firmware
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/xRx2xx/ltq_fw_PHY11G_IP_1v6_xRx2xx_A22_R8435.bin \
		$(1)/lib/firmware/ltq_fw_PHY11G_IP_xRx2xx_A22.bin
endef

define Package/ltq-gphy-fw-xrx3xx-f/install
	$(INSTALL_DIR) $(1)/lib/firmware
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/xRx3xx/ltq_fw_PHY22F_IP_1v5_xRx3xx_A21_RC434.bin \
		$(1)/lib/firmware/ltq_fw_PHY22F_IP_xRx3xx_A21.bin
endef

define Package/ltq-gphy-fw-xrx3xx-g/install
	$(INSTALL_DIR) $(1)/lib/firmware
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/xRx3xx/ltq_fw_PHY11G_IP_1v6_xRx3xx_A21_R8435.bin \
		$(1)/lib/firmware/ltq_fw_PHY11G_IP_xRx3xx_A21.bin
endef

define Package/ltq-gphy-fw-xrx5xx/install
	$(INSTALL_DIR) $(1)/lib/firmware
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/xRx5xx/ltq_fw_PHY11G_IP_1v1_xRx5xx_A21_R8548.bin \
		$(1)/lib/firmware/ltq_fw_PHY11G_IP_xRx5xx_A21.bin
endef

define Package/ltq-gphy-fw-prx3xx/install
	$(INSTALL_DIR) $(1)/lib/firmware
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/prx3xx/ltq_fw_PHY31G_IP_prx3xx_A11_R0651.bin \
		$(1)/lib/firmware/ltq_fw_PHY31G_IP_prx3xx_A11.bin
	$(INSTALL_DATA) $(PKG_BUILD_DIR)/prx3xx/ltq_fw_PHY31G_IP_prx3xx_Bxx_R0728.bin \
		$(1)/lib/firmware/ltq_fw_PHY31G_IP_prx3xx_Bxx.bin
endef

$(eval $(call BuildPackage,ltq-gphy-fw-xrx2xx-a1x-f))
$(eval $(call BuildPackage,ltq-gphy-fw-xrx2xx-a1x-g))
$(eval $(call BuildPackage,ltq-gphy-fw-xrx2xx-a2x-f))
$(eval $(call BuildPackage,ltq-gphy-fw-xrx2xx-a2x-g))
$(eval $(call BuildPackage,ltq-gphy-fw-xrx3xx-f))
$(eval $(call BuildPackage,ltq-gphy-fw-xrx3xx-g))
$(eval $(call BuildPackage,ltq-gphy-fw-xrx5xx))
$(eval $(call BuildPackage,ltq-gphy-fw-prx3xx))
