# IBM TJBot
<img src="images/tjbot.jpg" width="85%">

[IBM Watson Maker Kits](http://ibm.biz/mytjbot) are a collection of DIY open source templates to build things with [Watson](https://www.ibm.com/watson/products-services/) in a fun and easy way. [IBM TJBot](http://ibm.biz/mytjbot) is the first maker kit in the collection. You can 3D print or laser cut the robot body, then use one of our [recipes](recipes) to bring him to life!

In addition, you can unleash your own creativity and create new recipes that bring TJBot to life using any of the available [Watson services](https://www.ibm.com/watson/products-services/)!

**TJBot only works with a Raspberry Pi.**

# Build TJBot
You can make your own TJBot in a number of ways.

- **3d Print or Laser Cut**. If you have access to a 3D printer or laser cutter, you can print/cut TJBot yourself. Begin by downloading the [design files](https://ibmtjbot.github.io/#gettj) and firing up your printer/cutter.
- **TJBot Full Kit**. You can order a full TJBot kit with the laser cut cardboard and all the electronics from [Sparkfun](https://www.sparkfun.com/products/14123), [Adafruit](https://www.adafruit.com/product/3462), or [Robotkingdom](http://shop.robotkingdom.com.tw/raspberry-pi/tjbot01.html).
- **TJBot Cardboard Kit**. You can purchase the TJBot laser cut cardboard from [Texas Laser Creations](http://texlaser.com).

## Electronics
There are a number of components you can add to TJBot to bring him to life. Not all of these are required for all recipes.

- [Raspberry Pi 3 + SD card preloaded with NOOBS](http://www.mcmelectronics.com/product/RASPBERRY-PI-RPI-MODB-16GB-NOOBS-/83-17304). **This is a required component to make TJBot work!** 🤖
- [NeoPixel RGB LED (8mm)](https://www.adafruit.com/product/1734). Note that if you are using other kinds of LEDs, you may need to add a resistor; this LED doesn’t require one.
- [Female-to-female jumper wires](https://www.amazon.com/dp/B00KOL5BCC/). TJBot will only need 3 of these wires, so you’ll have extra.
- [Female-to-male jumper wires](https://www.amazon.com/dp/B00PBZMN7C/). TJBot will only need 3 of these wires, so you’ll have extra.
- [USB Microphone](https://www.amazon.com/gp/product/B00IR8R7WQ/). Other brands of USB microphones should also work.
- Mini Bluetooth Speaker. Any small speaker with either a 3.5mm audio jack or Bluetooth will work. Note that if you are using the 3.5mm audio jack, you may wish to add a [USB Audio Adapter](https://www.adafruit.com/product/1475) to avoid audio interference with the LED.
- [Servo Motor](https://www.amazon.com/RioRand-micro-Helicopter-Airplane-Controls/dp/B00JJZXRR0/). Note that the red (middle) wire is 5v, the brown wire is ground, and the orange wire is data.
- [Raspberry Pi Camera](https://www.amazon.com/dp/B01ER2SKFS/). Either the 5MP or 8MP camera will work.

## Сборка
Once you have obtained your TJBot, please refer to [the assembly instructions](http://www.instructables.com/id/Build-TJ-Bot-Out-of-Cardboard/) to put it all together.

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

[Recipes](recipes) это пошаговые инструкции, чтобы оживить ваш TJBot с помощью [Watson](https://www.ibm.com/watson/products-services/).

Мы подготовили 3 рецепта для вас [recipes](recipes) для вас:

- Используйте свой голос, чтобы управлять светом с помощью Watson[[instructions](http://www.instructables.com/id/Use-Your-Voice-to-Control-a-Light-With-Watson/)] [[github](https://github.com/ibmtjbot/tjbot/tree/master/recipes/speech_to_text)]
- Сделайте так, чтобы ваш робот реагировал на эмоции с помощью Watson [[instructions](http://www.instructables.com/id/Make-Your-Robot-Respond-to-Emotions-Using-Watson/)] [[github](https://github.com/ibmtjbot/tjbot/tree/master/recipes/sentiment_analysis)]
- Создайте говорящего робота с Watson [[instructions](http://www.instructables.com/id/Build-a-Talking-Robot-With-Watson-and-Raspberry-Pi/)] [[github](https://github.com/ibmtjbot/tjbot/tree/master/recipes/conversation)]
После ознакомления с нашими примерами рецептов, мы рекомендуем вам взглянуть на [популярные рецепты] (featured) созданный членами нашего сообщества.

# Contribute to TJBot
TJBot - это проект с открытым исходным кодом, разработанный для того, чтобы с ним было весело и легко взаимодействовать с помощью [Watson](https://www.ibm.com/watson/products-services/). Мы будем рады видеть, что вы можете сделать с ним!

Если вы хотите, чтобы ваш собственный рецепт был включен в наш список [featured recipe](featured), пожалуйста откройте issue [open an issue](../../issues) с ссылкой на ваш репозиторий и демо видео.

# About TJBot
[TJBot](http://ibm.biz/mytjbot) был назван в честь Thomas J. Watson, первого председателя и генерального директора IBM. TJBot был создан [Maryam Ashoori](https://github.com/maryamashoori) в подразделении IBM Research в качестве эксперимента, чтобы найти лучшие практики в разработке и реализации когнитивных объектов. Он родился 9 ноября 2016 года через [этот блог post](https://www.ibm.com/blogs/research/2016/11/calling-makers-meet-tj-bot/).

# License
This project uses the [Apache License Version 2.0](LICENSE) software license.
