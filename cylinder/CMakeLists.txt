cmake_minimum_required(VERSION 2.8)
find_package(VTK)
message(${VTK_USE_FILE})
include(${VTK_USE_FILE})
add_executable(main Cylinder.cxx)
target_link_libraries(main ${VTK_LIBRARIES})
