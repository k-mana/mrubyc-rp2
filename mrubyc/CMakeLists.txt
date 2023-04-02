# SPDX-License-Identifier: BSD-3-Clause

cmake_minimum_required(VERSION 3.13)

set(MRBC_USE_HAL "rp2040")
set(MRBC_REQUIRE_ALIGNMENT 32)
set(MAX_REGS_SIZE 256)
set(MAX_SYMBOLS_COUNT 500)
option(MRUBYC_SAMPLE "Building mruby/c samples" OFF)

add_subdirectory(mrubyc)
