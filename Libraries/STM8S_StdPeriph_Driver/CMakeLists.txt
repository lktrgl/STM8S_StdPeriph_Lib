cmake_minimum_required(VERSION 3.5)

project ( Project )

set( STM8_LIB_DIR . )

if( ${STM8S_CFG} EQUAL "STM8S105"
    OR ${STM8S_CFG} EQUAL "STM8S005"
    OR ${STM8S_CFG} EQUAL "STM8S103"
    OR ${STM8S_CFG} EQUAL "STM8S003"
    OR ${STM8S_CFG} EQUAL "STM8S001"
    OR ${STM8S_CFG} EQUAL "STM8S903"
    OR ${STM8S_CFG} EQUAL "STM8AF626x"
    OR ${STM8S_CFG} EQUAL "STM8AF622x"
    )
set( STM8_LIB_SOURCES_ADC1
    ${STM8_LIB_DIR}/inc/stm8s_adc1.h
    ${STM8_LIB_DIR}/src/stm8s_adc1.c
    )
endif()

if( ${STM8S_CFG} EQUAL "STM8S208"
    OR ${STM8S_CFG} EQUAL "STM8S207"
    OR ${STM8S_CFG} EQUAL "STM8S007"
    OR ${STM8S_CFG} EQUAL "STM8AF52Ax"
    OR ${STM8S_CFG} EQUAL "STM8AF62Ax"
    )
set( STM8_LIB_SOURCES_ADC2
    ${STM8_LIB_DIR}/inc/stm8s_adc2.h
    ${STM8_LIB_DIR}/src/stm8s_adc2.c
    )
endif()

if( ${STM8S_CFG} EQUAL "STM8S208"
    OR ${STM8S_CFG} EQUAL "STM8AF52Ax"
    )
set( STM8_LIB_SOURCES_CAN
    ${STM8_LIB_DIR}/inc/stm8s_can.h
    ${STM8_LIB_DIR}/src/stm8s_can.c
    )
endif()

if( ${STM8S_CFG} EQUAL "STM8S208"
   OR ${STM8S_CFG} EQUAL "STM8S207"
   OR ${STM8S_CFG} EQUAL "STM8S007"
   OR ${STM8S_CFG} EQUAL "STM8S103"
   OR ${STM8S_CFG} EQUAL "STM8S003"
   OR ${STM8S_CFG} EQUAL "STM8S001"
   OR ${STM8S_CFG} EQUAL "STM8S903"
   OR ${STM8S_CFG} EQUAL "STM8AF52Ax"
   OR ${STM8S_CFG} EQUAL "STM8AF62Ax"
    )
set( STM8_LIB_SOURCES_UART1
    ${STM8_LIB_DIR}/inc/stm8s_uart1.h
    ${STM8_LIB_DIR}/src/stm8s_uart1.c
    )
endif()

if( ${STM8S_CFG} EQUAL "STM8S105"
   OR ${STM8S_CFG} EQUAL "STM8S005"
   OR ${STM8S_CFG} EQUAL "STM8AF626x"
    )
set( STM8_LIB_SOURCES_UART2
    ${STM8_LIB_DIR}/inc/stm8s_uart2.h
    ${STM8_LIB_DIR}/src/stm8s_uart2.c
    )
endif()

if( ${STM8S_CFG} EQUAL "STM8S208"
   OR ${STM8S_CFG} EQUAL "STM8S207"
   OR ${STM8S_CFG} EQUAL "STM8S007"
   OR ${STM8S_CFG} EQUAL "STM8AF52Ax"
   OR ${STM8S_CFG} EQUAL "STM8AF62Ax"
    )
set( STM8_LIB_SOURCES_UART3
    ${STM8_LIB_DIR}/inc/stm8s_uart3.h
    ${STM8_LIB_DIR}/src/stm8s_uart3.c
    )
endif()

if( ${STM8S_CFG} EQUAL "STM8AF622x"
    )
set( STM8_LIB_SOURCES_UART4
    ${STM8_LIB_DIR}/inc/stm8s_uart4.h
    ${STM8_LIB_DIR}/src/stm8s_uart4.c
    )
endif()

if( ${STM8S_CFG} EQUAL "STM8S208"
   OR ${STM8S_CFG} EQUAL "STM8S207"
   OR ${STM8S_CFG} EQUAL "STM8S007"
   OR ${STM8S_CFG} EQUAL "STM8S103"
   OR ${STM8S_CFG} EQUAL "STM8S003"
   OR ${STM8S_CFG} EQUAL "STM8S001"
   OR ${STM8S_CFG} EQUAL "STM8S105"
   OR ${STM8S_CFG} EQUAL "STM8S005"
   OR ${STM8S_CFG} EQUAL "STM8AF52Ax"
   OR ${STM8S_CFG} EQUAL "STM8AF62Ax"
   OR ${STM8S_CFG} EQUAL "STM8AF626x"
    )
set( STM8_LIB_SOURCES_TIM2
    ${STM8_LIB_DIR}/inc/stm8s_tim2.h
    ${STM8_LIB_DIR}/src/stm8s_tim2.c
    )
endif()

if( ${STM8S_CFG} EQUAL "STM8S208"
   OR ${STM8S_CFG} EQUAL "STM8S207"
   OR ${STM8S_CFG} EQUAL "STM8S007"
   OR ${STM8S_CFG} EQUAL "STM8S105"
   OR ${STM8S_CFG} EQUAL "STM8S005"
   OR ${STM8S_CFG} EQUAL "STM8AF52Ax"
   OR ${STM8S_CFG} EQUAL "STM8AF62Ax"
   OR ${STM8S_CFG} EQUAL "STM8AF626x"
    )
set( STM8_LIB_SOURCES_TIM3
    ${STM8_LIB_DIR}/inc/stm8s_tim3.h
    ${STM8_LIB_DIR}/src/stm8s_tim3.c
    )
endif()

if( ${STM8S_CFG} EQUAL "STM8S208"
   OR ${STM8S_CFG} EQUAL "STM8S207"
   OR ${STM8S_CFG} EQUAL "STM8S007"
   OR ${STM8S_CFG} EQUAL "STM8S103"
   OR ${STM8S_CFG} EQUAL "STM8S003"
   OR ${STM8S_CFG} EQUAL "STM8S001"
   OR ${STM8S_CFG} EQUAL "STM8S105"
   OR ${STM8S_CFG} EQUAL "STM8S005"
   OR ${STM8S_CFG} EQUAL "STM8AF52Ax"
   OR ${STM8S_CFG} EQUAL "STM8AF62Ax"
   OR ${STM8S_CFG} EQUAL "STM8AF626x"
    )
set( STM8_LIB_SOURCES_TIM4
    ${STM8_LIB_DIR}/inc/stm8s_tim4.h
    ${STM8_LIB_DIR}/src/stm8s_tim4.c
    )
endif()

if( ${STM8S_CFG} EQUAL "STM8S903"
   OR ${STM8S_CFG} EQUAL "STM8AF622x"
    )
set( STM8_LIB_SOURCES_TIM5_6
    ${STM8_LIB_DIR}/inc/stm8s_tim5.h
    ${STM8_LIB_DIR}/src/stm8s_tim5.c
    ${STM8_LIB_DIR}/inc/stm8s_tim6.h
    ${STM8_LIB_DIR}/src/stm8s_tim6.c
    )
endif()

set( STM8_LIB_SOURCES
    ${STM8_LIB_SOURCES_ADC1}
    ${STM8_LIB_SOURCES_ADC2}
    ${STM8_LIB_SOURCES_CAN}
    ${STM8_LIB_SOURCES_UART1}
    ${STM8_LIB_SOURCES_UART2}
    ${STM8_LIB_SOURCES_UART3}
    ${STM8_LIB_SOURCES_UART4}
    ${STM8_LIB_SOURCES_TIM2}
    ${STM8_LIB_SOURCES_TIM3}
    ${STM8_LIB_SOURCES_TIM4}
    ${STM8_LIB_SOURCES_TIM5_6}
    ${STM8_LIB_DIR}/inc/stm8s_tim1.h
    ${STM8_LIB_DIR}/inc/stm8s_wwdg.h
    ${STM8_LIB_DIR}/inc/stm8s_beep.h
    ${STM8_LIB_DIR}/inc/stm8s_exti.h
    ${STM8_LIB_DIR}/inc/stm8s_rst.h
    ${STM8_LIB_DIR}/inc/stm8s_iwdg.h
    ${STM8_LIB_DIR}/inc/stm8s_awu.h
    ${STM8_LIB_DIR}/inc/fireworks.h
    ${STM8_LIB_DIR}/inc/stm8s_spi.h
    ${STM8_LIB_DIR}/inc/stm8s_clk.h
    ${STM8_LIB_DIR}/inc/stm8s_flash.h
    ${STM8_LIB_DIR}/inc/stm8s.h
    ${STM8_LIB_DIR}/inc/stm8s_gpio.h
    ${STM8_LIB_DIR}/inc/stm8s_i2c.h
    ${STM8_LIB_DIR}/inc/stm8s_itc.h

    ${STM8_LIB_DIR}/src/stm8s_tim1.c
    ${STM8_LIB_DIR}/src/stm8s_i2c.c
    ${STM8_LIB_DIR}/src/stm8s_clk.c
    ${STM8_LIB_DIR}/src/stm8s_rst.c
    ${STM8_LIB_DIR}/src/stm8s_awu.c
    ${STM8_LIB_DIR}/src/stm8s_itc.c
    ${STM8_LIB_DIR}/src/stm8s_gpio.c
    ${STM8_LIB_DIR}/src/stm8s_flash.c
    ${STM8_LIB_DIR}/src/fireworks.c
    ${STM8_LIB_DIR}/src/stm8s_exti.c
    ${STM8_LIB_DIR}/src/stm8s_wwdg.c
    ${STM8_LIB_DIR}/src/stm8s_beep.c
    ${STM8_LIB_DIR}/src/stm8s_iwdg.c
    ${STM8_LIB_DIR}/src/stm8s_spi.c
     )

add_library ( stm8_spd
    ${STM8_LIB_SOURCES}
     )

include_directories (
    ${STM8_LIB_DIR}/inc
     )
