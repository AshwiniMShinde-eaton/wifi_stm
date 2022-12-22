cmake_minimum_required(VERSION 3.13.1)

target_sources(app PRIVATE 
"cyhal_system.c"
#"wifi_bt_if.c"
#"wifi_bt_if.h"
)

#target_include_directories(app PUBLIC "./")