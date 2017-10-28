# ethereum-workshop

* установка необходимого софта
* запуск контракта, просмотр работы приложения
* написание кода
* деплой в основную тестовую сетку




# Деплой в основную сетку
1. устанавливаем parity [link](https://github.com/paritytech/parity)
2. создаем аккаунт на [myetherwallet](https://www.myetherwallet.com/) в kovan testnet, сохраняем key-store file на компьютер
3. запускаем `parity-ui` и переходим в kovan testnet
4. импортируем аккаунт из key-store
5. чтобы получить 1 тестовый эфир: создаем gist на github с вашим адресом и пишем команду в терминале: `curl http://github-faucet.kovan.network/url --data "address=https://gist.github.com/[github_username]/[gist_hash]`, затем идем в https://kovan.etherscan.io/ и смотрим свои транзакции. Можно и другими способами: https://github.com/kovan-testnet/faucet
6. после того как тестовая сеть синхронизировалась мы запускаем `truffle migrate` и идем в parity клиент, чтобы подтвердить транзакции.<br>

Ремарка: тоже самое можно сделать, подняв рабочую через консоль или воспользоваться Infura
