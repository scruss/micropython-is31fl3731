Driver for IS31FL3731-based LED matrices
========================================

Original documentation at http://micropython-is31fl3731.readthedocs.io/

Trivially modified to add support for the 7x17 matrix built into the [url=https://www.elecfreaks.com/picoed.html]ELECFREAKS Pico:ed[/url]:

    from machine import I2C
    import is31fl3731
    
    i2c = I2C(1)  # scl=19, sda=18
    display = is31fl3731.PicoEd(i2c)
    display.fill(127)
