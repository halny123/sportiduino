#### Version 1.0.3
-------------

Данный репозиторий содержит информацию о моей модификации системы электронной отметки для ориентирования созданной Александром Воликовым.
https://github.com/alexandervolikov/sportiduino

Прошивка писалась на основе Mifare прошивок станций версии 1.4.0 - Александра Воликова.

[Все, что касается схемы, плат, изготовления находится здесь](https://github.com/halny123/sportiduino/tree/master/NRFstation)

Прошивка только для Mifare чипов т.к. в наличии только они пока.

[Базовая станция](https://github.com/halny123/sportiduino/tree/master/Base%20station/MifareBaseStation)

[Мастер станция](https://github.com/halny123/sportiduino/tree/master/Master%20station/MifareMasterStation)

Что добавленно в схему и на плату.
------------
 - Возможность установить SMD и\или выводной светодиод. Позволяет сделать разборную конструкцию станции.
 - Добавлен геркон.
   Служит для :
   - подачи питания на радиомодуль NRF24l01
   - входа в режим програмирования через радиомодуль
   - с помощью него станция оперативно выводится из **Sleep** режима
   - переводится в  **Sleep** режим после выхода из режима програмирования через радиомодуль. 
    
 - Добавленна возможность установки радиомодуля NRF24l01 как в выводном исполнении так и под монтаж на плату. Это позволяет програмировать станции без использования чипов.
     
Пока реализована только односторонняя связь.

     - Можно устанавливать время

     - Задавать настройку конфигурации/пароля

     - Усыплять станции

     - Задавать режим работы станции(Старт\Финиш\Полевая\Очистка\Проверка)

В дальнейшем планируется доделать двухстороннюю связь с передачей логов со станции.

 - Есть возможность установить внешнюю память 24*** если появится необходимость
 - Выведены с 3-х свободных пинов МК дорожки с контактными площадками, если понадобится в дальнейшем можно их использовать.

[Описание процесса изготовления](https://github.com/halny123/sportiduino/tree/master/NRFstation)
-------------

[Видео работы ](https://youtu.be/SSd08Qn7M1Y)
------------

[Перешел на метки NTAG215](https://github.com/halny123/sportiduino/tree/master/Chip)
-------------
Добавил 3D модели для печати чипов под метки 25мм NTAG215 и фото того что получилось.
Чип состоит из двух половинок в "верхнюю крышку" вклеиваю NTAG метку 25мм, предварительно приклеив ее на пластик 0,4мм толщиной. Далее склеиваю две половинки чипа. Добавляю ремешок и чип готов.

![Перешел на метки NTAG215](https://github.com/halny123/sportiduino/tree/master/Chip/NTAG-215/Image/Chip.png)

License:         GNU GPLv3
