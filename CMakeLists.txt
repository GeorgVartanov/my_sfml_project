cmake_minimum_required(VERSION 3.15)
project(my_sfml_project VERSION 0.1.0)

include(CTest)
enable_testing()


add_subdirectory(src)
add_subdirectory(dependencies)



set(CPACK_PROJECT_NAME ${PROJECT_NAME})
set(CPACK_PROJECT_VERSION ${PROJECT_VERSION})
include(CPack)
