cmake_minimum_required(VERSION 3.24)
project(MyApp CXX)

get_latest_conan_version(LATEST_CONAN_VERSION)
message(STATUS "Latest Conan version: ${LATEST_CONAN_VERSION}")
download_conan(VERSION ${LATEST_CONAN_VERSION} DESTINATION ${CMAKE_BINARY_DIR}/conan)
