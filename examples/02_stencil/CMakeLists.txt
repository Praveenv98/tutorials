# Copyright (c) 2016 Thomas Heller
#
# Distributed under the Boost Software License, Version 1.0. (See accompanying
# file LICENSE_1_0.txt or copy at http://www.boost.org/LICENSE_1_0.txt)

cmake_minimum_required(VERSION 2.8)

project(stencil CXX)

find_package(HPX REQUIRED)

add_executable(stencil_serial stencil_serial.cpp)
hpx_setup_target(stencil_serial)

add_executable(stencil_parallel_0 stencil_parallel_0.cpp)
hpx_setup_target(stencil_parallel_0)

add_executable(stencil_parallel_1 stencil_parallel_1.cpp)
hpx_setup_target(stencil_parallel_1)