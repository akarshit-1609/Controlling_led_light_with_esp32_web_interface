# ESP32 PlatformIO Project to control LED light

You can turn On/Off LED Light with web interface GUI support.

## Prerequisites

*   **PlatformIO:** Make sure you have PlatformIO installed. You can find installation instructions on the [PlatformIO website](https://platformio.org/).
*   **Git:** You need Git installed to clone the repository.

## Getting Started

1.  **Clone the repository:**

    Open your terminal or command prompt and use the following command to clone the project:

    ```bash
    git clone https://github.com/akarshit-1609/Controlling_led_light_with_esp32_web_interface.git
    ```

2.  **Open in PlatformIO:**

    Open the cloned project in your preferred IDE with the PlatformIO extension installed (e.g., VS Code).

3.  **Configure Variables:**

    Before uploading the code to your ESP32, you need to configure some variables, particularly the GPIO pin connected to your LED.

    *   **Locate the configuration:** Open the `src/main.cpp` file.
    *   **Find the variable:** Look for a line similar to this:

        ```c++
        const char* ssid = "Your_ssid"; // Replace with your custom ssid
        const char* password = "your_password"; // Replace with your password

        const int led = 2; // Replace with your LED GPIO pin
        ```

    *   **Replace the value:** Change the `2` to the actual GPIO pin number where your LED is connected on your ESP32 board. Refer to your ESP32 board's pinout diagram if you are unsure.

4.  **Build and Upload:**

    *   Connect your ESP32 board to your computer via USB.
    *   In PlatformIO, click the "Build" button to compile the project.
    *   Click the "Upload" button to upload the compiled code to your ESP32.

## Project Structure

*   `platformio.ini`: PlatformIO configuration file.
*   `src/main.cpp`: The main source code file containing the LED control logic.
*   `lib/`: (Optional) Directory for external libraries.


## Usage

Once the code is uploaded, connect any device with esp32 wifi by ssid and password given in the code after open the browser and type url http://192.168.0.1 and enter than the LED connected to the configured `LED_PIN` should be control by your device.

## Demo

https://github.com/user-attachments/assets/92e3ac94-d2eb-447d-8388-1a7aaf3db1da

[![Watch on YouTube](https://img.shields.io/badge/-Watch%20on%20YouTube-red?style=flat&logo=youtube&logoColor=white)](https://www.youtube.com/watch?v=oxVEiBCz5go?si=vBeSSYlmwBNJvuOp)



