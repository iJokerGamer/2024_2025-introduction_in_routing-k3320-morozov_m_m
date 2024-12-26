University: [ITMO University](https://itmo.ru/ru/)  
Faculty: [FICT](https://fict.itmo.ru)  
Course: [Introduction in routing](https://github.com/itmo-ict-faculty/introduction-in-routing)  
Year: 2024/2025
Group: K3320  
Author: Morozov Matvey  
Lab: Lab4  
Date of create: 24.12.2024  
Date of finished: 25.12.2024

## Лабораторная работ №4 "Эмуляция распределенной корпоративной сети связи, настройка iBGP, организация L3VPN, VPLS"

## <a>Ход работы</a>

- С помощью данной команды создаем папку:
  --- touch marsh3.clab.yaml---
- В файл записываем построение сети
- С помощью данной команды собираем Containerlab:
  --- sudo clab deploy marsh4.clab.yaml---
  <img src="./imgs/1.png" width=900>

- С помощью данной команды строим нашу сеть:
  --- sudo clab graph ---
  <img src="./imgs/2.png" width=900>
  <img src="./imgs/3.png" width=900>

С помощью данной команды входим в настроуку интерфейса:
--- sudo ssh admin@clab-lab4-...---

### <a>Текст конфигураций для каждого сетевого устройства</a>

#### <a>Настройка R01_NY:</a>

<img src="./imgs/4.png" width=900>

#### <a>Настройка R01_SBP:</a>

<img src="./imgs/5.png" width=900>

#### <a>Настройка R01_SVL:</a>

<img src="./imgs/6.png" width=900>

#### <a>Настройка R01_HKI:</a>

<img src="./imgs/7.png" width=900>

#### <a>Настройка R01_LND:</a>

<img src="./imgs/8.png" width=900>

#### <a>Настройка R01_LBN:</a>

<img src="./imgs/9.png" width=900>

### <a>Результаты пингов. Проверка связности VRF:</a>

<img src="./imgs/10.png" width=900>
<img src="./imgs/11.png" width=900>
<img src="./imgs/12.png" width=900>

#### <a>Настройка PC1:</a>

<img src="./imgs/13.png" width=900>

#### <a>Настройка PC2:</a>

<img src="./imgs/14.png" width=900>

#### <a>Настройка PC3:</a>

<img src="./imgs/15.png" width=900>

#### <a>Настройка R01_SVL:</a>

<img src="./imgs/16.png" width=900>

#### <a>Настройка R01_NY:</a>

<img src="./imgs/17.png" width=900>

#### <a>Настройка R01_SPB:</a>

<img src="./imgs/18.png" width=900>

### <a>Результаты пингов.</a>

<img src="./imgs/19.png" width=900>
<img src="./imgs/20.png" width=900>
<img src="./imgs/21.png" width=900>
