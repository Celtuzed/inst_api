# Космический Инстаграм

Этот код нужен для скачивания картинок с Hubble и SpaceX, а также благодаря коду можно выложить картинки в инсту.

### Как установить

Для того чтобы использовать скрипт с выкладыванием фото в инстаграм нужно будет положить в `.env` файл пароль
```
INSTAGAM_PASSWORD=Ваш_пароль
```
и логин  
```
INSTAGAM_USERNAME=Ваш_логин
```

Python3 должен быть уже установлен.
Затем используйте `pip` (или `pip3`, есть конфликт с Python2) для установки зависимостей:
```
  pip install -r requirements.txt
```

### Использование

Для запуска скрипта нужно ввести один из аргуметнов: `-sx/--SpaceX`; `-hi/--Hubble_id`;
`-hc/--Hubble_collection`; `-ip`/`--Instagram_post`

```
main.py -sx/--SpaceX
```
Скачивает последние фото из каталогов SpaceX.
```
main.py -hi/--Hubble_id Id_картинки
```
Скачивает картинку по id с сервиса Hubble.
```
main.py -hc/--Hubble_collection Название коллекции
```
Скачивает сразу коллекцию картинок с сервиса Hubble.
```
main.py -ip/--Instagram_post
```
Постит картинки из папки `images` в инстаграм.
### Цель проекта

Код написан в образовательных целях на онлайн-курсе для веб-разработчиков [dvmn.org](https://dvmn.org/).
