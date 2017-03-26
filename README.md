# SushiBits One

ARM Cortex-M in Arduino form factor, and consumes very little power.

## Introduction & Goal

This is one of my "design challenges" to myself:

*   Arduino-compatible form factor,
*   Take an 48-pin STM32 microcontroller (since STM32F103CBT6 are that cheap,)
*   Bring all I/O pins out somewhere, be it the connectors, JTAG or USB,
*   No two pins can be shorted together,
*   Use only switch-mode power supply,
*   Two layer PCB only,
*   Single side load.

## Main components

*   STM32 microcontroller in LQFP-48 package. I have tested the following:
    *   STM32F072C8T6 (Cortex-M0 @48MHz)
    *   STM32F103CBT6 (Cortex-M3 @72MHz)
    *   STM32L151CCT6 (Cortex-M3 @32MHz, ULP)
    *   STM32F303CCT6 (Cortex-M4F @72MHz)
    *   STM32F373CCT6 (Cortex-M4F @72MHz)
*   WCH CH340B: USB to UART adapter.
*   TI TPS562200: VIN to 5V buck converter.
*   TI LM3671-3.3: 5V to 3.3V buck converter.

## License

This is [open source hardware](http://www.oshwa.org/), licensed under the
[3-clause BSD license](LICENSE.md).
