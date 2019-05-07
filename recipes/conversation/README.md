# Conversation
> Поговори с TJBot!

Этот рецепт использует [Watson Assistant](https://www.ibm.com/watson/services/conversation/), [Watson Speech to Text](https://www.ibm.com/watson/services/speech-to-text/), and [Watson Text to Speech](https://www.ibm.com/watson/services/text-to-speech/) сервисы для того чтобы превратить TJ в говорящего робота.

## Hardware
Требуется TJBot с микрофоном и колонками.

## Build and Run
Во-первых, убедитесь, что вы настроили Raspberry Pi для TJBot, выполнив [bootstrap instructions](https://github.com/ibmtjbot/tjbot/tree/master/bootstrap).

Далее перейдите к папке `recipes/conversation` и установите зависимости.

    $ cd tjbot/recipes/conversation
    $ npm install

Создайте экземляры сервисов [Watson Assistant](https://www.ibm.com/watson/services/conversation/), [Watson Speech to Text](https://www.ibm.com/watson/services/speech-to-text/), и [Watson Text to Speech](https://www.ibm.com/watson/services/text-to-speech/) и запишите учетные данные аутентификации.

Импортируйте файл `workspace-sample.json` в сервис Watson Assistant и запишите workspace ID.

Сделайте копию файла конфигурации по умолчанию и обновите его, используя свои учетные записи от сервиса Watson и workspace ID.

    $ cp config.default.js config.js
    $ nano config.js
    <enter your credentials and the conversation workspace ID in the specified places>

Запустите!

    sudo node conversation.js

> Используйте `sudo` команду. Требуются права доступа Root.

Watson conversation использует намерения, чтобы обозначить цель предложения. Например, когда вы спрашиваете TJBot «Пожалуйста, представьтесь», намерение(intent) - представление. Вы можете добавить свои собственные новые намерения, но сейчас мы создали для вас несколько намерений:

- Представление(Introduction). Вы можете сказать фразу такую как "Watson, please introduce yourself", "Watson, who are you", and "Watson, can you introduce yourself"
- Шутка(Joke). Вы можете спросить "Watson, please tell me a joke" or "Watson, I would like to hear a joke".

Для получения полного списка, посмотрите содержание  workspace-sample.json

 **Приветственное слово** используется для того, чтобы TJBot знал что вы говорите с ним. По умолчанию приветственное слово 'Watson', но вы его может поменять в файле config.js. Обновите файл конфигурации, чтобы изменить имя робота в разделе tjConfig:

    // set up TJBot's configuration
    
    exports.tjConfig = {
        log: {   level: 'verbose'    },
        robot: {   name: 'tee jay bot'  }
    };

Вы можете изменить 'имя' на любое, как вы хотели бы назвать своего TJBot.

# Watson Services
- [Watson Assistant](https://www.ibm.com/watson/services/conversation/)
- [Watson Text to Speech](https://www.ibm.com/watson/services/text-to-speech/)
- [Watson Speech to Text](https://www.ibm.com/watson/services/speech-to-text/)

# License
This project is licensed under Apache 2.0. Full license text is available in [LICENSE](../../LICENSE).

# Contributing
See [CONTRIBUTING.md](../../CONTRIBUTING.md).
