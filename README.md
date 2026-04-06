# 1. Тема и целевая аудитория

Социальная сеть для просмотра фото- и видео- контента

## 1.1 Аналоги
Среди аналогов можно выделить Instagram, TikTok, Vk, Facebook, Snapchat, Pinterest и другие

## 1.2 Аудитория

**Основная аудитория:** люди в возрасте от 13 до 65 лет, где самая активная группа: мужчины и женщины в возрасте от 25 до 34 лет (17,9%) [[1]](https://datareportal.com/reports/digital-2022-instagram-headlines?rq=instagram)

**География:** сервис ориентирован на пользователей со всего мира (глобальная)

**Охват аудитории:** по данным [[2]](https://www.statista.com/statistics/272014/global-social-networks-ranked-by-number-of-users/) число активных пользователей Instagram за месяц составлят 3 млрд.

## 1.3 Требования к функционалу

1. Публикация контента (фото или видео)
2. Просмотр ленты
3. Оценка понравившегося контента
4. Публикация историй
5. Просмотр историй

## 1.4 Метрики

| Метрика | Значение | Описание |
| :--- | :--- | :--- |
| MAU | 3 млрд [[2]](https://www.statista.com/statistics/272014/global-social-networks-ranked-by-number-of-users/) | Количество пользователей в месяц |
| DAU | 500 млн [[3]](https://www.demandsage.com/instagram-statistics/) | Количество пользователей в день |
| Посты в месяц | 17 шт [[4]](https://buffer.com/resources/instagram-engagement-rate/) | Среднее кол-во публикаций в месяц |
| Тип публикуемого контента | 5.3 - фото, 2.4 - карусель, 2.3 - reels [[5]](https://metricool.com/instagram-research-study-2023/) | Распределение контента на 10 публикаций |
| Тип контента в stories | 57% фото, 43% видео [[10]](https://www.socialinsider.io/social-media-benchmarks/instagram-stories-benchmarks/) | Распределение контента в сторис |
| Кол-во подписчиков | 1k - 10k [[9]](https://mention.com/en/reports/instagram/followers/) | Медианное значение кол-ва подписчиков на один аккаунт |
| Просмотр Reels | 30% [[12]](https://www.outfame.com/blog/instagram-reels-statistics/) | Процент проведенный за просмотр Reels относительно всего времени, проведенного в приложении |
| Просмотр Stories | 20% [[12]](https://backlinko.com/instagram-users/) | Процент проведенный за просмотр Stories относительно всего времени, проведенного в приложении |
| Скролл ленты | 35% [[12]](https://backlinko.com/instagram-users/) | Процент проведенный за скроллом ленты относительно всего времени, проведенного в приложении
| Время в Instagram | 33.9 минут [[12]](https://backlinko.com/instagram-users/) | Время проведенное пользователем в Instagram за день в среднем |


# 2. Расчет нагрузки

## 2.1 Продуктовые метрики
### Сводная таблица
| Метрика | Значение |
| :--- | :--- |
| MAU | 3 млрд [[2]](https://www.statista.com/statistics/272014/global-social-networks-ranked-by-number-of-users/) |
| DAU | 500 млн [[3]](https://www.demandsage.com/instagram-statistics/) |
| Средний размер хранилища пользователя | 5.78 Гб |
| Среднее количество действий пользователя в день | 182.09 |

### Средний размер хранилища пользователя
Исходя из [[2]](https://www.statista.com/statistics/272014/global-social-networks-ranked-by-number-of-users/) и [[3]]( https://www.demandsage.com/instagram-statistics/) посчитаем средний возраст одного аккаунта Instagram
| Год | Число пользователей | Разница с предыдущим годом | Возраст |
| :--- | :--- | :--- | :--- |
| 2013 | 110 млн | 110 млн | 13 лет |
| 2014 | 200 млн | 90 млн | 12 лет |
| 2015 | 370 млн | 170 млн | 11 лет |
| 2016 | 500 млн | 130 млн | 10 лет |
| 2017 | 700 млн | 200 млн | 9 лет |
| 2018 | 1 млрд | 300 млн | 8 лет |
| 2019 | 1.1 млрд | 100 млн | 7 лет |
| 2020 | 1.3 мдрд | 200 млн | 6 лет |
| 2021 | 2 млрд | 700 млн | 5 лет |
| 2022 | 2.3 мдрд | 300 млн | 4 года |
| 2023 | 2.4 мдрд | 100 млн | 3 года |
| 2025 | 3 млрд | 600 млн | 1 год |

Тогда средний возраст аккаунта в Instagram расчитывается как:

$$
\frac{
13 * 110 + 12 * 90 + 11 * 170 + 10 * 130 + 9 * 200 + 8 * 300 + 7 * 100 + 6 * 200 + 5 * 700 + 4 * 300 + 3 * 100 + 1 * 600
}{
3000
} = 5.793
$$

Найдем средний объем данных для пользователя:
| Тип данных | Среднее кол-во в месяц, шт | Размер 1 единицы | Средний срок хранения (лет) | Всего, шт | Всего | Расчет |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| Фото | 9.01 | 250 Кб | 5.793 | 626.34 | 156.59 Мб | Кол-во: 17 постов * 0.53 доля постов с фото (раздел 1.4) |
| Видео (reels) | 3.91 | 7 Мб | 5.793 | 271.81 | 1.9 Гб | Кол-во: 17 постов * 0.23 для постов с видео (раздел 1.4) |
| Stories | 17 [[10]](https://www.socialinsider.io/social-media-benchmarks/instagram-stories-benchmarks/) | 3.15 Мб | 5.793 | 1181.77 | 3.72 Гб | Кол-во Мб: 250 Кб * 0.57 + 7 Мб * 0.43 (раздел 1.4) |
| **Итого** |  |  |  | **2079.92** | **5.78 Гб** |

### Среднее количество действий пользователя в день
| Действие | Среднее, шт | Пояснение
| :--- | :--- | :--- |
| Вход/загрузка ленты | 7 [[11]](https://afftank.com/blog/instagram-statistics/) | - |
| Просмотр постов | 71.19 | 35% времени на ленту из общего времени 33.9 минут (раздел 1.4). Один пост до 10 секунд |
| Просмотр Reels | 30 | 30% времени на Reels из общего времени 33.9 минут (раздел 1.4). Один Reels 15-20 секунд |
| Просмотр Stories | 52.9 | 20% времени на Stories из общего времени 33.9 минут (раздел 1.4). Одна Stories 5-7 секунд |
| Лайки и комментарии | 20 [[13]](https://eathealthy365.com/how-many-daily-likes-does-instagram-really-get/) | - |
| Публикация фото | 0.3 | Из расчета 9.01 в месяц |
| Публиакция Reels | 0.13 | Из расчета 3.91 в месяц |
| Публикация Stories | 0,57 | Из расчета 17 в месяц |
| **Итого** | **182.09** |

## 2.2 Технические метрики
### Сводная таблица
| Метрика | Значение |
| :--- | :--- |
| Хранилище | 17 330 Пб |
| Суммарный суточный трафик | 199 Пб |
| Средняя нагрузка | 18 389 Гбит/с |
| Пиковая нагрузка | 55 168 Гбит/с |
| RPS (средний) | 1 053 819 |
| RPS (пиковый, ×3) | 3 161 457 |

### Хранилище
Для 3 мдрд активных пользователей [[2]](https://www.statista.com/statistics/272014/global-social-networks-ranked-by-number-of-users/)
| Тип данных | Значение для одного пользователя, шт | Значение для одного пользователя | Общее значение, млрд шт | Общее значение, Пб |
| :--- | :--- | :--- | :--- | :--- |
| Фото | 626.34 | 156.59 Мб | 1879.02 | 469.77 | 
| Видео | 271.81 | 1.9 Гб | 815.43 | 5700 |
| Stories | 1181.77 | 3.72 Гб | 3545.31 | 11160 |
| **Итого** |  |  | **6.239 трлн** | **17 330 Пб** |  

### Сетевой трафик
Суточный трафик на 500 млн пользователей [[3]](https://www.demandsage.com/instagram-statistics/). Пиковую нагрзуку возьмем ×3 относительно средней нагрузки [[15]](https://www.designgurus.io/answers/detail/how-do-you-estimate-capacity-rpsstoragebandwidth-for-a-social-app)

<table>
  <tr>
    <td rowspan="4"><strong>Трафик на скачивание контента</strong></td>
    <td><strong>Действие</strong></td>
    <td><strong>Суточный объем, Пб</strong></td>
    <td><strong>Средняя нагрузка, Гбит/с</strong></td>
    <td><strong>Пиковая нагрузка (×3), Гбит/с</strong></td>
    <td><strong>Расчет</strong></td>
  </tr>
  <tr>
    <td>Просмотр ленты</td>
    <td>8.9</td>
    <td>823.96</td>
    <td>2 471.88</td>
    <td>500 млн * 71.19 * 250 Кб</td>
  </tr>
  <tr>
    <td>Просмотр Reels</td>
    <td>105</td>
    <td>9 722.22</td>
    <td>29 166.67</td>
    <td>500 млн * 30 * 7 Мб</td>
  </tr>
  <tr>
    <td>Просмотр Stories</td>
    <td>83.32</td>
    <td>7 714.58</td>
    <td>23 143.75</td>
    <td>500 млн * 52.9 * 3.15 Мб</td>
  </tr>
  <tr>
    <td rowspan="3"><strong>Трафик на загрузку контента</strong></td>
    <td>Публикация фото</td>
    <td>0.0375</td>
    <td>3.47</td>
    <td>10.42</td>
    <td>500 млн * 0.3 * 250 Кб</td>
  </tr>
  <tr>
    <td>Публикация Reels</td>
    <td>0.455</td>
    <td>42.13</td>
    <td>126.39</td>
    <td>500 млн * 0.13 * 7 Мб</td>
  </tr>
  <tr>
    <td>Просмотр Stories</td>
    <td>0.90</td>
    <td>83.125</td>
    <td>249.375</td>
    <td>500 млн * 0.57 * 3.15 Мб</td>
  </tr>
  <tr>
    <td><strong>Итого</strong></td>
    <td></td>
    <td><strong>199</strong></td>
    <td><strong>18 389</strong></td>
    <td><strong>55 168</strong></td>
    <td></td>
  </tr>
</table>

### RPS

<table>
  <tr>
    <td rowspan="5"><strong>Запросы на чтение</strong></td>
    <td><strong>Действие</strong></td>
    <td><strong>Суточное количество</strong></td>
    <td><strong>RPS (средний)</strong></td>
    <td><strong>RPS (пиковый, ×3)</strong></td>
    <td><strong>Расчет</strong></td>
  </tr>
  <tr>
    <td>Вход/загрузка ленты</td>
    <td>3.5 млрд</td>
    <td>40 509</td>
    <td>121 527</td>
    <td>500 млн * 7</td>
  </tr>
  <tr>
    <td>Просмотр постов (лента)</td>
    <td>35.6 млрд</td>
    <td>412 037</td>
    <td>1 236 111</td>
    <td>500 млн * 71.19</td>
  </tr>
  <tr>
    <td>Просмотр Reels</td>
    <td>15 млрд</td>
    <td>173 611</td>
    <td>520 833</td>
    <td>500 млн * 30</td>
  </tr>
  <tr>
    <td>Просмотр Stories</td>
    <td>26.45 млрд</td>
    <td>306 134</td>
    <td>918 402</td>
    <td>500 млн * 52.9</td>
  </tr>
  <tr>
    <td rowspan="4"><strong>Запросы на запись</strong></td>
    <td>Лайки и комментарии</td>
    <td>10 млрд</td>
    <td>115 741</td>
    <td>347 223</td>
    <td>500 млн * 20</td>
  </tr>
  <tr>
    <td>Публикация фото</td>
    <td>150 млн</td>
    <td>1 736</td>
    <td>5 208</td>
    <td>500 млн * 0.3</td>
  </tr>
  <tr>
    <td>Публикация Reels</td>
    <td>65 млн</td>
    <td>752</td>
    <td>2 256</td>
    <td>500 млн * 0.13</td>
  </tr>
  <tr>
    <td>Публикация Stories</td>
    <td>285 млн</td>
    <td>3 299</td>
    <td>9 897</td>
    <td>500 млн * 0.57</td>
  </tr>
  <tr>
    <td colspan="2"><strong>Итого</strong></td>
    <td><strong>91.05 млрд</strong></td>
    <td><strong>1 053 819</strong></td>
    <td><strong>3 161 457</strong></td>
    <td></td>
  </tr>
</table>

# 3. Глобальная балансировка нагрузки
## 3.1 Разбиение по доменам
| Домен | Функциональность |
| :--- | :--- | 
| api.social.com | Лента, посты, лайки, stories metadata, пользователи | 
| cdn.social.com | Фото, reels, stories | 
| upload.social.com | Загрузка контента |

## 3.2 Расположение ДЦ
Согласно [[16]](https://www.theglobalstatistics.com/instagram-global-users-statistics) распределение аудитории в Instagram происходит неравномерно. Большая часть (~50%) приходится на Азию, а следующий по количество пользователей регион - Америка. Тогда, исходя из этих данных, расположение основных ДЦ выглядит так:
| Регион | Город, страна | Обоснование | Процент покрытия, % | RPS, средний | RPS, x3 |
| :--- | :--- | :--- | :--- | :--- | :--- |
| Северная Америка | Ашберн, США | крупнейший интернет-хаб, низкая latency по США | 11 | 115 920 | <nobr>347 760</nobr> |
| Южная Америка | Сан-Паулу, Бразилия | крупнейший рынок региона, развитая инфраструктура | 14 | 147 534 | 442 604 |
| Европа | Франкфурт, Германия | главный интернет-хаб Европы (DE-CIX), центр EU трафика | 19 | 200 226 | 600 677 |
| Южная Азия | Мумбаи, Индия | низкая latency для Индии | 28 | 295 069 | 885 208 |
| Юго-восточная Азия | Сингапур | ключевой хаб Юго-Восточной Азии | 25 | 263 454 | 790 364 |

Размещение ДЦ вблизи крупнейших регионов присутствия аудитории позволяет снизить задержку для основных пользовательских сценариев: загрузка ленты, просмотр stories и reels, публикация контента. Это положительно влияет на DAU, среднее время, проведенное в приложении, а также снижает вероятность отказа при загрузке фото и видео.

## 3.3 Распределение запросов по типам по ДЦ
| Тип запроса         | Глобальный средний RPS | Принцип распределения по ДЦ                                   |
| :------------------ | :--------------------: | :------------------------------------------------------------ |
| Загрузка ленты      |         40 509         | по Geo DNS пропорционально доле аудитории региона             |
| Просмотр постов     |         412 037        | по Geo DNS пропорционально доле аудитории региона             |
| Просмотр Reels      |         173 611        | metadata через `api.social.com`, медиа через `cdn.social.com` |
| Просмотр Stories    |         306 134        | metadata через `api.social.com`, медиа через `cdn.social.com` |
| Лайки и комментарии |         115 741        | по Geo DNS в ближайший ДЦ                                     |
| Публикация фото     |          1 736         | через `upload.social.com` в ближайший ДЦ                      |
| Публикация Reels    |           752          | через `upload.social.com` в ближайший ДЦ                      |
| Публикация Stories  |          3 299         | через `upload.social.com` в ближайший ДЦ                      |


## 3.4 Схема глобальной балансировки
Регулировка трафика между датацентрами осуществляется на нескольких уровнях. На глобальном уровне используется Geo DNS, который направляет пользователей в ближайший датацентр. Для более точного распределения нагрузки применяется weighted DNS routing, позволяющий изменять долю трафика, направляемого в каждый регион.

В случае отказа датацентра используется механизм health-check и failover: недоступные регионы исключаются из DNS-ответов, и новые запросы перенаправляются в резервные датацентры.

Для доставки мультимедийного контента используется CDN с поддержкой Anycast. При недоступности origin-сервера в одном регионе CDN может обращаться к другому датацентру (origin failover).

```mermaid
flowchart LR
    U[Пользователь]

    %% Домены
    U --> API[api.social.com]
    U --> UPLOAD[upload.social.com]
    U --> CDN[cdn.social.com]

    %% DNS балансировка
    API --> DNS1[Geo DNS]
    UPLOAD --> DNS2[Geo DNS]

    DNS1 --> DC[Nearest DC]
    DNS2 --> DC

    %% CDN Anycast
    CDN --> ANYCAST[Anycast routing]
    ANYCAST --> EDGE[CDN Edge]

    EDGE -->|cache hit| U
    EDGE -->|cache miss| DC

    %% Failover (логика)
    DNS1 -.->|failover| DC
    DNS2 -.->|failover| DC
    EDGE -.->|origin fallback| DC
```

## Источники

1. https://datareportal.com/reports/digital-2022-instagram-headlines?rq=instagram
2. https://www.statista.com/statistics/272014/global-social-networks-ranked-by-number-of-users/
3. https://www.demandsage.com/instagram-statistics/
4. https://buffer.com/resources/instagram-engagement-rate/
5. https://metricool.com/instagram-research-study-2023/
6. https://tinyimagepro.com/blog/compress-photos-for-social-media/
7. https://arxiv.org/abs/2008.11317
8. https://ru.tipard.com/video/crop-video-in-instagram.html
9. https://mention.com/en/reports/instagram/followers/
10. https://www.socialinsider.io/social-media-benchmarks/instagram-stories-benchmarks/
11. https://afftank.com/blog/instagram-statistics/
12. https://backlinko.com/instagram-users/
13. https://eathealthy365.com/how-many-daily-likes-does-instagram-really-get/
14. https://xtendedview.com/instagram-marketing-statistics/
15. https://www.designgurus.io/answers/detail/how-do-you-estimate-capacity-rpsstoragebandwidth-for-a-social-app
16. https://www.theglobalstatistics.com/instagram-global-users-statistics