power_supply-objs := power_supply_core.o

ifeq ($(CONFIG_SYSFS),y)
power_supply-objs += power_supply_sysfs.o
endif

ifeq ($(CONFIG_LEDS_TRIGGERS),y)
power_supply-objs += power_supply_leds.o
endif

ifeq ($(CONFIG_POWER_SUPPLY_DEBUG),y)
EXTRA_CFLAGS += -DDEBUG
endif

obj-$(CONFIG_POWER_SUPPLY)	+= power_supply.o

obj-$(CONFIG_PDA_POWER)		+= pda_power.o
obj-$(CONFIG_BATTERY_S3C)	+= s3c_fake_battery.o

ifeq ($(CONFIG_TARGET_LOCALE_KOR),y)
obj-$(CONFIG_BATTERY_SEC)	+= sec_battery_kor.o
else
obj-$(CONFIG_BATTERY_SEC)	+= sec_battery.o
endif

obj-$(CONFIG_APM_POWER)		+= apm_power.o
obj-$(CONFIG_MAX8925_POWER)	+= max8925_power.o
obj-$(CONFIG_MAX8998_POWER)	+= max8998_power.o
obj-$(CONFIG_WM831X_BACKUP)	+= wm831x_backup.o
obj-$(CONFIG_WM831X_POWER)	+= wm831x_power.o
obj-$(CONFIG_WM8350_POWER)	+= wm8350_power.o
obj-$(CONFIG_TEST_POWER)	+= test_power.o
obj-$(CONFIG_POWER_S5M8751)	+= s5m8751-power.o

obj-$(CONFIG_BATTERY_DS2760)	+= ds2760_battery.o
obj-$(CONFIG_BATTERY_DS2782)	+= ds2782_battery.o
obj-$(CONFIG_BATTERY_PMU)	+= pmu_battery.o
obj-$(CONFIG_BATTERY_OLPC)	+= olpc_battery.o
obj-$(CONFIG_BATTERY_TOSA)	+= tosa_battery.o
obj-$(CONFIG_BATTERY_COLLIE)	+= collie_battery.o
obj-$(CONFIG_BATTERY_WM97XX)	+= wm97xx_battery.o
obj-$(CONFIG_BATTERY_BQ27x00)	+= bq27x00_battery.o
obj-$(CONFIG_BATTERY_DA9030)	+= da9030_battery.o
obj-$(CONFIG_BATTERY_MAX17040)	+= max17040_battery.o
obj-$(CONFIG_BATTERY_Z2)	+= z2_battery.o
obj-$(CONFIG_CHARGER_PCF50633)	+= pcf50633-charger.o

ifeq ($(CONFIG_TARGET_LOCALE_KOR),y)
obj-$(CONFIG_FUELGAUGE_MAX17042) += max17042-fuelgauge-kor.o
else
obj-$(CONFIG_FUELGAUGE_MAX17042) += max17042-fuelgauge.o
endif

obj-$(CONFIG_MAX8997_CHARGER)	+= max8997-charger.o
obj-$(CONFIG_MAX8922_CHARGER)	+= max8922-charger.o
obj-$(CONFIG_SMB136_CHARGER)	+= smb136_charger.o
