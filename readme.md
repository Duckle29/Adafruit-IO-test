## Adafruit IO Secure ESP8266 with CertStore

This is a little example PIO project for the ESP8266, allowing it to securely connect to the
Adafruit IO MQTT servers over MQTTS, however instead of using a certificate fingerprint
which is prone to expiring (often within a few months) it uses a [certificate store](https://arduino-esp8266.readthedocs.io/en/latest/esp8266wifi/bearssl-client-secure-class.html#certificate-stores)

The code is a combination of the [BearSSL certStore example](https://github.com/esp8266/Arduino/blob/master/libraries/ESP8266WiFi/examples/BearSSL_CertStore/BearSSL_CertStore.ino)
and the [Adafruit secure esp8266 example](https://github.com/adafruit/Adafruit_MQTT_Library/tree/master/examples/adafruitio_secure_esp8266)

It's made to work with platformIO.  
The python script will have to be modified if used with Arduino (path to ar.exe needs to be updated)