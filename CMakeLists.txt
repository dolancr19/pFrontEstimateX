#--------------------------------------------------------
# The CMakeLists.txt for:                 pFrontEstimateX
# Author(s):                                      John Li
#--------------------------------------------------------

FILE(GLOB SRC *.cpp)

ADD_EXECUTABLE(pFrontEstimateX ${SRC})
   
TARGET_LINK_LIBRARIES(pFrontEstimateX
   ${MOOS_LIBRARIES}
   ufield
   mbutil
   m
   pthread
   henrik_anneal
)
