# ethereum-workshop

* установка необходимого софта
* запуск контракта, просмотр работы приложения
* написание кода
* деплой в основную тестовую сетку

# Установка необходимого софта
1. npm, node, truffle, truffle-default-builder
2. **ВНИМАНИЕ!!!** Чтобы демо работало надо иметь версию truffle 3.2.1 . Если у вас уже стоит truffle, то удалите другую версию: `npm uninstall -g truffle` и напишите в терминале: `npm install -g truffle@3.2.1` 
3. устаналиваем `truffle-default-builder` с помощью `npm install truffle-default-builder --save`
4. если вы все правильно сделали, то сделайте `truffle init, truffle migrate, затем truffle build и truffle serve` и откроете браузер по ссылке `localhost:8080`



# Деплой в основную сетку
1. устанавливаем parity [link](https://github.com/paritytech/parity)
2. создаем аккаунт на [myetherwallet](https://www.myetherwallet.com/) в kovan testnet, сохраняем key-store file на компьютер
3. запускаем `parity-ui` и переходим в kovan testnet
4. импортируем аккаунт из key-store
5. чтобы получить 1 тестовый эфир: создаем gist на github с вашим адресом и пишем команду в терминале: `curl http://github-faucet.kovan.network/url --data "address=https://gist.github.com/[github_username]/[gist_hash]`, затем идем в https://kovan.etherscan.io/ и смотрим свои транзакции. Можно и другими способами: https://github.com/kovan-testnet/faucet
6. после того как тестовая сеть синхронизировалась мы запускаем `truffle migrate` и идем в parity клиент, чтобы подтвердить транзакции.<br>

Ремарка: тоже самое можно сделать, подняв рабочую через консоль или воспользоваться Infura
