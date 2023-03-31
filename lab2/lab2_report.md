##### Цель работы: 
Изучить построение сети IP-телефонии с помощью маршрутизатора Cisco 2811, коммутатора Cisco catalyst 3560 и IP телефонов Cisco 7960.


В первую очередь создаётся заданная схема и настривается CMERouter (Рис. 1)
![image](https://user-images.githubusercontent.com/64036217/226312578-4fafa35a-f885-43b1-aa00-8adb99a97dfa.png)

Рисунок 1 - первоначальная схема и настройка роутера

После этого нужно настроить DHCP сервер для передачи голоса и данных на уже готовый роутер (Рис. 2).
![image](https://user-images.githubusercontent.com/64036217/226312909-132b8ca2-ef1c-49fd-a496-d835b4cc2391.png)


Рисунок 2 - настройка DHCP

Далее настраивается Cisco CallManager Express на CMERouter (Рис. 3).
![image](https://user-images.githubusercontent.com/64036217/226313005-43863af3-d560-408f-bbb6-fb9511adb885.png)


Рисунок 3 - настройка Cisco CallManager Express

После этого нужно задать нужные настройки коммутаторам, чтобы они работали через vlan (Рис. 4).
![image](https://user-images.githubusercontent.com/64036217/226314379-599e663f-f99c-483d-8c96-1015748be6ec.png)

Рисунок 4 - настройка vlan

Далее настраиваются номера телефонов и проверяется, корректно ли они подключены между собой (Рис. 5)
![image](https://user-images.githubusercontent.com/64036217/226314665-fb6f7aab-3c72-4a26-9bd8-912046532ccc.png)
![image](https://user-images.githubusercontent.com/64036217/226314685-c0aa88ae-bcb6-4368-8874-a5bd667d4d66.png)

Рисунок 5 - настройка телефонов

Следовательно, всё работает корректно.


Далее создаётся следующая схема (Рис. 6)
![image](https://user-images.githubusercontent.com/64036217/226314875-264a4dcf-d2ba-4a3f-b5a3-112fd1babf49.png)


Рисунок 6 - схема устройств

После этого настраивается коммутатор с работой через vlan (Рис. 7)
![image](https://user-images.githubusercontent.com/64036217/226315010-c24da433-cb69-4a9c-85d8-a70529757beb.png)


Рисунок 7 - настройка vlan


Даллее настроен vlan 99 (риснок 8).
![image](https://user-images.githubusercontent.com/64036217/229092571-4a227940-c826-4149-987f-3183ca32fad9.png)


Рисунок 8 - настройка работы vlan 99

А также 10 и 20 (рисунок 9).
![image](https://user-images.githubusercontent.com/64036217/229092654-219f5d1e-5f7e-46bb-96be-3411277fd4ae.png)

Рисунок 9 - настройка vlan 10 и 20

При этом vlan 99 смотрит в сторону роутера, а vlan 10 и 20 смотрят в сторону конечных устройств

На CMERouter созданы логические подынтерфейсы для vlan 10, vlan 20 и vlan 99 (рисунок 10).
![image](https://user-images.githubusercontent.com/64036217/229092791-6d0639e9-3919-4812-862c-6dc9b9c10834.png)


Рисунок 10 - настройка подынтерфейсов

На CMERouter также прописаны настройки DHCP сервера (рисунок 11).
![image](https://user-images.githubusercontent.com/64036217/229092889-5f5c32dd-c014-4b72-a295-fbc4fa0920cd.png)


Рисунок 11 - настройка DHCP

Далее на роутере настраивается телефонный сервис и номера телефонов (рисунок 12).

![image](https://user-images.githubusercontent.com/64036217/229093115-2758a7e7-c8e6-4eff-a361-d4de4a1b9228.png)

Рисунок 12 - настройка телефонного сервиса


Вывод: Изучено построение сети IP-телефонии с помощью маршрутизаторов Cisco 2811, коммутатора Cisco catalyst 3560 и IP телефонов Cisco 7960, настроено два вида различных сетевых топологий
