Examples
********

Matrix
======

Example usage with ESP8266::

    import is31fl3731
    from machine import I2C, Pin
    i2c = I2C(Pin(5), Pin(4))
    display = is31fl3731.Matrix(i2c)
    display.fill(127)


Charlie Wing
============

Example usage with the Feather HUZZAH ESP8266 board::

    import is31fl3731
    from machine import I2C, Pin
    i2c = I2C(Pin(5), Pin(4))
    display = is31fl3731.CharlieWing(i2c)
    display.fill(127)


Pico:ed
=======

Example usage with the ELECFREAKS Pico:ed::

    from machine import I2C
    import is31fl3731
    i2c = I2C(1)  # scl=19, sda=18
    display = is31fl3731.PicoEd(i2c)
    display.fill(127)
