cmake_minimum_required(VERSION 3.10)
project(HelloFrame)

# Specify the include directory
include_directories(include)

# Add the library
add_library(helloFrame STATIC src/helloFrame.c)

# Optionally, specify an installation directory
install(TARGETS helloFrame DESTINATION lib)
install(DIRECTORY include/ DESTINATION include)
