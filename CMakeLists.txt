cmake_minimum_required(VERSION 3.0.0)
project(koza VERSION 0.1.0)

include(CTest)
enable_testing()


#include("build/conanbuildinfo.cmake")
#conan_basic_setup()
add_executable(koza main.cpp)
#target_link_libraries(koza ${CONAN_LIBS})

set(CPACK_PROJECT_NAME ${PROJECT_NAME})
set(CPACK_PROJECT_VERSION ${PROJECT_VERSION})
include(CPack)
