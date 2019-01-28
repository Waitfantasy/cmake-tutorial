project(HELLO)

cmake_minimum_required(VERSION 3.13.3)

add_subdirectory(src)

install(TARGETS hello RUNTIME DESTINATION /usr/local/bin)

install(PROGRAMS hello.sh
        DESTINATION /usr/local/bin
        PERMISSIONS OWNER_EXECUTE GROUP_EXECUTE)