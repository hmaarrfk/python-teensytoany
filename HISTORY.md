# History

## 0.0.30 (2023-04-03)

* Increase default timeout to 0.2 seconds from 0.1. This helps receive error
  messages from missed I2C communications.
* Return an error if no response is returned from a standard command indicating
  a timeout.

## 0.0.29 (2023-03-06)

* Try to avoid racy conditions in version reading
* Flush buffers upon startup to help with crash recovery.

## 0.0.28 (2023-03-04)

* Make the error message when no device is found more human friendly.

## 0.0.27 (2022-10-16)

* Use packaging instead of distutils for version identification

## 0.0.26 (2021-09-13)

* added function `spi_read_byte` enabling the user to read SPI register.

## 0.0.25 (2021-07-14)

* added function `analog_read` enabling the user to read analog signals.

## 0.0.24 (2021-06-03)

* added `i2c_read_payload and` `i2c_write_payload functions` which allows users to read and write a contiguous payload of bytes

## 0.0.23 (2021-02-13)

* Ensure compatibility with pyserial 3.X
* Power a ``start_poweroff`` parameter to ``TeensyPower`` to start the device
  in the on state.
* Added the ability to close and open the device without deleting the python
  object.

## 0.0.22 (2020-06-18)

* Added the ability to control a power switch that is connected to the
  nominally on port.

## 0.0.20 (2019-12-14)

* Added capabilities for SPI and Analog functions

## 0.0.16 (2019-11-30)

* `TeensyPower` destructor will not raise an error when the device had failed
   to open.

## 0.0.15 (2019-11-29)

* `TeensyPower` devices will automatically poweroff the output when
  closed.

## 0.0.14 (2019-11-29)

* Added the specialized `TeensyPower` driver.

## 0.0.13 (2019-11-20)

* Added a few more serial numbers to the `teensytoany.known_devices`

## 0.0.1 (2019-11-07)

* First release on PyPI.
