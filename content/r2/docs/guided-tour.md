---
title: Guided Tour
type: docs
rev: r2
---

# Guided Tour

Let's have a quick look at the boards and what's on them. All three boards have the same components except the USB connectors.

{{< columns >}}
[![Serpente](/r2/tour_serpente.jpg)](/r2/tour_serpente.jpg)
<--->
[![Serpente Plug](/r2/tour_plug.jpg)](/r2/tour_plug.jpg)
<--->
[![Serpente Plug C](/r2/tour_plug_c.jpg)](/r2/tour_plug_c.jpg)
{{< /columns >}}

- **USB A, male or female USB Type-C Connector** - Three options to choose from, use the one that works best for you! USB is used for both data and power. The Type-C connectors supports only USB 2.0 signals and is hardwired to be a Sink only.
- **Reset Button** - Allows you to reset the board quickly and if you double press it, the board boots into the bootloader.
- **4MB Flash Storage** - All 4MB of the storage are available to you, you can store your CircuitPython files as well as logs, images and more! When connected to a PC, the flash storage shows up as a disk drive. 
- **ATSAMD21 Microcontroller** - Cortex-M0+ running at 48MHz, not the fastest thing around, but fast enough for prototyping and simple applications.
- **6 Flexible GPIOs** - All 6 GPIOs can be used as analog inputs, PWM outputs or regular digital IOs. You can also configure them to be SPI, I2C and/or UART. See [Pinout]({{< relref "/r2/docs/pinout.md" >}}) and [GPIO Configurations]({{< relref "/r2/docs/gpios.md" >}}) for more details.
- **3.3V LDO** - The LDO provides up to 250mA of current for you.
- **RGB LED** - Each color is user-controllable with a possibility to PWM the colors.
- **Optional External Power** - If you don't want to use the USB to power the board, connect an external source (max 6V) to the `VIN` pin and you're ready to go!
- **Mount holes** (female Type-C only) - We used the extra space to provide you with two mounting holes in case you want to make sure your Serpente stays in place.
- **Breadboardable** - The spacing of the headers allows you to use the boards with a breadboard, both as GPIO and power!
- **Castellated edges** - You can easily use the Serpente boards as CircuitPython modules.