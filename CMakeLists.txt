add_contract(marathon marathon ${CMAKE_CURRENT_SOURCE_DIR}/src/marathon.cpp)
target_include_directories(marathon.wasm
   PUBLIC
   ${CMAKE_CURRENT_SOURCE_DIR}/include)

set_target_properties(marathon.wasm
   PROPERTIES
   RUNTIME_OUTPUT_DIRECTORY "${CMAKE_CURRENT_BINARY_DIR}")
