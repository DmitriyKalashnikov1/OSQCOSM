######## A simple cmakelists.txt file for OpenCV() #############  
cmake_minimum_required(VERSION 2.8)                            
PROJECT(OSQCOSM)                                         

FIND_PACKAGE( OpenCV REQUIRED )                              
INCLUDE_DIRECTORIES( ${OpenCV_INCLUDE_DIRS} )

ADD_EXECUTABLE(OSQCOSM OSQCOSM.cpp)                         
TARGET_LINK_LIBRARIES (OSQCOSM ${OpenCV_LIBS})         
########### end ####################################  
