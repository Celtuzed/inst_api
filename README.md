# Космический Телеграм

Этот код нужен для скачивания картинок с NASA и SpaceX, а также благодаря коду можно выложить картинки в телеграм.

### Как установить
Перед использованием бота в своём телеграм канале, нужно ознакомиться с данной документацией `https://smmplanner.com/blog/otlozhennyj-posting-v-telegram/`
Для того чтобы использовать скрипт с выкладыванием фото в телеграм нужно будет положить в `.env` файл токен бота
```
  TG_BOT_API_KEY=Ваш_токен
```


Python3 должен быть уже установлен.
Затем используйте `pip` (или `pip3`, есть конфликт с Python2) для установки зависимостей:
```
  pip install -r requirements.txt
```

### Использование

Для запуска скрипта нужно ввести один из аргуметнов: `-sx/--SpaceX`; `-ena/--EPIC_NASA`;
`-ana/--APOD_NASA`; `-tg`/`--Telegram`

```
  main.py -sx/--SpaceX
```
Скачивает последние фото из каталогов SpaceX.
```
  main.py -ena/--EPIC_NASA
```
Скачивает фотографии нашей планеты за последний день(может быть раньше).
```
  main.py -ana/--APOD_`
```
Скачивает фотографии дня за последние 30 дней из NASA.
```
  main.py -tg/--Telegram
```
Постит картинки из папки `images` в телеграм канал.
### Цель проекта

Код написан в образовательных целях на онлайн-курсе для веб-разработчиков [dvmn.org](https://dvmn.org/).
