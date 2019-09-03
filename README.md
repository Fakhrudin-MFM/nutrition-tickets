# IONDV. Nutrition-tickets

Эта страница на [Русском](/README_RU.md)

<h1 align="center"> <a href="https://www.iondv.com/"><img src="/nutrition_tickets.png" height="500px" alt="IONDV. Framework nutrition tickets" align="center"></a>
</h1>  

The **IONDV. Nutrition-tickets** web-app is licensed under **Apache 2.0**. The app is implemented on IONDV. Framework as a simple example of a basic application created in [IONDV. Studio](https://github.com/iondv/studio/blob/master/readme_ru.md).  It's a part of "How to create applications in IONDV. Studio" [tutorial](https://www.youtube.com/watch?v=e201ko9fkQ8). 

### IONDV. Framework in brief

**IONDV. Framework** - is a node.js open source framework for developing accounting applications
or microservices based on metadata and individual modules. Framework is a part of 
instrumental digital platform to create enterprise 
(ERP) apps. This platform consists of the following open-source components: the [IONDV. Framework](https://github.com/iondv/framework), the
[modules](https://github.com/topics/iondv-module) и ready-made applications expanding it
functionality, visual development environment [Studio](https://github.com/iondv/studio) to create metadata for the app.

* For more details, see [IONDV. Framework site](https://iondv.com). 

* Documentation is available in the [Github repository](https://github.com/iondv/framework/blob/master/docs/en/index.md).

## Description 

**IONDV. Nutrition-tickets** - is a web application based on [IONDV. Framework](https://iondv.com), created in [IONDV. Studio](https://github.com/iondv/studio/blob/master/README.md). It is used as a registry to account, store, and present the data on preferential coupons for citizens with a preferential category. Основное назначение приложения это выдача талонов на получение социального питания.
Ключевой сущность является *Талон*, который содержит в себе информацию описательного характера и ссылки на гражданина, которому предназначен. 
*Главное преимущество* - контроль за льготными талонами граждан, имеющих ту или иную льнотную категорию, что позволяет, при необходимости, получить точную информации о талоне и гражданине.

### Как создать? 

Смотрите [видео](https://www.youtube.com/watch?v=e201ko9fkQ8&t=331s) о создании простого приложения [IONDV. Nutrition-tickets](https://github.com/iondv/nutrition-tickets) в **IONDV. Studio**. Читайте подробную [инструкцию](https://github.com/iondv/nutrition-tickets/blob/master/tutorial/ru/index.md), где поэтапно описаны действия для создания системы в **IONDV. Studio**.

<a href="https://www.youtube.com/watch?v=e201ko9fkQ8&t=331s" target="_blank"><img src="/tickets_video.png" height="250px" alt="" title=""></a>

## Демо

Демо доступ в систему для ознакомления, без регистрации: https://nutrition-tickets.iondv.com. Существует три основных роли: **оператор**, **кассир**, **контролёр**. Название роли соответствует ее логину, пароль один для всех трех логинов - **ion-demo**. 

Учетная запись для [бек-офиса](https://nutrition-tickets.iondv.com/registry) под пользователем с ролью "Администратор": логин **demo**, пароль **ion-demo**. 

### Модули

Основу реестра талонов составляет [модуль Регистри](https://github.com/iondv/registry). 
Также используются: 

* [Административный модуль](https://github.com/iondv/ionadmin) - позволяет управлять пользователями и ролями для доступа к системе и другими функциями, неоходимыми администартору.  

## Как получить?  

### Git

Быстрый старт с использованием репозитория IONDV. Nutrition-tickets на GitHub — [подробная инструкция](https://github.com/iondv/framework/blob/master/docs/ru/readme.md#быстрый-старт-с-использованием-репозитория).  

1. Установите системное окружение и глобальные зависимости.
2. Клонируйте ядро, модуль и приложение.
3. Соберите и разверните приложение.
4. Запустите.

Или установка и запуск в одну строку под Linux с использованием установщика [iondv-app](https://github.com/iondv/iondv-app) (требуется локально node.js, MongoDB и Git):
```
bash <(curl -sL https://raw.githubusercontent.com/iondv/iondv-app/master/iondv-app) -q -i -m localhost:27017 nutrition-tickets
```
Где вместо `localhost:27017` нужно указать адрес MongoDb. После запуска открыть ссылку 'http://localhost:8888', учетная запись бек офиса **demo**, пароль **ion-demo**.

### Docker

Запуск приложения с использованием докер контейнера - [подробная инструкция](https://hub.docker.com/r/iondv/nutrition-tickets).

1. Запустите СУБД mongodb: `docker run --name mongodb -v mongodb_data:/data/db -p 27017:27017 -d mongo`
2. Запустите IONDV. Telecom `docker run -d -p 80:8888 --link mongodb iondv/nutrition-tickets`.
3. Откройте ссылку `http://localhost` в браузере через минуту (время требуется для инициализации данных). Для бек офиса логин: **demo**, пароль: **ion-demo** 

## Ссылки

Для дополнительной информации смотрите следующие ресурсы:

* [Инструкция по созданию IONDV. Ticket](tutorial/ru/index.md)
* [Руководство пользователя IONDV. Studio](https://github.com/iondv/studio/tree/master/manuals/RP_studio.docx)
* [IONDV. Framework](https://iondv.com/) 
* [Facebook](https://www.facebook.com/iondv/)

--------------------------------------------------------------------------  


#### [License](/LICENSE) &ensp; [Contact us](https://iondv.com/contacts) &ensp; [Russian](/README_RU.md)          
<div><img src="https://mc.iondv.com/watch/github/docs/ticket-en" style="position:absolute; left:-9999px;" height=1 width=1 alt="iondv metrics"></div>


--------------------------------------------------------------------------  

Copyright (c) 2018 **LLC "ION DV".**  
All rights reserved.
