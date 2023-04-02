# SPDX-License-Identifier: BSD-3-Clause

cmake_minimum_required(VERSION 3.13)

include(pico_sdk_import.cmake)

project(blink)

pico_sdk_init()

add_subdirectory(mrubyc)

add_executable(blink)

target_sources(blink PRIVATE
	blink.c
	)

target_link_libraries(blink PRIVATE
	pico_stdlib
	mrubyc
	)

pico_enable_stdio_usb(blink 1)
pico_enable_stdio_uart(blink 0)

pico_add_extra_outputs(blink)
