# Arduino CAN (ESP32 only)



An Arduino ESP32 library for sending and receiving data using CAN bus.

## Compatible Hardware
* [Espressif ESP32](http://espressif.com/en/products/hardware/esp32/overview)'s built-in [SJA1000](https://www.nxp.com/products/analog/interfaces/in-vehicle-network/can-transceiver-and-controllers/stand-alone-can-controller:SJA1000T) compatible CAN controller with an external 3.3V CAN transceiver

### Espressif ESP32 wiring

Requires an external 3.3V CAN transceiver, such as a [TI SN65HVD230](http://www.ti.com/product/SN65HVD230).

| CAN transceiver | ESP32 |
| :-------------: | :---: |
| 3V3 | 3V3 |
| GND | GND |
| CTX | GPIO_5 |
| CRX | GPIO_4 |

`CTX` and `CRX` pins can be changed by using `CAN.setPins(rx, tx)`.

## Installation

### Using the Arduino IDE Library Manager

1. Choose `Sketch` -> `Include Library` -> `Manage Libraries...`
2. Type `CAN` into the search box.
3. Click the row to select the library.
4. Click the `Install` button to install the library.

### Using Git

```sh
cd ~/Documents/Arduino/libraries/
git clone https://github.com/sandeepmistry/arduino-CAN CAN
```

## API

See [API.md](API.md).

## Examples

See [examples](examples) folder.


## License

This library is [licensed](LICENSE) under the [MIT Licence](http://en.wikipedia.org/wiki/MIT_License).
