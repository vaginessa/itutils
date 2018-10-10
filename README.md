# Collection of utilities




## общие ресурсы

#### OWASP (https://www.owasp.org/index.php/Main_Page)

это открытый проект по обеспечению безопасности веб-приложений. На нем содержится большое количество материалов, гайдов по тестированию, разные чек-листы и другие материалы
обязательное изучения:

>https://www.owasp.org/index.php/Category:OWASP_Top_Ten_Project
>https://www.owasp.org/index.php/OWASP_Testing_Guide_v4_Table_of_Contents

#### exploit-db (https://www.exploit-db.com/)

#### IPper https://ipper.ru/

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

## тренинг

#### Damn Vulnerable Web Application (DVWA) (http://www.dvwa.co.uk/)

Это сайт на PHP, который демонстрирует ряд уязвимостей для изучения

#### Buggy web application (bWAPP) (http://www.itsecgames.com/)

Это открытое приложение и включает в себя около сотни уязвимостей, которые классифицируются по OWASP. Также есть готовая сборка для виртуальной машины bee-box.

## безопасность

WebRTC: может «засветить» реальный IP юзера, несмотря на использование VPN, Tor, Proxy.

# I just found the contents of this repository around the web.
