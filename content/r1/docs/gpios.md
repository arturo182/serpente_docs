---
title: GPIO Configurations
type: docs
rev: r1
---

# GPIO Configurations

Thanks to the flexibility of the SAMD21 SERCOM peripheral, the Serpente boards give you access to multiple serial interfaces with just 6 GPIOs. See [Pinout]({{< relref "/r1/docs/pinout.md" >}}) for an overview of the pins.

Note that most of the interfaces are easily accessible using CircuitPython, altough some of them can't be used at the same time:
{{< highlight python >}}
import board, busio

spi = board.SPI()
i2c = board.I2C()
uart = board.UART()
uart2 = busio.UART(board.TX2, board.RX2)
{{< / highlight >}} 

Here's a list of some of the ways you can configure the GPIOs on your Serpente:

## SPI + 3 GPIOs
<img src="/r1/config-spi.png" style="width: 500px">

## I2C + 4 GPIOs
<img src="/r1/config-i2c.png" style="width: 500px">

## UART + 4 GPIOs
<img src="/r1/config-uart.png" style="width: 500px"><br>
or<br>
<img src="/r1/config-uart2.png" style="width: 500px"><br>

## 2x UART + 2 GPIOs
<img src="/r1/config-2xuart.png" style="width: 500px"><br>
**Note: Because of a quirk on CircuitPython's implementation, you need to initialize UART 2 before UART.**

## SPI + I2C + 1 GPIO
<img src="/r1/config-spi-i2c.png" style="width: 500px">

## SPI + UART + 1 GPIO
<img src="/r1/config-spi-uart.png" style="width: 500px">

## UART + I2C + 2 GPIOs
<img src="/r1/config-uart-i2c.png" style="width: 500px">

## 6 GPIOs
See [Pinout]({{< relref "/r1/docs/pinout.md" >}}).