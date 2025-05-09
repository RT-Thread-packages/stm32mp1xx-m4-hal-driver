from building import *
import os

cwd = GetCurrentDir()
path = [os.path.join(cwd, 'Inc')]
src_path = os.path.join(cwd, 'Src')

CPPDEFINES = ['USE_HAL_DRIVER']

src = [
os.path.join(src_path, 'stm32mp1xx_hal.c'),
os.path.join(src_path, 'stm32mp1xx_hal_hsem.c'),
os.path.join(src_path, 'stm32mp1xx_hal_exti.c'),
os.path.join(src_path, 'stm32mp1xx_hal_ipcc.c'),
os.path.join(src_path, 'stm32mp1xx_hal_cortex.c'),
os.path.join(src_path, 'stm32mp1xx_hal_dma.c'),
os.path.join(src_path, 'stm32mp1xx_hal_dma_ex.c'),
os.path.join(src_path, 'stm32mp1xx_hal_mdma.c'),
os.path.join(src_path, 'stm32mp1xx_hal_pwr.c'),
os.path.join(src_path, 'stm32mp1xx_hal_pwr_ex.c'),
os.path.join(src_path, 'stm32mp1xx_hal_rcc.c'),
os.path.join(src_path, 'stm32mp1xx_hal_rcc_ex.c'),
os.path.join(src_path, 'stm32mp1xx_hal_gpio.c'),
os.path.join(src_path, 'stm32mp1xx_hal_adc.c'),
os.path.join(src_path, 'stm32mp1xx_hal_adc_ex.c'),
os.path.join(src_path, 'stm32mp1xx_hal_dac.c'),
os.path.join(src_path, 'stm32mp1xx_hal_dac_ex.c'),
os.path.join(src_path, 'stm32mp1xx_hal_i2c.c'),
os.path.join(src_path, 'stm32mp1xx_hal_i2c_ex.c'),
os.path.join(src_path, 'stm32mp1xx_hal_spi.c'),
os.path.join(src_path, 'stm32mp1xx_hal_tim.c'),
os.path.join(src_path, 'stm32mp1xx_hal_tim_ex.c'),
]

if GetDepend(['RT_USING_SERIAL']) or GetDepend(['RT_USING_NANO', 'RT_USING_CONSOLE']):
    src += [os.path.join(src_path, 'stm32mp1xx_hal_uart.c')]
    src += [os.path.join(src_path, 'stm32mp1xx_hal_uart_ex.c')]

if GetDepend(['RT_USING_USB']):
    src += [os.path.join(src_path, 'stm32mp1xx_hal_pccard.c')]
    src += [os.path.join(src_path, 'stm32mp1xx_hal_pcd.c')]
    src += [os.path.join(src_path, 'stm32mp1xx_hal_pcd_ex.c')]
    src += [os.path.join(src_path, 'stm32mp1xx_hal_hcd.c')]
    src += [os.path.join(src_path, 'stm32mp1xx_ll_usb.c')]

if GetDepend(['RT_USING_CAN']):
    src += [os.path.join(src_path, 'stm32mp1xx_hal_can.c')]
    
if GetDepend(['BSP_USING_WWDG']):
    src += [os.path.join(src_path, 'stm32mp1xx_hal_wwdg.c')]

if GetDepend(['BSP_USING_LPTIM']):
    src += [os.path.join(src_path, 'stm32mp1xx_hal_lptim.c')]

if GetDepend(['RT_USING_RTC']):
    src += [os.path.join(src_path, 'stm32mp1xx_hal_rtc.c')]
    src += [os.path.join(src_path, 'stm32mp1xx_hal_rtc_ex.c')]

if GetDepend(['RT_USING_WDT']):
    src += [os.path.join(src_path, 'stm32mp1xx_hal_wwdg.c')]

if GetDepend(['RT_USING_SDIO']):
    src += [os.path.join(src_path, 'stm32mp1xx_ll_sdmmc.c')]
    src += [os.path.join(src_path, 'stm32mp1xx_hal_sd.c')]
    src += [os.path.join(src_path, 'stm32mp1xx_ll_delayblock.c')]

if GetDepend(['RT_USING_AUDIO']):
    src += [os.path.join(src_path, 'stm32mp1xx_hal_sai.c')]
    src += [os.path.join(src_path, 'stm32mp1xx_hal_sai_ex.c')]
    
if GetDepend(['BSP_USING_DCMI']):
    src += [os.path.join(src_path, 'stm32mp1xx_hal_dcmi.c')]
 
if GetDepend(['BSP_USING_FMC']):
    src += [os.path.join(src_path, 'stm32mp1xx_ll_fmc.c')]
    src += [os.path.join(src_path, 'stm32mp1xx_ll_fsmc.c')]

if GetDepend(['BSP_USING_SDRAM']):
    src += [os.path.join(src_path, 'stm32mp1xx_hal_sdram.c')]

if GetDepend(['BSP_USING_EXT_FMC_IO']):
    src += [os.path.join(src_path, 'stm32mp1xx_hal_sram.c')]

if GetDepend(['BSP_USING_ON_CHIP_FLASH']):
    src += [os.path.join(src_path, 'stm32mp1xx_hal_flash.c')]
    src += [os.path.join(src_path, 'stm32mp1xx_hal_flash_ex.c')]
    src += [os.path.join(src_path, 'stm32mp1xx_hal_flash_ramfunc.c')]

if GetDepend(['BSP_USING_LTDC']):
    src += [os.path.join(src_path, 'stm32mp1xx_hal_ltdc.c')]
    src += [os.path.join(src_path, 'stm32mp1xx_hal_ltdc_ex.c')]
    src += [os.path.join(src_path, 'stm32mp1xx_hal_dma2d.c')]
    src += [os.path.join(src_path, 'stm32mp1xx_ll_dma2d.c')]
    src += [os.path.join(src_path, 'stm32mp1xx_hal_dsi.c')]

if GetDepend(['BSP_USING_FDCAN']):
    src += [os.path.join(src_path, 'stm32mp1xx_hal_fdcan.c')]

if GetDepend(['BSP_USING_QSPI']):
    src += [os.path.join(src_path, 'stm32mp1xx_hal_qspi.c')]

if GetDepend(['BSP_USING_SPDIFRX']):
    src += [os.path.join(src_path, 'stm32mp1xx_hal_spdifrx.c')]

if GetDepend(['BSP_USING_DFSDM']):
    src += [os.path.join(src_path, 'stm32mp1xx_hal_dfsdm.c')]
    src += [os.path.join(src_path, 'stm32mp1xx_hal_dfsdm_ex.c')]

if GetDepend(['BSP_USING_HASH']):
    src += [os.path.join(src_path, 'stm32mp1xx_hal_hash.c')]
    src += [os.path.join(src_path, 'stm32mp1xx_hal_hash_ex.c')]

if GetDepend(['BSP_USING_CRC']):
    src += [os.path.join(src_path, 'stm32mp1xx_hal_crc.c')]
    src += [os.path.join(src_path, 'stm32mp1xx_hal_crc_ex.c')]

if GetDepend(['BSP_USING_RNG']):
    src += [os.path.join(src_path, 'stm32mp1xx_hal_rng.c')]

if GetDepend(['BSP_USING_CRYP']):
    src += [os.path.join(src_path, 'stm32mp1xx_hal_cryp.c')]
    src += [os.path.join(src_path, 'stm32mp1xx_hal_cryp_ex.c')]

if GetDepend(['BSP_USING_RTC']):
    src += [os.path.join(src_path, 'stm32mp1xx_hal_rtc.c')]
    src += [os.path.join(src_path, 'stm32mp1xx_hal_rtc_ex.c')]
    
group = DefineGroup('STM32MP-HAL', src, depend = ['PKG_USING_STM32MP1_M4_HAL_DRIVER'], CPPPATH = path, CPPDEFINES = CPPDEFINES)

Return('group')
