cmake_minimum_required(VERSION 3.0.0)
project(hello VERSION 0.1.0)

# SET(EXECUTABLE_OUTPUT_PATH ${PROJECT_BINARY_DIR}/bin)
# SET(LIBRARY_OUTPUT_PATH ${PROJECT_BINARY_DIR}/lib)
ADD_SUBDIRECTORY(src bin)


INSTALL(FILES COPYRIGHT README DESTINATION share/doc/cmake/t2)
INSTALL(PROGRAMS runhello.sh DESTINATION bin)
INSTALL(DIRECTORY doc/ DESTINATION share/doc/cmake/t2)
