University: [ITMO University](https://itmo.ru/ru/)  
Faculty: [FICT](https://fict.itmo.ru)  
Course: [Introduction in routing](https://github.com/itmo-ict-faculty/introduction-in-routing)  
Year: 2024/2025
Group: K3320  
Author: Morozov Matvey  
Lab: Lab3  
Date of create: 24.12.2024  
Date of finished: 25.12.2024

## Лабораторная работ №3 "Эмуляция распределенной корпоративной сети связи, настройка OSPF и MPLS, организация первого EoMPLS"

## <a>Ход работы</a>

#### <a>Минимальная теория</a>

- MPLS - это метод маркировки данных через приоритетность данных (скорость увеличивается)
- OSPF - метод графа, нахождение кратчайшего пути.
- EoMPLS - EoMPLS представляет собой метод передачи Ethernet-фреймов через MPLS-сеть, позволяя нам объединить преимущества обоих протоколов.

#### <a>Первый этап</a>

- С помощью данной команды создаем папку:
  --- touch marsh3.clab.yaml---
- В файл записываем построение сети
- С помощью данной команды собираем Containerlab:
  --- sudo clab deploy marsh3.clab.yaml---
- С помощью данной команды строим нашу сеть:
  --- sudo clab graph ---

<img src="./imgs/1.png" width=900>

#### <a>Второй этап-настройка устройств</a>

С помощью данной команды входим в настроуку интерфейса:
--- sudo ssh admin@clab-lab3-...---

#### <a>R01.NY</a>

<img src="./imgs/2.png" width=900>

#### <a>R01.LDN</a>

<img src="./imgs/3.png" width=900>

#### <a>R01.HKI</a>

<img src="./imgs/4.png" width=900>

#### <a>R01.SPB</a>

<img src="./imgs/5.png" width=900>

#### <a>R01.MSK</a>

<img src="./imgs/6.png" width=900>

#### <a>R01.LBN</a>

<img src="./imgs/7.png" width=900>

#### <a>SGI-Prism</a>

<img src="./imgs/8.png" width=900>

#### <a>PC1</a>

<img src="./imgs/9.png" width=900>

#### <a>Результат пинга</a>

<img src="./imgs/10.png" width=900>

#### <a>Пример таблицы маршрутов MPLS</a>

<img src="./imgs/11.png" width=900>

#### <a>Вывод</a>

В ходе выполнения данной лабораторной работы мы на практике познакомились с протоколами OSPF, MPLS, EoMPLS и механизмами их организации.
