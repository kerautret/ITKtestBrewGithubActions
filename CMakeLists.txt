project(ITKtestBrewGithubActions)
cmake_minimum_required(VERSION 3.1)
 if(COMMAND cmake_policy)
      cmake_policy(SET CMP0003 NEW)
    endif(COMMAND cmake_policy)


find_package(ITK REQUIRED)
include(${ITK_USE_FILE})
   
add_executable(testITK testITK.cpp)
  
target_link_libraries(testITK ${ITK_LIBRARIES})


