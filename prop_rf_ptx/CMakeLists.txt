#
# Copyright (c) 2018 Nordic Semiconductor
#
# SPDX-License-Identifier: LicenseRef-Nordic-5-Clause
#
cmake_minimum_required(VERSION 3.20.0)

find_package(Zephyr REQUIRED HINTS $ENV{ZEPHYR_BASE})
project(NONE)

FILE(GLOB app_sources src/*.c)
# NORDIC SDK APP START

add_subdirectory(${CMAKE_CURRENT_SOURCE_DIR}/../libraries/prop_rf/ ${CMAKE_BINARY_DIR}/libraries/prop_rf/)

target_sources(app PRIVATE ${app_sources})

# NORDIC SDK APP END
