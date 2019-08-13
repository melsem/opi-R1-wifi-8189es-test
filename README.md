# opi-R1-wifi-8189es-test
* Модуль собирается без ошибок. Но не проверял как работает.
* Платку только собираюсь покупать.

# Пакет kmod-rtl8189es для OpenWrt-master_kernel-4.19:
* Дрaйвер wifi радиомодуля: rtl8189es

* Поместить all-add-wifi-rtl8189es-opi-R1.patch в $(BUILD_DIR)
* и дать команду:
```
patch -p1 < all-add-wifi-rtl8189es-opi-R1.patch
```

* Compile
```
./scripts/feeds update -a
./scripts/feeds install -a
make menuconfig
```
* Выбрать в "Kernel modules" - "Wireless Drivers test-RTL8189ES"
* отметить "rtl8189es"
```
make V=s
```

