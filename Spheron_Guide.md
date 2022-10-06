<div align="center">
  
# Hypersign validator node on Akash Network
# Нода валидатора сети Hypersign, развертка в Akash Network.
  
</div>
  
<div align="center">

<p align="center"><img src="https://user-images.githubusercontent.com/23629420/163564929-166f6a01-a6e2-4412-a4e9-40e54c821f05.png" width=70% </p>

| [Akash Network](https://akash.network/) | [Forum Akash Network](https://forum.akash.network/) | 
|:--:|:--:|
___
Before you start - subscribe to our news channels: 

Прежде чем начать - подпишитесь на наши новостные каналы:

| [Discord Akash](https://discord.gg/WR56y8Wt) | [Telegram Akash EN](https://t.me/AkashNW) | [Telegram Akash RU](https://t.me/akash_ru) | [TwitterAkash](https://twitter.com/akashnet_) | [TwitterAkashRU](https://twitter.com/akash_ru) |
|:--:|:--:|:--:|:--:|:--:|

</div>

<div align="center">
  
| [Discord Hypersign](https://discord.gg/ezJZVjPDDS) | [Twitter Hypersign](https://twitter.com/hypersignchain/) | [Site Hypersign](https://hypersign.id/) | [GitHub Hypersign](https://github.com/hypersign-protocol/hid-node) | [Telegram Hypersign](https://t.me/hypersignchain) |
|:--:|:--:|:--:|:--:|:--:|
  
</div>

<div align="center">
  
[English version](https://github.com/Dimokus88/Hypersign/tree/main#english-version) | [Русская версия](https://github.com/Dimokus88/Hypersign/tree/main#%D1%80%D1%83%D1%81%D1%81%D0%BA%D0%B0%D1%8F-%D0%B2%D0%B5%D1%80%D1%81%D0%B8%D1%8F) 
 
</div>

___

# English version
  
### Deploying a Hypersign node using Spheron.

**UI Spheron** works through a browser, it does not need to be installed as a separate software on your device. Go to https://aqua.spheron.network . Then log in
through the suggested methods on the site (I chose `github`).

<p align="center"><img src="https://user-images.githubusercontent.com/23629420/194246404-dd551cc4-5ba4-4722-b258-8fd4245cf976.PNG" width=30% </p>

Go to the **Billing** tab and make sure you have a **PRO** billing plan. If this is not the case - **change your tariff plan**.
> P.S. To replenish the balance of test USDT, use the [faucet](https://faucet.spheron.network/)

<p align="center"><img src="https://user-images.githubusercontent.com/23629420/194247295-603014c3-7560-4f4e-9a69-2ea39b86a52a.png" width=60% </p>

You must also have more than **6 AKT** on your account:

<p align="center"><img src="https://user-images.githubusercontent.com/23629420/194266961-12dbf8da-16bc-420b-94fc-34e06b6b9cf5.png" width=60% </p>

Switch to **Compute** mode:

<p align="center"><img src="https://user-images.githubusercontent.com/23629420/194298597-1ddf1f1f-6b62-42b8-b648-8d45c6d6dd8a.png" width=60% </p>

Let's go to the dashboard and create a new cluster:

<p align="center"><img src="https://user-images.githubusercontent.com/23629420/194307371-0e5c06da-85af-4e65-8e0a-ebdd4ac5897b.png" width=60% </p>

Specify the cluster name and deployment image `dimokus88/hypersign:0.2`:

<p align="center"><img src="https://user-images.githubusercontent.com/23629420/194306924-2c79519c-1371-4c7d-90d9-4f37ec56fb90.png" width=60% </p>

Click **Next** and select the desired resources for your deployment:

<p align="center"><img src="https://user-images.githubusercontent.com/23629420/194308760-9cb1bf90-a3b9-41d8-af90-047a19f00682.png" width=60% </p>

Open ports:

  * `80` - fixed **80**
  * `22` (for ssh connection) - **random**
  * `26656` (for p2p connections) - **random**
  * `26657` (for websocket) - **random**
  
Specify the following variables:
  * `my_root_password` - password for connecting via ssh to the node.
  * `MONIKER` - node name
  * `SNAP_RPC` - public RPC node for installation and network connection.
  
Click **Deploy**. It may take up to **5 minutes** to start a node and start synchronization.
  
<p align="center"><img src="https://user-images.githubusercontent.com/23629420/194317376-11481ff0-5bad-4def-a125-b2efcadaf7f1.png" width=70% </p>

Navigating to the forwarded port **26657**, the `websocket` of the node will open in the logs, where its up-to-date information will be available.
  
![image](https://user-images.githubusercontent.com/23629420/194314067-d0ad2488-57f0-4dde-b3f2-997243b4061d.png)

  
At this stage, the node is deployed, wait for synchronization.
<p align="center"><img src="https://user-images.githubusercontent.com/23629420/194318809-3e59fc20-2513-456d-8091-9e1fedb35b44.png" width=70% </p>


  
[Back to top](https://github.com/Dimokus88/Hypersign/blob/main/README.md#Hypersign-validator-node-on-akash-network)

**Thank you for using Akash Network!**
___

___
# Русская версия
  
### Развертка ноды Hypersign с помощью Spheron.

**UI Spheron** работает через браузер, его не нужно устанавливать как отдлеьное ПО на ваше устройство. Перейдите по адресу https://aqua.spheron.network . Затем авторизуйтесь
через предложенные способы на сайте (я выбрал `github`).

<p align="center"><img src="https://user-images.githubusercontent.com/23629420/194246404-dd551cc4-5ba4-4722-b258-8fd4245cf976.PNG" width=30% </p>

Перейдите во вкладку **Billing** и убедитесь что у вас стоит тарифный план **PRO**. Если это не так - **смените тарфиный план**.
> P.S. Для пополнения баланса тестовых USDT восплользуйтесь [краном](https://faucet.spheron.network/)

<p align="center"><img src="https://user-images.githubusercontent.com/23629420/194247295-603014c3-7560-4f4e-9a69-2ea39b86a52a.png" width=60% </p>

Также у вас должно быть на счете более **6 AKT**:

<p align="center"><img src="https://user-images.githubusercontent.com/23629420/194266961-12dbf8da-16bc-420b-94fc-34e06b6b9cf5.png" width=60% </p> 

Переключитесь в режим **Compute**:

<p align="center"><img src="https://user-images.githubusercontent.com/23629420/194298597-1ddf1f1f-6b62-42b8-b648-8d45c6d6dd8a.png" width=60% </p> 

Перейдем в дашборд и создадим новый кластер:

<p align="center"><img src="https://user-images.githubusercontent.com/23629420/194307371-0e5c06da-85af-4e65-8e0a-ebdd4ac5897b.png" width=60% </p> 

Укажте имя кластера и образ развертывания `dimokus88/hypersign:0.2`:

<p align="center"><img src="https://user-images.githubusercontent.com/23629420/194306924-2c79519c-1371-4c7d-90d9-4f37ec56fb90.png" width=60% </p>  

Нажмите **Next** и выберете желаемые ресурсы для вашего развертывания:

<p align="center"><img src="https://user-images.githubusercontent.com/23629420/194308760-9cb1bf90-a3b9-41d8-af90-047a19f00682.png" width=60% </p>  

Откройте порты:

  * `80` - фиксированный **80**
  * `22` (для подключения по ssh) - **рандом** 
  * `26656` (для p2p соединений)- **рандом**
  * `26657` (для вебсокета)- **рандом**
  
Укажите следующие переменные:
  * `my_root_password` - пароль для подключение по ssh к ноде.
  * `MONIKER` - имя ноды
  * `SNAP_RPC` - публичная RPC нода для инсталяции и подключения к сети.
  
Нажмите **Deploy**. Для запуска ноды и начала синхронизации может потребоваться **от 5 минут**.
  
<p align="center"><img src="https://user-images.githubusercontent.com/23629420/194317376-11481ff0-5bad-4def-a125-b2efcadaf7f1.png" width=70% </p>

Перейдя на переадресованный порт **26657** в логах откроется `websocket` ноды, где будет доступна ее актуальная информация. 
  
![image](https://user-images.githubusercontent.com/23629420/194314067-d0ad2488-57f0-4dde-b3f2-997243b4061d.png)

  
На данном этапе нода развернута, дождитесь синхронизации.

<p align="center"><img src="https://user-images.githubusercontent.com/23629420/194318809-3e59fc20-2513-456d-8091-9e1fedb35b44.png" width=70% </p>
  
[К началу](https://github.com/Dimokus88/Hypersign/blob/main/README.md#Hypersign-validator-node-on-akash-network)

**Спасибо что воспользовались Akash Network!**
___

