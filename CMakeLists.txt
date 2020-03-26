cmake_minimum_required(VERSION 3.0.0)

project(liblinear VERSION 0.1.0)

add_subdirectory(blas)

set(SOURCES linear.cpp linear.h svm-scale.c  tron.cpp tron.h) #train.c predict.c 

add_library(liblinear SHARED ${SOURCES})

target_link_libraries(liblinear PUBLIC blas)

