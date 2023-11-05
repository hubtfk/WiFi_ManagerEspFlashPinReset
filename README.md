# ESP8266 Wi-Fi Manager Example

This Arduino code provides an example of using the WiFiManager library with an ESP8266 microcontroller. WiFiManager simplifies the process of connecting your ESP8266 to a Wi-Fi network by providing a web-based configuration portal for Wi-Fi setup.

## Prerequisites

- Arduino IDE
- ESP8266 board
- [WiFiManager library](https://github.com/tzapu/WiFiManager)

## Setup

1. Install the required libraries:
   - [WiFiManager](https://github.com/tzapu/WiFiManager): This library simplifies Wi-Fi network configuration.

2. Connect a push button to pin D3 (GPIO0) on your ESP8266 board. This button is used to trigger a Wi-Fi reset.

3. Upload the code to your ESP8266 board using the Arduino IDE.

## Usage

1. When you power on your ESP8266, it will attempt to connect to a Wi-Fi network.

2. If the ESP8266 fails to connect to a network, it will create a Wi-Fi access point (AP) named "MyESP8266AP."

3. You can connect to this AP using a device (e.g., a smartphone or computer).

4. Open a web browser and go to the address "192.168.4.1."

5. You will be presented with a web-based configuration portal to select and connect to a Wi-Fi network.

6. Once you configure the Wi-Fi network settings, the ESP8266 will attempt to connect to the selected network.

7. If you ever need to reset the Wi-Fi settings, press the push button connected to pin D3 (GPIO0). This will reset the settings and create the AP again.

8. Your custom code can be added to the "Your code here" section to perform specific tasks once Wi-Fi is successfully configured.

## Troubleshooting

- If you encounter any issues, check the connections and ensure that you have installed the required libraries.

- Make sure that you have the ESP8266 board selected in the Arduino IDE.

- If you need to reset the Wi-Fi settings, press the push button on pin D3 (GPIO0) as described above.

That's it! You have set up an ESP8266 with WiFiManager to simplify Wi-Fi configuration for your project.
