# cc112x-driver
TI cc112x spi driver (Well formed code from TI examples)

### How to use

1. Add `#include "cc112x_spi.h"` in your code

2. Implement extern functions of spi interface in your code

```
extern void cc112x_spi_select_chip(void);
extern void cc112x_spi_deselect_chip(void);
extern uint32_t cc112x_spi_write(const uint8_t * buf, const uint32_t len);
extern uint32_t cc112x_spi_read(const uint8_t * buf, const uint32_t len);
extern uint8_t cc112x_spi_write_read_byte(const uint8_t wbyte);
extern void cc112x_debug(const rf_debug_t debug, const uint8_t data, const rf_status_t status); /* if debug is needed */

```
