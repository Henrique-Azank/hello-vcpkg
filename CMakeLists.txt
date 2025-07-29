
# Minimum version of CMAKE required
cmake_minimum_required(VERSION 3.10)

# Name of the project
project(TemplateProject VERSION 1.0 LANGUAGES CXX)

# Find the required libraries for the project
find_package(fmt CONFIG REQUIRED)

# Add the executable target
add_executable(${PROJECT_NAME} src/main.cpp)

# Link the required libraries
target_link_libraries(${PROJECT_NAME} PRIVATE fmt::fmt)
