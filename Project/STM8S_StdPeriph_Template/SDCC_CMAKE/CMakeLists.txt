cmake_minimum_required(VERSION 3.5)

project ( Project )

set(MCU stm8)
set(STM8S_CFG STM8S208)
set(CMAKE_C_FLAGS "-m${MCU} -D${STM8S_CFG} -V --opt-code-size --verbose")

set( STM8_LIB_DIR ../../../Libraries/STM8S_StdPeriph_Driver )
set( SRC_DIR ../.. )

include_directories (
    ${STM8_LIB_DIR}/inc
     ../.
     )

add_subdirectory( ${STM8_LIB_DIR} build/STM8S_StdPeriph_Driver )


add_executable ( SampleProject
     ${SRC_DIR}/main.c
     ${SRC_DIR}/stm8s_it.c
     ${SRC_DIR}/stm8s_it.h
     ${SRC_DIR}/stm8s_conf.h
     )

target_link_libraries(SampleProject
     stm8_spd
     )
