# BM32S2031-1
Espressif Driver for Holtek's BM32S2031-1


## Modes of function

The BM32S2031-1 has two function modes, called `IO` and `UART`. 

### IO Mode

The Io mode is the simplest one. The two pins are working as an "input" `IN` and an "output" `OUT` pin. After 0.5s from the reset there are two options:

* `IN` is high: standar operation,the `OUT` pin is if the object is detected and low if it is not.  
* `IN` is low: leraning operation,the `OUT` pin goes from low to high when the distance is calibrated.

### UART Mode

The module waits for commands starting with `0x55` from the UART.  

