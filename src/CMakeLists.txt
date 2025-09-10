file(GLOB HEADER_LIST "${PROJECT_SOURCE_DIR}/include/debugging/*.h;${PROJECT_SOURCE_DIR}/include/tests/*.h")

add_library(debugginglib LIBRARY.cpp ${HEADER_LIST})

target_include_directories(debugginglib PUBLIC ../include/debugging)

target_compile_features(debugginglib PUBLIC cxx_std_20)