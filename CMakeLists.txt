######## A simple cmakelists.txt file for OpenCV() #############  
cmake_minimum_required(VERSION 2.8)                            
PROJECT(motempl)                                         

FIND_PACKAGE( OpenCV REQUIRED )                              
INCLUDE_DIRECTORIES( ${OpenCV_INCLUDE_DIRS} )

ADD_EXECUTABLE(motempl motempl.cpp)                         
TARGET_LINK_LIBRARIES (motempl ${OpenCV_LIBS})         
########### end ####################################  
