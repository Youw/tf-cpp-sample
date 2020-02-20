cmake_minimum_required(VERSION 3.10)

set(CMAKE_CXX_STANDARD 14)

project(TF_CPP_SAMPLE)

find_package(TensorflowCC REQUIRED COMPONENTS Shared)

add_executable(${PROJECT_NAME}
    source/TensorFlowInference.cpp
    source/TensorFlowInference.cpp
)
target_link_libraries(${PROJECT_NAME}
     TensorflowCC::Shared
)
