add_library(stbiw stb_image_write.cpp)

if (NOT CMAKE_BUILD_TYPE)
    set(CMAKE_BUILD_TYPE Release)
endif()

set_target_properties(stbiw PROPERTIES LINKER_LANGUAGE CXX)
target_include_directories(stbiw PUBLIC .)