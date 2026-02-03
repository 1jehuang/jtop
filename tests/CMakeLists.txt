# SPDX-License-Identifier: Apache-2.0

include(FetchContent)
FetchContent_Declare(
  googletest
  GIT_REPOSITORY https://github.com/google/googletest.git
  GIT_TAG v1.17.0
  FIND_PACKAGE_ARGS NAMES GTest
)
FetchContent_MakeAvailable(googletest)

add_library(libjtop_test)
target_include_directories(libjtop_test PUBLIC ${PROJECT_SOURCE_DIR}/src)
target_link_libraries(libjtop_test libjtop GTest::gtest_main)

add_executable(btop_test tools.cpp)
target_link_libraries(btop_test libjtop_test)

include(GoogleTest)
gtest_discover_tests(btop_test)
