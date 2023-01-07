
# _ESP32+LVGL8+ILI9341+GT911 (based on IDF 5.0)_

This is the simplest example to start develop an application with a new LVGL features (chart as example) using lvgl_esp32_drivers (develop branch).

![](https://github.com/valentyn-zaitsev/esp32_lvgl8_ili9341_gt911/blob/master/img/LVGL_example.jpg)

## How to use example

To make the project compatible is needed to do several minor changes in **lvgl_esp32_drivers** submodule:

1) Add ```driver``` to CMakeLists.txt

![driver](https://github.com/valentyn-zaitsev/esp32_lvgl8_ili9341_gt911/blob/master/img/driver.png)

2) Comment the line ```.bit_num = LEDC_TIMER_10_BIT```, in lv_port/esp_lcd_backlight.c file

![backlight](https://github.com/valentyn-zaitsev/esp32_lvgl8_ili9341_gt911/blob/master/img/backlight_fix.png)

## Hardware setup

In the project is used ESP32-3248S035 board, but it's easy to change display or touch driver setting through menuconfig.


