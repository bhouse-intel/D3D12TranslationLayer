# Copyright (c) Microsoft Corporation.
# Licensed under the MIT License.
cmake_minimum_required(VERSION 3.13)
project(dxbcparser)

include_directories(test "C:/Program Files (x86)/Windows Kits/10/include/10.0.22000.0/um")

add_library(dxbcparser STATIC
    src/BlobContainer.cpp
    src/DXBCUtils.cpp
    include/BlobContainer.h
    include/DXBCUtils.h
    include/pch.h)

target_include_directories(dxbcparser
    PUBLIC include
    PUBLIC ../external)
    
