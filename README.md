# Работа с Github
Для работы с github, у вас должно быть:
- установлен git на компьютер
- аккаунт на https://github.com/

# 1. Создание репозитория
![Иллюстрация к проекту](https://4.downloader.disk.yandex.ru/disk/3ea556ed4f45badae25132c9fbcb5ba037239effc9a8981ed12664ca6d4fa50e/59ef9b56/ePBJmrC14u0gjjVo9JgMX6f3qomrUE1eeBrCnI3eYI5UKwg-Zu2V06KSVEJkyoaKCWpYvWzZxRPje2H6X1Uaxw%3D%3D?uid=0&filename=2017-10-24_18-56-28.png&disposition=inline&hash=&limit=0&content_type=image%2Fpng&fsize=36166&hid=0e28fabd5b2206fd782279ae086edd77&media_type=image&tknv=v2&etag=73cc7addcd678a72209a903bd7d35e24)

В правой части header'а, нажимаем на "+", в выпадающем блоке выбираем New repository 

Вводим названием своего репозитория(проекта), и нажимаем на кнопку "Create repository" 
![Иллюстрация к проекту](https://4.downloader.disk.yandex.ru/disk/8f4f53fbe95c1069079c55a9aa5f0d2c4285008050e8ac1680215d0435319be9/59ef9c85/ePBJmrC14u0gjjVo9JgMX6Ep99vK-ktBjNnG0UJ_GXdXcCtC-_o6lgWABHytxUdJoz6jIrQw9DsfJJp_ildjXg%3D%3D?uid=0&filename=2017-10-24_19-02-22.png&disposition=inline&hash=&limit=0&content_type=image%2Fpng&fsize=33926&hid=681dcb4fc60db5af7a30d9a4164234ab&media_type=image&tknv=v2&etag=71e4259b9a2455db5d5ef6fa0802a9ba)

Открываем терминал(консоль) в папке с Вашим проектом, в моем случае это терминал в WebStorm, и вводим команду
```sh
$ git init
```
### 1.1 Сохранение изменений
Эта команда проинициализирует git в Вашем проекте.
Чтобы записать изменения в репозиторий, необходимо ввести 2 команды
```sh
$ git add .
```
И записанным измененями добавить соответствующий коммит
```sh
$ git commit -m "Текст коммита"
```
### 1.2 Отправка изменений на Github
Чтобы отправить изменения на удаленный репозиторий(github), нужно добавить адрес удаленного репозитория (делается 1 раз)
```sh
$ git remote add origin https://github.com/USERNAME/PROJECT_NAME.git
```
И отправить изменения, командой
```sh
$ git push -u origin master
```

Обратите внимание, что github помогает Вам тем, что показывает "стартовые" команды, с адресом вашего репозитория 
![Иллюстрация к проекту](https://2.downloader.disk.yandex.ru/disk/c2c0f53a225100ef77899b16783214d131e4be33bff2e4b470d86ff1c1919e31/59ef9f3f/ePBJmrC14u0gjjVo9JgMXwVy9sPPMQbLRaVfv4MfjNnftjirX6IkRNMWO3RVrkrXIYNhvL1klLEyN_7BKdqW8Q%3D%3D?uid=0&filename=2017-10-24_19-12-56.png&disposition=inline&hash=&limit=0&content_type=image%2Fpng&fsize=24673&hid=2fda01c1f9a7208a5bfbfa81e9b3d3a6&media_type=image&tknv=v2&etag=103bef7745438000a8552e26b6a75cd2)

# 2. Выполнение домашних заданий
Для каждого домашнего задания, необходимо создавать отдельную ветку, в соответствии с ТЗ на учебную неделю. Тоесть, для ТЗ1 ветка week_1, для ТЗ2 ветка week_2 и т.д.
Для того , чтобы создать новую ветку , и переключится на нее:
```sh
$ git checkout -b week_1
```
Выполняете ТЗ, и сохраняете изменения ( п. 1.2 этой инструкции )

# 3. Проверка работы
![Иллюстрация к проекту](https://1.downloader.disk.yandex.ru/disk/a7242c10413a86b1de7f18e9d6eaa50cf5854638e43843692be5cae8331b35e5/59efa515/ePBJmrC14u0gjjVo9JgMX-owpO_fBWIAplNwYfy8vgvNDWiGtc_mzQ242G_W81FBzL9iWEmnA2ledZwo7zRjcg%3D%3D?uid=0&filename=2017-10-24_19-39-01.png&disposition=inline&hash=&limit=0&content_type=image%2Fpng&fsize=21365&hid=dd3e2fd904b6841b8e56d5fa9bbd97dd&media_type=image&tknv=v2&etag=8a718992619a1ffe9bb418e226d34eac)
Создаем новую ветку gh-pages 
Заходим в настройки репозитория

- Переходим на вкладку settings
- Выбираем ветку gh-pages. Нажимаем save
- Копируем получившуюся ссылку

![Иллюстрация к проекту](https://1.downloader.disk.yandex.ru/disk/e10dddd576cd8516fda5d18680e05497fea9109afb00f89f2e26e48a330147f6/59efa574/ePBJmrC14u0gjjVo9JgMX_HbdUCX27jIykUHF1BF4XiRVO39mvSBTddmxIamq9I3bXmr3mM6wXtjOFJQx1dgLg%3D%3D?uid=0&filename=2017-10-24_19-40-52.png&disposition=inline&hash=&limit=0&content_type=image%2Fpng&fsize=74373&hid=9e68efdfd72fb05f9b9e4dd950cb3afe&media_type=image&tknv=v2&etag=33dfbfd3bc8dda7d69a7316c3ebd0c28)

Создаем pull request из week_1 в master. ОБРАТИТЕ ВНИМАНИЕ, если вы работали в ветке week_1 , то и пул реквест делаете из ветки week_1, для остальных веток меняйте соответственно. 
И скидываем ссылку наставнику на свой pull request

![Иллюстрация к проекту](https://2.downloader.disk.yandex.ru/disk/fcf3840b3bf8a93e0ba60717c098e5ad80f057f49098e586a6c4c9eff6688c26/59efa667/ePBJmrC14u0gjjVo9JgMX4wiTh-zpXnIhBt93b2s4ucMMY3lmgB-Rc-ndF7zMCDv0txknlHXkyO0avjqJ5aKsQ%3D%3D?uid=0&filename=2017-10-24_19-44-44.png&disposition=inline&hash=&limit=0&content_type=image%2Fpng&fsize=29929&hid=79920ec80d5a9822925fa52f5b9c70ea&media_type=image&tknv=v2&etag=c39decce045b84bbcad128faec1076c5)

### Публикуем изменения на github pages
В консоли пишем
```sh
git push origin week_3:gh-pages
```

### 3.2 Какие файлы, куда загружать.
В рабочие ветки week_1,week_2 и т.д загружаете все "рабочие файлы" ( т.е scss)
В ветку gh-pages, загружаете только CSS ( без SCSS)

week_3 заменяем на текущую недельную ветку

# Что отправлять наставнику:
- Ссылку на pull request
- Ссылу на Github Pages

Если наставник не успел проверить ваше задание или вы не доделали прошлую ветку, делаете новую ветку не из master а из актуальной ветки.

Работаете в ней, делаете коммит и пуш на удаленный репозиторий

Создаете новый pull request и снова пишите настанику
