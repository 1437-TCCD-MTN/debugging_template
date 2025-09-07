file(GLOB HEADER_LIST "${PROJECT_SOURCE_DIR}/include/PROJECT/*.h;${PROJECT_SOURCE_DIR}/include/tests/*.h")

add_library(PROJECTlib PROJECT_LIBRARY.cpp ${HEADER_LIST})

target_include_directories(PROJECTlib PUBLIC ../include/PROJECT)

target_compile_features(PROJECTlib PUBLIC cxx_std_20)