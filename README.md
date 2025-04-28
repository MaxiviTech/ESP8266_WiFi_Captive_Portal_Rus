# ESP8266 WiFi Captive Portal 2.0 Rus

## Дисклеймер
Этот проект создан для тестирования возможностей и в образовательных целях. Используйте его только против ваших сетей и устройств. Я не несу отвественности за ваши действия совершенные с помощью этой программы.

## О проекте 
WiFi Веб-страница авторизации для NodeMCU (ESP8266 Модуля) c DNS спуфингом. Она запрашивает у пользователя электронную почту и пароль для входа на поддельную страницу, для того чтобы "Получить доступ к интернету".

Встроенный светодиод будет мигать 5 раз когда учетные данные опубликованы.

<b>Внимание!</b> Ваши сохраненные учетные данные исчезнут когда вы перезапустите/отключите ESP8266.

<b>Заметка:</b> Если вы хотите увидеть хранимые учетные данные, перейдите на <a>"**http**://</a>yourcurrentwebsite.com<a>/creds</a>" или "**172.0.0.1**<a>/creds</a>".

# Скриншоты

<table>
  <tr>
    <th>172.0.0.1/index</th>
    <th>172.0.0.1/post</th> 
    <th>172.0.0.1/creds</th>
  </tr>
  <tr>
    <td><img src="https://raw.githubusercontent.com/125K/ESP8266_WiFi_Captive_Portal_2.0/master/src/1_index.png" title="Index"></td>
    <td><img src="https://raw.githubusercontent.com/BlueArduino20/ESP8266_WiFi_Captive_Portal_2.0/master/src/2_post.png" title="Post"></td>
    <td><img src="https://raw.githubusercontent.com/BlueArduino20/ESP8266_WiFi_Captive_Portal_2.0/master/src/3_creds.png" title="Creds"></td>
  </tr>
</table>

# Установка (ESP8266 Flasher - Простой способ)

1. Установите <a href="https://github.com/nodemcu/nodemcu-flasher"><b>ESP8266 Flasher</b></a>.

2. Загрузите файл <b><a href="https://github.com/125K/ESP8266_WiFi_Captive_Portal_2.0/releases/download/2.1/release.bin">release.bin</b></a>.

3. Откройте ESP8266 Flasher и выберите Node MCU порт.

<img width="80%" src="https://raw.githubusercontent.com/BlueArduino20/ESP8266_WiFi_Captive_Portal_2.0/master/src/1_port_selection.PNG">

4. Далее, войдите во вкладку config и выберите только что загруженный .bin файл.

<img width="80%" src="https://raw.githubusercontent.com/BlueArduino20/ESP8266_WiFi_Captive_Portal_2.0/master/src/2_file_selection.png">

5. Можете перейти обратно к первой вкладке и нажать "Flash".

6. Готово!

# Установка (Arduino IDE - Продвинутый способ)

1. Откройте ваш <a href="https://www.arduino.cc/en/main/software">Arduino IDE</a> и перейдите в "File -> Preferences -> Boards Manager URLs" и вставьте следующую ссылку:
``http://arduino.esp8266.com/stable/package_esp8266com_index.json``.
2. Перейдите в "Tools -> Board -> Boards Manager", найдите "esp8266" и установите.
3. Перейдите в "Tools -> Board" и выберите вашу плату.
4. Загрузите и откройте скетч "<a href="https://github.com/BlueArduino20/ESP8266_WiFi_Captive_Portal_2.0/blob/master/ESP8266_WiFi_Captive_Portal_2.0.ino"><b>ESP8266_WiFi_Captive_Portal_2.0.ino</b></a>".
5. При желании вы можете изменить некоторые параметры такие как SSID и элементы веб-страницы.
6. Загрузите ваш код на плату.
7. Всё готово!
