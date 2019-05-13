# IBM TJBot
<img src="images/tjbot.jpg" width="85%">

[IBM Watson Maker Kits](http://ibm.biz/mytjbot) - это коллекция из DIY open source шаблонов для создания различных устройств с помощью [Watson](https://www.ibm.com/watson/products-services/) в веселой и простой форме. [IBM TJBot](http://ibm.biz/mytjbot) это первый комплект в этой коллекции. Вы можете сделать 3D печать тела робота, а затем использовать один из наших [рецептов](recipes) чтобы оживить его!

Кроме того, вы можете раскрыть свой творческий потенциал и создать новые рецепты, которые оживят TJBot, используя любой из доступных сервисов [Watson](https://www.ibm.com/watson/products-services/)!

**TJBot работает только на Raspberry Pi.**

# Build TJBot
Вы можете создать свой собственный TJBot несколькими способами.

- **3d печать или лазерная резка**. Если у вас есть доступ к принтеру 3D или лазерной резке, то вы можете напечатать TJBot самостоятельно. Начните с скачивания [файлов дизайна](https://ibmtjbot.github.io/#gettj) и загружайте в ваш принтер/резак.
- **TJBot Full Kit**. Вы можете заказать полный комплект TJBot с картоном для лазерной резки и всей электроникой от [Sparkfun](https://www.sparkfun.com/products/14123), [Adafruit](https://www.adafruit.com/product/3462), или [Robotkingdom](http://shop.robotkingdom.com.tw/raspberry-pi/tjbot01.html).
- **TJBot Cardboard Kit**. Вы можете купить нарезанный лазером картон робота TJBot в [Texas Laser Creations](http://texlaser.com).

## Электроника
Есть ряд компонентов, которые вы можете добавить в TJBot, чтобы его оживить. Не все из них требуются для всех рецептов.

- [Raspberry Pi 3 + SD card preloaded with NOOBS](http://www.mcmelectronics.com/product/RASPBERRY-PI-RPI-MODB-16GB-NOOBS-/83-17304). **Это обязательный компонент для работы TJBot!** 🤖
- [NeoPixel RGB LED (8mm)](https://www.adafruit.com/product/1734). Обратите внимание, что если вы используете другие виды светодиодов, вам может потребоваться добавить резистор; в этот светодиод резистор не требуется.
- [Female-to-female jumper wires](https://www.amazon.com/dp/B00KOL5BCC/). TJBot понадобится только 3 из этих проводов.
- [Female-to-male jumper wires](https://www.amazon.com/dp/B00PBZMN7C/). TJBot понадобится только 3 из этих проводов.
- [USB Microphone](https://www.amazon.com/gp/product/B00IR8R7WQ/). Другие марки USB микрофонов также должны работать.
- Mini Bluetooth Speaker. Подойдет любой маленький динамик с 3,5-мм аудиоразъемом или Bluetooth. Обратите внимание, что если вы используете 3,5-мм аудиоразъем, то возможно вам надо будет добавить [USB Audio Adapter](https://www.adafruit.com/product/1475) чтобы избежать звуковых помех со светодиодом LED.
- [Servo Motor](https://www.amazon.com/RioRand-micro-Helicopter-Airplane-Controls/dp/B00JJZXRR0/). Обратите внимание, что красный (средний) провод имеет напряжение 5 В, коричневый провод заземлен, а оранжевый - данные.
- [Raspberry Pi Camera](https://www.amazon.com/dp/B01ER2SKFS/). Будет работать 5-мегапиксельная или 8-мегапиксельная камера.

## Сборка
Как только вы получили свой TJBot, пожалуйста следуйте видео инструкциям по сборке тела робота [the assembly instructions](http://www.instructables.com/id/Build-TJ-Bot-Out-of-Cardboard/).

Для справки, вот схема подключения светодиодов и сервомотора к вашему Raspberry Pi.

![](images/wiring.png)

> 💡 Будьте осторожны при подключении светодиода! Если он подключен неправильно, то может сгореть. Светодиод имеет плоскую выемку на одной стороне(на картинке она справа); используйте это, чтобы сориентировать светодиод и выяснить, где какой вывод.

> Для сервопривода обратите внимание, что красный (средний) провод имеет напряжение 5 В, коричневый провод заземлен, а оранжевый - данные.

# Как оживить TJBot
Сначала убедитесь, что вы правильно настроили Raspberry Pi для TJBot.
Просто запустите эту команду, чтобы загрузить и установить TJBot:

```
curl -sL http://ibm.biz/tjbot-bootstrap | sudo sh -
```

[Рецепты](recipes) это пошаговые инструкции, чтобы оживить ваш TJBot с помощью [Watson](https://www.ibm.com/watson/products-services/).

Мы подготовили для вас 3 [рецепта](recipes):

- Создайте говорящего робота с Watson [[instructions](http://www.instructables.com/id/Build-a-Talking-Robot-With-Watson-and-Raspberry-Pi/)] [[github](https://github.com/betamaniac/tjbot/tree/master/recipes/conversation)]

- Используйте свой голос, чтобы управлять светом с помощью Watson[[instructions](http://www.instructables.com/id/Use-Your-Voice-to-Control-a-Light-With-Watson/)] [[github](https://github.com/ibmtjbot/tjbot/tree/master/recipes/speech_to_text)]
(На английском языке)
- Сделайте так, чтобы ваш робот реагировал на эмоции с помощью Watson [[instructions](http://www.instructables.com/id/Make-Your-Robot-Respond-to-Emotions-Using-Watson/)] [[github](https://github.com/ibmtjbot/tjbot/tree/master/recipes/sentiment_analysis)]
(На английском языке)


# Внесите свой вклад в проект TJBot
TJBot - это проект с открытым исходным кодом, разработанный для того, чтобы с ним было весело и легко взаимодействовать с помощью [Watson](https://www.ibm.com/watson/products-services/). Мы будем рады видеть, что вы можете сделать с ним!

Если вы хотите, чтобы ваш собственный рецепт был включен в наш список [рецептов](featured), пожалуйста откройте issue [open an issue](../../issues) с ссылкой на ваш репозиторий и демо видео.

# Подробнее о TJBot
[TJBot](http://ibm.biz/mytjbot) был назван в честь Thomas J. Watson, первого председателя и генерального директора IBM. TJBot был создан [Maryam Ashoori](https://github.com/maryamashoori) в подразделении IBM Research в качестве эксперимента, чтобы найти лучшие практики в разработке и реализации когнитивных объектов. Он родился 9 ноября 2016 года через [этот блог](https://www.ibm.com/blogs/research/2016/11/calling-makers-meet-tj-bot/).

# Лицензия
Этот проект использует [Apache License Version 2.0](LICENSE).
