cmake_minimum_required(VERSION 3.0.0)

project(blas VERSION 0.1.0)

set(SOURCES blas.h blasp.h daxpy.c ddot.c dnrm2.c dscal.c)

add_library(blas SHARED ${SOURCES})

