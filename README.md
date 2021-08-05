# STM32F401CC_CM4_LAB_Codes

## Functions
HAL_StatusTypeDef 	HAL_ADC_Start (ADC_HandleTypeDef *hadc)
 	Enables ADC and starts conversion of the regular channels.
HAL_StatusTypeDef 	HAL_ADC_Stop (ADC_HandleTypeDef *hadc)
 	Disables ADC and stop conversion of regular channels.
HAL_StatusTypeDef 	HAL_ADC_PollForConversion (ADC_HandleTypeDef *hadc, uint32_t Timeout)
 	Poll for regular conversion complete.
HAL_StatusTypeDef 	HAL_ADC_PollForEvent (ADC_HandleTypeDef *hadc, uint32_t EventType, uint32_t Timeout)
 	Poll for conversion event.
HAL_StatusTypeDef 	HAL_ADC_Start_IT (ADC_HandleTypeDef *hadc)
 	Enables the interrupt and starts ADC conversion of regular channels.
HAL_StatusTypeDef 	HAL_ADC_Stop_IT (ADC_HandleTypeDef *hadc)
 	Disables the interrupt and stop ADC conversion of regular channels.
void 	HAL_ADC_IRQHandler (ADC_HandleTypeDef *hadc)
 	Handles ADC interrupt request.
HAL_StatusTypeDef 	HAL_ADC_Start_DMA (ADC_HandleTypeDef *hadc, uint32_t *pData, uint32_t Length)
 	Enables ADC DMA request after last transfer (Single-ADC mode) and enables ADC peripheral.
HAL_StatusTypeDef 	HAL_ADC_Stop_DMA (ADC_HandleTypeDef *hadc)
 	Disables ADC DMA (Single-ADC mode) and disables ADC peripheral.
uint32_t 	HAL_ADC_GetValue (ADC_HandleTypeDef *hadc)
 	Gets the converted value from data register of regular channel.
__weak void 	HAL_ADC_ConvCpltCallback (ADC_HandleTypeDef *hadc)
 	Regular conversion complete callback in non blocking mode.
__weak void 	HAL_ADC_ConvHalfCpltCallback (ADC_HandleTypeDef *hadc)
 	Regular conversion half DMA transfer callback in non blocking mode.
__weak void 	HAL_ADC_LevelOutOfWindowCallback (ADC_HandleTypeDef *hadc)
 	Analog watchdog callback in non blocking mode.
__weak void 	HAL_ADC_ErrorCallback (ADC_HandleTypeDef *hadc)
 	Error ADC callback.
