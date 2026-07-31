cmake_minimum_required(VERSION 3.28)

# library core sources
set(LCD1602_I2C_SRCS
    ${CMAKE_CURRENT_LIST_DIR}/lcd1602_i2c.c)

# include directories
set(LCD1602_I2C_INCLUDES
    ${CMAKE_CURRENT_LIST_DIR})

# register library to the system
add_library(lcd1602_i2c INTERFACE)
target_sources(lcd1602_i2c INTERFACE ${LCD1602_I2C_SRCS})
target_include_directories(lcd1602_i2c INTERFACE ${LCD1602_I2C_INCLUDES})
