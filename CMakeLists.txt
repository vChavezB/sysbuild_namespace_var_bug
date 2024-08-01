cmake_minimum_required(VERSION 3.20.0)

message("MY VAR VALUE ${MY_VAR}")
find_package(Zephyr REQUIRED HINTS $ENV{ZEPHYR_BASE})
project(sysbuild_var_bug)
target_sources(app PRIVATE main.c)
