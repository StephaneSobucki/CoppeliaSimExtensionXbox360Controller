project(xbox_controller)
cmake_minimum_required(VERSION 2.8)

set(sim_include "src/include")
include_directories(${sim_include} "src/")
file(GLOB vrep_src "src/common/*.cpp")
file(GLOB xbox360controller "src/*.cpp")
add_library(simExtXbox360Controller SHARED ${xbox360controller} ${vrep_src})
target_link_libraries(simExtXbox360Controller Xinput9_1_0.lib)