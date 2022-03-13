# MicroPython on STM32F4 Discovery

## Main Resources

- Full tutorial: [STM32 Micropython](https://www.youtube.com/watch?v=a_G3WqjfPBA)
- [Download the latest MicroPython firmware for STM32F4-Discovery](https://micropython.org/download/STM32F4DISC/)
- [STM32F4-Discovery pins definition for MicroPython](https://github.com/micropython/micropython/blob/master/ports/stm32/boards/STM32F4DISC/pins.csv)

## Blinky Application

```python
import pyb

# Define the pins to be used
greenLed = pyb.Pin('LED_GREEN', pyb.Pin.OUT_PP)
redLed = pyb.Pin('LED_RED', pyb.Pin.OUT_PP)
blueLed = pyb.Pin('LED_BLUE', pyb.Pin.OUT_PP)
orangeLed = pyb.Pin('LED_ORANGE', pyb.Pin.OUT_PP)

while true:
    
    # Turn on Green LED
    greenLed.value(1)
    pyb.delay(1000)
    # Turn off Green LED
    greenLed.value(0)
    pyb.delay(1000)
```

## Other References

- [STM32F4DISCOVERY Setting GPIOs and Modules](https://forum.micropython.org/viewtopic.php?t=832)
- [MicroPython and STM32F407 Discovery Board](http://comedicles.com/chapters/micropython-esp8266-stm-arm/micropython-and-stm32f407-discovery-board/)

