cmake_minimum_required(VERSION 3.10)

project(744051)

# Specify the source files
set(SOURCES
	src/744051.c
)

# Create the library
add_library(744051 STATIC ${SOURCES})

# Specify include directories
target_include_directories(744051 PUBLIC include)

# Link the necessary libraries
target_link_libraries(744051
	pico_stdlib
	hardware_adc
)
