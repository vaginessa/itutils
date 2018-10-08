# Collection of utilities




## General

#### OWASP (https://www.owasp.org/index.php/Main_Page)

это открытый проект по обеспечению безопасности веб-приложений. На нем содержится большое количество материалов, гайдов по тестированию, разные чек-листы и другие материалы
обязательное изучения:

>https://www.owasp.org/index.php/Category:OWASP_Top_Ten_Project
>https://www.owasp.org/index.php/OWASP_Testing_Guide_v4_Table_of_Contents

#### exploit-db (https://www.exploit-db.com/)




## Website scan

### Dnsrecon (Kali)
Утилита на Python, которая отображает хосты, домены и другую информация о сайте. 

Для базового тестирования:
> dnsrecon -d site.com

для брута деректорий:
> dnsrecon -d c -D /root/dnsmapCommonSubdomains.txt

### Dirb (Kali)
Он покажет всевозможные существующие страницы, где ответы не содержат код страницы 404. 
> dirb site.com

### Nmap (Kali)
Сетевой сканер, который позволяет показать какие порты используются и что на них установлено.





## Wordpress

### WPscan (Kali)
> wpscan -u site.com

после найти уязвимости: exploit-db




## тренинг

### Damn Vulnerable Web Application (DVWA) (http://www.dvwa.co.uk/)

Это сайт на PHP, который демонстрирует ряд уязвимостей для изучения

### Buggy web application (bWAPP) (http://www.itsecgames.com/)

Это открытое приложение и включает в себя около сотни уязвимостей, которые классифицируются по OWASP. Также есть готовая сборка для виртуальной машины bee-box.


