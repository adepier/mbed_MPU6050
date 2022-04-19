 
set(MPU_SOURCES MPU6050.cpp) 
add_library(mbed_MPU6050 STATIC ${PID_SOURCES})
target_link_libraries( mbed_MPU6050 mbed-os mbed_I2Cdev)

set(MPU_HEADER_DIR ${CMAKE_CURRENT_SOURCE_DIR} )
target_include_directories(mbed_MPU6050 PUBLIC ${MPU_HEADER_DIR})