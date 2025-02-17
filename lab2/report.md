University: [ITMO University](https://itmo.ru/ru/)

Faculty: [FICT](https://fict.itmo.ru)

Course: [IP-telephony](https://github.com/itmo-ict-faculty/ip-telephony)

Year: 2024/2025

Group: K34202

Author: Gusevskaya Arina Eduardovna

Lab: Lab2

Date of create: 16.02.2025

Date of finished: 16.02.2025

# Лабораторная работа №2 "Конфигурация voip в среде Сisco packet tracer"

<b>Цель работы:</b> Изучить построение сети IP-телефонии с помощью маршрутизатора Cisco 2811, коммутатора Cisco catalyst 3560 и IP телефонов Cisco 7960.

## Ход выполнения работы 

### Часть 1

1. Соберем схему сети.

<img src="img/sc.png" width="500">

2. Отключим синтаксис ввода слов от DNS серверов.

<img src="img/dns.png" width="500">

3. Зададим пароли для защиты маршрутизатора как в удаленном режиме, так и в режиме консоли. Как это сделать, написано в [статье](https://ciscotips.ru/passwords).

<img src="img/password.jpg" width="500">

4. Настроим интерфейс fa0/0 на маршрутизаторе.

<img src="img/int.png" width="500">

5. Аналогично лаб 1 настроим dhcp сервер для передачи голоса и данных. Дополнительно пропишем option 150, чтобы автоматически подтягивать настройки для телефонов с TFTP сервера.

<img src="img/dhcp.png" width="500">

6. Настроим Cisco CallManager Express на маршрутизаторе.

<img src="img/ex.png" width="500">

7. На коммутаторе назначим для vlan 1 диапазоны портов и раздадим телефонам собственные номера.

<img src="img/number.png" width="500">

8. Убедимся, что телефоны включены и проверим связность.

Звонок с первого на второй телефон.

<img src="img/12.png" width="500">

Звонок с первого на третий телефон.

<img src="img/13.png" width="500">

Звонок с третьего на второй телефон.

<img src="img/32.png" width="500">

### Часть 2

1. Соберем схему сети, заданную по условию.

<img src="img/sc1.png" width="500">

2. Создадим vlan порты на коммутаторе для взаимодействия коммутатора с маршрутизатором.

<img src="img/vlan.png" width="500">

3. Укажем дефолтный маршрут.

<img src="img/def.png" width="500">

4. Выполненим настройку портов.

<img src="img/fa24.png" width="500">

5. Настроим DHCP-сервер для передачи голоса и данных.

<img src="img/dhcp1.png" width="500">

6. Настроим услуги телефони.

<img src="img/usl.png" width="500">

7. Выдадим телефонам собственные номера.

<img src="img/num.png" width="500">

8. На компьютерах включим режим DHCP для выдачи IP-адреса.

<img src="img/com.png" width="500">

9. Адреса были автоматически выданы телефонам.

<img src="img/red.png" width="500">

10. Проверим связность телефонов.

Звонок с первого на второй телефон

<img src="img/t12.png" width="500">

Звонок со второго на третий телефон

<img src="img/t23.png" width="500">

11. Проверим связность компьютеров.

<img src="img/p12.png" width="500">

<img src="img/p13.png" width="500">

<b>Вывод:</b> В ходе выполнения данной лабораторной работы было изучено построение сети IP-телефонии с помощью маршрутизатора Cisco 2811, коммутатора Cisco catalyst 3560 и IP телефонов Cisco 7960.
