# SPDX-License-Identifier: Apache-2.0

zephyr_include_directories(./)
zephyr_library_include_directories(
    ${ZEPHYR_BASE}/modules/hal_infineon
  )

zephyr_library_sources_ifdef(CONFIG_WIFI_CYW43XXX cyw43xxx_drv.c)
zephyr_compile_definitions(CYBSP_WIFI_CAPABLE)

zephyr_compile_definitions(CY_RTOS_AWARE)

add_subdirectory("wifi-host-driver")
add_subdirectory("pal/targets/TARGET_STM32/Inc")
add_subdirectory("pal/targets/TARGET_STM32/Src")
add_subdirectory("pal/hal/include")
