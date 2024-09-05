---
## Front matter
title: "Отчёт по лабораторной работе №1


Информационная безопасность"
subtitle: "Установка и конфигурация операционной системы на виртуальную машину"
author: "Выполнила: Шаповалова Диана Дмитриевна, 


НПИбд-02-21, 1032211220"

## Generic otions
lang: ru-RU
toc-title: "Содержание"

## Bibliography
bibliography: bib/cite.bib
csl: pandoc/csl/gost-r-7-0-5-2008-numeric.csl

## Pdf output format
toc: true # Table of contents
toc-depth: 2
lof: true # List of figures
fontsize: 12pt
linestretch: 1.5
papersize: a4
documentclass: scrreprt
## I18n polyglossia
polyglossia-lang:
  name: russian
  options:
	- spelling=modern
	- babelshorthands=true
polyglossia-otherlangs:
  name: english
## I18n babel
babel-lang: russian
babel-otherlangs: english
## Fonts
mainfont: PT Serif
romanfont: PT Serif
sansfont: PT Sans
monofont: PT Mono
mainfontoptions: Ligatures=TeX
romanfontoptions: Ligatures=TeX
sansfontoptions: Ligatures=TeX,Scale=MatchLowercase
monofontoptions: Scale=MatchLowercase,Scale=0.9
## Biblatex
biblatex: true
biblio-style: "gost-numeric"
biblatexoptions:
  - parentracker=true
  - backend=biber
  - hyperref=auto
  - language=auto
  - autolang=other*
  - citestyle=gost-numeric
## Pandoc-crossref LaTeX customization
figureTitle: "Рис."
tableTitle: "Таблица"
listingTitle: "Листинг"
lofTitle: "Список иллюстраций"
lolTitle: "Листинги"
## Misc options
indent: true
header-includes:
  - \usepackage{indentfirst}
  - \usepackage{float} # keep figures where there are in the text
  - \floatplacement{figure}{H} # keep figures where there are in the text
---

# Цель работы
Целью данной работы является приобретение практических навыков установки операционной системы на виртуальную машину, настройки минимально необходимых для дальнейшей работы сервисов.

# Последовательность выполнения работы
 Запустите виртуальную машину VirtualBox. Создайте новую виртуальную машину. Для этого в VirtualBox выберите
Машина-Создать.  
 Укажите имя виртуальной машины (ваш логин в дисплейном классе), тип операционной системы — Linux, RedHat. Укажите размер основной памяти виртуальной машины — 2048
МБ (или большее число, кратное 1024 МБ, если позволяют технические характеристики вашего компьютера). Задайте конфигурацию жёсткого диска — загрузочный,VDI (BirtualBox Disk
Image), динамический виртуальный диск.  
 Задайте размер диска — 40 ГБ (или больше), его расположение — в данном
случае /var/tmp/имя_пользователя/имя_пользователя.vdi.  
![image](https://github.com/user-attachments/assets/322eb1ef-6882-42f3-8374-9eafef891177)  
 Выберите в VirtualBox для Вашей виртуальной машины Настройки-Носители . Добавьте новый привод оптических дисков и выберите образ операционной системы.  
![image](https://github.com/user-attachments/assets/6ae00f7c-7727-49ae-b1f5-7a594a7b7064)  
 Запустите виртуальную машину, выберите English в качестве языка интерфейса и перейдите к настройкам установки операционной
системы.  
 При необходимости скорректируйте часовой пояс, раскладку клавиатуры
(рекомендуется добавить русский язык, но в качестве языка по умолчанию указать английский язык; задать комбинацию клавиш для переключения
между раскладками клавиатуры — например Alt + Shift ).  
 В разделе выбора программ укажите в качестве базового окружения
Server with GUI , а в качестве дополнения — Development Tools. Отключите KDUMP.  
 Место установки ОС оставьте без изменения. Включите сетевое соединение и в качестве имени узла укажите
user.localdomain, где вместо user укажите имя своего пользователя в соответствии с соглашением об именовании.  
 Установите пароль для root и пользователя с правами администратора. После завершения установки операционной системы корректно перезапустите виртуальную машину и примите условия лицензии.  
![image](https://github.com/user-attachments/assets/11a3132b-bc41-4eaf-911c-fd90f5a5a55c)  
![image](https://github.com/user-attachments/assets/4464718b-f194-48c3-85b1-7c43e8bfa4d9)  
![image](https://github.com/user-attachments/assets/2c18262d-d169-4b64-9de0-49c330ec9709)  

# Домашнее задание
 Дождитесь загрузки графического окружения и откройте терминал. В окне
терминала проанализируйте последовательность загрузки системы, выполнив команду dmesg.  
Можно использовать поиск с помощью grep:  
dmesg | grep -i "то, что ищем"  
Получите следующую информацию.  
1. Версия ядра Linux (Linux version).  
2. Частота процессора (Detected Mhz processor).  
3. Модель процессора (CPU0).  
4. Объем доступной оперативной памяти (Memory available).  
5. Тип обнаруженного гипервизора (Hypervisor detected).  
6. Тип файловой системы корневого раздела.  
![image](https://github.com/user-attachments/assets/38253019-5bef-43fd-a6d9-85f72b5585d1)

# Вывод 
 Было настроено рабочее пространство для лабораторных работ, приобретены практические навыки
установки операционной системы на виртуальную машину и настройки минимально необходимых для дальнейшей работы сервисов.  

# Список литературы
 Документация по Virtual Box: https://www.virtualbox.org/wiki/Documentation



