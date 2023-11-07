---
description: Как получить публичный и приватный ключи?
---

# Ключи MongoDB Atlas

{% hint style="info" %}
Облачные сервисы MongoDB могут быть заблокированы вашим провайдером. Используйте VPN. Если VPN нет, можно рассмотреть вариант расширения для браузера[ Hola VPN](https://chrome.google.com/webstore/detail/hola-vpn-the-website-unbl/gkojfkhlekighikafcpjkiklfbnlmeio).
{% endhint %}

Переходите по ссылке [https://www.mongodb.com/cloud/atlas/register](https://www.mongodb.com/cloud/atlas/register)

Заполняйте поля формы либо авторизуйтесь через Google. Затем подтверждайте регистрацию через e-mail. Перейдя по ссылке в письме, вы окажетесь на странице настройки кластера MongoDB Atlas. Скорее всего, вам предложат заполнить форму-опросник. Ответы не столь принципиальны. На вопрос о языке программирования можно ответить **JavaScript / Node.js**

После ответа на вопросы будет показана форма с опциями по развёртыванию кластера базы данных. Нужно выбирать бесплатный вариант **M0**.

Облачный провайдер - **AWS**, регион - любой европейский (предпочтителен **eu-central-1**, Frankfurt).

В поле **Name** вводите ppp, после чего нажимайте кнопку **Create**.

После создания кластера вы окажетесь в административной панели MongoDB Atlas. В верхней части страницы будут вкладки, переходите на **App Services**.

Если появится окно с предложением создать приложение (Build better apps faster with App Services), то выбирайте вариант **Build your own app**. Если окно не появилось, нажмите на кнопку **Create a New App**.

В следующем окне появится форма, где нужно выбрать (раздел **Link your Data Source**) ранее созданный кластер базы данных ppp.

В поле **Name your Application** вводите ppp

В секции **App Deployment Model** выбирайте вариант **Single Region**. Затем нажимайте на кнопку **Create App Service**.

Теперь, когда приложение MongoDB Atlas создано, можно получить ключи API для приложения ppp.&#x20;

Для этого найдите в верху страницы справа от значка шестерёнки выпадающий список **Access Manager**, а нем пункт **Project Access**.

В открывшейся странице перейдите на вкладку **API Keys**. Нажмите на кнопку **Create API Key**.

Далее появится форма, где в поле **Description** нужно ввести ppp, в выпадающем списке **Project Permissions** укажите роли: Project Cluster Manager, Project Data Access Admin, Project Data Access Read Write, Project Data Access Read Only, Project Read Only, Project Owner.

Нажимайте **Next**. Будут показаны два ключа: публичный и приватный. Вводите их в приложении ppp в облачных сервисах. Ключи отображаются только один раз, при закрытии страницы с MongoDB Atlas посмотреть их повторно не получится.
