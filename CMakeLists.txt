cmake_minimum_required(VERSION 4.2)
project(platform_sandbox VERSION 0.1.0 LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

find_package(SFML 3 COMPONENTS graphics window system REQUIRED)

add_executable(plaftorm_sandbox
                        src/main
)


target_link_libraries(platform_sandbox PRIVATE
                                sfml-graphics
                                sfml-window
                                sfml-system
)
