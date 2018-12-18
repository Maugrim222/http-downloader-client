# cmake_minimum_required(VERSION <specify CMake version here>)
project(Assignment)

set(CMAKE_CXX_STANDARD 11)

include_directories(include)
include_directories(src)

add_executable(Assignment
        bin/downloader
        src/downloader.c
        src/http.c
        src/http.h
        src/queue.c
        src/queue.h
        test/http_download.c
        test/http_test.c
        test/queue_test.c
        large.txt
        Makefile
        small.txt
        test.txt
        test_download.sh)
