cmake_minimum_required(VERSION 3.20)

add_library(AGUI INTERFACE)
target_include_directories(AGUI INTERFACE ${CMAKE_CURRENT_LIST_DIR}/include)
target_link_libraries(
  AGUI
  INTERFACE
    "-framework Metal -framework Foundation -framework Cocoa -framework CoreGraphics -framework MetalKit"
)
