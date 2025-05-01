## (yet another) pico at arduino form factor board thingy

Wishlist: 
- power socket with 5V regulator (Vsys) also linked to Vin (shield compatibility)
- jumper switches (solder bridges on PCB bottom) for power selection: 5V or 3.3V
- multiplexer for 6 analog inputs (74HC4053?)

comments on first edition: 

Aangepaste schema/PCB layout voor een Raspberry Pico in Arduino jasje.

Uno compatible pinnen voor de Pico is niet gestandaardiseerd. Dus pinning overgenomen van FlexyPin versie: https://shop.pimoroni.com/products/raspberry-pi-pico-to-uno-flexypin-adapter?variant=40387747414099

A4-A6 zijn toegevoegd middels 74HC4053 mux en geschakeld met GPIO22. Hierdoor ontbreekt SCL/SDA helaas wel op A5/A6.

Verdere poorten:
SPI0 is op D10-D13 (losse 6-pin).
SPI1 zit op D16-D19.
I2C0 zit op D20/D21.
I2C1 zit o.a. op D2/D3.
UART0 zit op D0/D1.

