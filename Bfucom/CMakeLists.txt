# CMakeList.txt : CMake project for Bfucom, include source and define
# project specific logic here.
#
cmake_minimum_required (VERSION 3.8)

# Add source to this project's executable.
add_executable (Bfucom "Bfucom.cpp" "Bfucom.h")

find_package(fmt REQUIRED)
target_link_libraries(Bfucom PRIVATE fmt::fmt)
