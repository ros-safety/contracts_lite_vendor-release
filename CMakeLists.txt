cmake_minimum_required(VERSION 3.5)
project(contracts_lite_vendor)

# Use C++14
set(CMAKE_CXX_STANDARD 14)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

if(CMAKE_COMPILER_IS_GNUCXX OR CMAKE_CXX_COMPILER_ID MATCHES "Clang")
  add_compile_options(-Wall -Wextra -Wpedantic)
endif()

# find dependencies
find_package(ament_cmake REQUIRED)

set(contracts_lite_DESTDIR ${CMAKE_CURRENT_BINARY_DIR}/contracts_lite_install)

include(ExternalProject)
ExternalProject_Add(contracts_lite
  GIT_REPOSITORY https://github.com/ros-safety/contracts_lite.git
  GIT_TAG 0.5.0
  GIT_SHALLOW TRUE
  BUILD_IN_SOURCE TRUE
  INSTALL_DIR ${contracts_lite_DESTDIR}
  CONFIGURE_COMMAND ${CMAKE_COMMAND} -DCMAKE_INSTALL_PREFIX=<INSTALL_DIR> -DCMAKE_POSITION_INDEPENDENT_CODE=ON .
)

ament_export_include_directories(include)

install(DIRECTORY ${contracts_lite_DESTDIR}/include/
  DESTINATION include
)

ament_package()
