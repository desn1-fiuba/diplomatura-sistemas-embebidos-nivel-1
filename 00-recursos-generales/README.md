# Recursos generales de la Diplomatura en Sistemas Embebidos - Nivel 1

Esta carpeta reúne documentación técnica común a las materias de la Diplomatura en Sistemas Embebidos - Nivel 1.

La documentación se organiza en torno a tres niveles:

1. La placa de desarrollo NUCLEO-F446RE.
2. El microcontrolador STM32F446RE.
3. El procesador ARM Cortex-M4.
4. El entorno de desarrollo, las herramientas STM32Cube y las bibliotecas HAL/LL.

Se recomienda consultar siempre los enlaces oficiales, ya que los fabricantes pueden actualizar los documentos técnicos con nuevas revisiones.

---

## Placa de desarrollo NUCLEO-F446RE

### Página oficial de la placa

- [NUCLEO-F446RE - Página oficial de STMicroelectronics](https://www.st.com/en/evaluation-tools/nucleo-f446re.html)

Página oficial de la placa de desarrollo NUCLEO-F446RE. Incluye descripción general, recursos de hardware, documentación, archivos de diseño y herramientas asociadas.

### Manual de usuario de la placa

- [UM1724 - STM32 Nucleo-64 boards User Manual](https://www.st.com/resource/en/user_manual/um1724-stm32-nucleo64-boards-mb1136-stmicroelectronics.pdf)

Manual de usuario de las placas STM32 Nucleo-64 basadas en la placa MB1136.  
Este documento resulta fundamental para identificar conectores Arduino, conectores ST Morpho, alimentación, ST-LINK, jumpers, solder bridges y distribución física de pines.

---

## Microcontrolador STM32F446RE

### Página oficial del microcontrolador

- [STM32F446RE - Página oficial de STMicroelectronics](https://www.st.com/en/microcontrollers-microprocessors/stm32f446re.html)

Página oficial del microcontrolador STM32F446RE. Incluye información general del dispositivo, documentación, modelos, herramientas y recursos asociados.

### Hoja de datos

- [DS10693 - STM32F446xC/E Datasheet](https://www.st.com/resource/en/datasheet/stm32f446mc.pdf)

Hoja de datos del microcontrolador STM32F446xC/E.  
Este documento permite consultar características generales, memoria, periféricos disponibles, encapsulado, pines, condiciones eléctricas y límites de operación.

> Nota: aunque el archivo se denomina `stm32f446mc.pdf`, el documento corresponde a la familia STM32F446xC/E e incluye al STM32F446RE utilizado en la NUCLEO-F446RE.

### Manual de referencia

- [RM0390 - STM32F446xx Reference Manual](https://www.st.com/resource/en/reference_manual/dm00135183-stm32f446xx-advanced-arm-based-32-bit-mcus-stmicroelectronics.pdf)

Manual de referencia del microcontrolador STM32F446xx.  
Es el documento principal para estudiar la arquitectura interna del microcontrolador y sus periféricos: RCC, GPIO, EXTI, USART, UART, SPI, I2C, timers, ADC, DMA, memorias y buses internos.

### Manual de programación STM32 Cortex-M4

- [PM0214 - STM32 Cortex-M4 MCUs and MPUs Programming Manual](https://www.st.com/resource/en/programming_manual/pm0214-stm32-cortexm4-mcus-and-mpus-programming-manual-stmicroelectronics.pdf)

Manual de programación para microcontroladores STM32 basados en ARM Cortex-M4.  
Describe el modelo de programación, registros del núcleo, excepciones, interrupciones, SysTick, NVIC y aspectos propios del procesador desde la perspectiva STM32.

---

## Procesador ARM Cortex-M4

### Página oficial del procesador

- [Arm Cortex-M4 - Página oficial de Arm](https://www.arm.com/products/silicon-ip-cpu/cortex-m/cortex-m4)

Página oficial del procesador ARM Cortex-M4.  
Sirve como referencia general sobre las características del núcleo utilizado por el STM32F446RE.

### Manual técnico del procesador

- [DDI0439B - Cortex-M4 Technical Reference Manual](https://developer.arm.com/documentation/ddi0439/b/)

Manual técnico del procesador ARM Cortex-M4.  
Describe la arquitectura del núcleo, el modelo de programación, las interfaces, el sistema de excepciones, el NVIC, la unidad de protección de memoria y los recursos de depuración.

---

## STM32Cube, HAL y LL

### Manual de drivers HAL y Low Layer

- [UM1725 - Description of STM32F4 HAL and Low-Layer Drivers](https://www.st.com/resource/en/user_manual/um1725-description-of-stm32f4-hal-and-lowlayer-drivers-stmicroelectronics.pdf)

Manual de usuario de los drivers HAL y LL para la familia STM32F4.  
Sirve como referencia para comprender las funciones generadas por STM32CubeIDE y utilizadas en los proyectos de firmware.

### STM32CubeIDE

- [STM32CubeIDE - Página oficial de STMicroelectronics](https://www.st.com/en/development-tools/stm32cubeide.html)

Entorno de desarrollo integrado utilizado en la diplomatura para crear, configurar, compilar, depurar y cargar proyectos en la placa NUCLEO-F446RE.

### STM32CubeMX

- [STM32CubeMX - Página oficial de STMicroelectronics](https://www.st.com/en/development-tools/stm32cubemx.html)

Herramienta gráfica de configuración de microcontroladores STM32.  
En STM32CubeIDE se encuentra integrada para configurar pines, periféricos, reloj del sistema, middleware y generación automática de código de inicialización.

### STM32CubeF4

- [STM32CubeF4 - Paquete oficial de firmware para STM32F4](https://www.st.com/en/embedded-software/stm32cubef4.html)

Paquete de firmware oficial para la familia STM32F4.  
Incluye drivers HAL, drivers LL, CMSIS, middleware y ejemplos de referencia para distintos periféricos.

---

## Recomendación de uso

Para las prácticas de la diplomatura se recomienda consultar los documentos en este orden:

1. **UM1724**, para ubicar conectores, pines, alimentación y ruteo físico de la placa.
2. **Datasheet STM32F446xC/E**, para revisar características eléctricas, encapsulado y pines.
3. **RM0390**, para estudiar los periféricos internos del microcontrolador.
4. **PM0214**, para comprender el núcleo Cortex-M4 desde la perspectiva STM32.
5. **DDI0439B**, para profundizar en la arquitectura del procesador ARM Cortex-M4.
6. **UM1725**, para interpretar las funciones HAL y LL utilizadas en los proyectos.

---

## Nota sobre almacenamiento de documentos

En este repositorio se priorizan enlaces oficiales de descarga en lugar de almacenar copias locales de los PDF.

Esto permite:

- acceder a la versión más actualizada de cada documento;
- reducir el tamaño del repositorio;
- evitar duplicar documentación técnica del fabricante;
- mantener trazabilidad hacia las fuentes oficiales.
