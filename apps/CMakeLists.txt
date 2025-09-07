add_executable(PROJECT.cpp)
target_compile_features(PROJECT PRIVATE cxx_std_20)

target_link_libraries(PROJECT PRIVATE PROJECTLIB)