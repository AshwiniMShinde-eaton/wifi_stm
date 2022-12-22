cmake_minimum_required(VERSION 3.13.1)

target_sources(app PRIVATE
    "stm32_cyhal_gpio.c"
    "stm32_cyhal_lptimer.c"
	"stm32_cyhal_sdio.c"
	"stm32_cyhal_spi.c"
	"stm32_cyhal_trng.c"
#	"stm32_cyhal_uart.c"
)
