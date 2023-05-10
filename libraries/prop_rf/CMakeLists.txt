#
# Copyright (c) 2019 Nordic Semiconductor ASA
#
# SPDX-License-Identifier: LicenseRef-Nordic-5-Clause
#

target_include_directories(app PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})
target_sources(app PUBLIC ${CMAKE_CURRENT_SOURCE_DIR}/prop_rf.c)
target_sources(app PUBLIC ${CMAKE_CURRENT_SOURCE_DIR}/prop_rf_ppi.c)
#target_sources(app PUBLIC ${CMAKE_CURRENT_SOURCE_DIR}/prop_rf_dppi.c)
