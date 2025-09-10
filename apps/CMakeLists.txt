add_executable(debugging debugging.cpp)
target_compile_features(debugging PRIVATE cxx_std_20)

target_link_libraries(debugging PRIVATE debuggingLIB)