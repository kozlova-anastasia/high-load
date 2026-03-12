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
| Кол-во постов в неделю | 2 [[14]](https://xtendedview.com/instagram-marketing-statistics/) | Кол-во постов в неделю для аккаунтов с количеством подписчиков < 10 тыс. |

# 2. Расчет нагрузки

## 2.1 Продуктовые метрики
### Сводная таблица
| Метрика | Значение |
| :--- | :--- |
| MAU | 3 млрд [[2]](https://www.statista.com/statistics/272014/global-social-networks-ranked-by-number-of-users/) |
| DAU | 500 млн [[3]](https://www.demandsage.com/instagram-statistics/) |
| Средний размер хранилища пользователя | 39.65 Гб |
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
| Фото | 9.01 | 0.5 Мб | 5.793 | 626.34 | 313.17 Мб | Кол-во: 17 постов * 0.53 доля постов с фото (раздел 1.4) |
| Видео (reels) | 3.91 | 50 Мб | 5.793 | 271.81 | 13.6 Гб | Кол-во: 17 постов * 0.23 для постов с видео (раздел 1.4) |
| Stories | 17 [[10]](https://www.socialinsider.io/social-media-benchmarks/instagram-stories-benchmarks/) | 21.8 Мб | 5.793 | 1181.77 | 25.74 Гб | Кол-во Мб: 0.5 Мб * 0.57 + 50 Мб * 0.43 (раздел 1.4) |
| **Итого** |  |  |  | **2079.92** | **39.65 Гб** |

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
| Хранилище | 118.96 Эб |
| Суммарный суточный трафик | 1353.95 Пб |
| Средняя нагрузка | 125 365 Гбит/с |
| Пиковая нагрузка | 376 095 Гбит/с |
| RPS (средний) | 1 053 819 |
| RPS (пиковый, ×3) | 3 161 457 |

### Хранилище
Для 3 мдрд активных пользователей [[2]](https://www.statista.com/statistics/272014/global-social-networks-ranked-by-number-of-users/)
| Тип данных | Значение для одного пользователя, шт | Значение для одного пользователя | Общее значение, млрд шт | Общее значение, Пб |
| :--- | :--- | :--- | :--- | :--- |
| Фото | 626.34 | 313.17 Мб | 1879.02 | 939.51 | 
| Видео | 271.81 | 13.6 Гб | 815.43 | 40800 |
| Stories | 1181.77 | 25.74 Гб | 3545.31 | 77220 |
| **Итого** |  |  | **6.239 трлн** | **118.96 Эб** |  

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
    <td>17.8</td>
    <td>1648</td>
    <td>4944</td>
    <td>500 млн * 71.19 * 0.5 Мб</td>
  </tr>
  <tr>
    <td>Просмотр Reels</td>
    <td>750</td>
    <td>69 444</td>
    <td>208 322</td>
    <td>500 млн * 30 * 50 Мб</td>
  </tr>
  <tr>
    <td>Просмотр Stories</td>
    <td>576.61</td>
    <td>53 390</td>
    <td>160 170</td>
    <td>500 млн * 52.9 * 21.8 Мб</td>
  </tr>
  <tr>
    <td rowspan="3"><strong>Трафик на загрузку контента</strong></td>
    <td>Публикация фото</td>
    <td>0.075</td>
    <td>6.94</td>
    <td>20.82</td>
    <td>500 млн * 0.3 * 0.5 Мб</td>
  </tr>
  <tr>
    <td>Публикация Reels</td>
    <td>3.25</td>
    <td>300.9</td>
    <td>902.7</td>
    <td>500 млн * 0.13 * 50 Мб</td>
  </tr>
  <tr>
    <td>Просмотр Stories</td>
    <td>6.21</td>
    <td>575</td>
    <td>1725</td>
    <td>500 млн * 0.57 * 21.8 Мб</td>
  </tr>
  <tr>
    <td><strong>Итого</strong></td>
    <td></td>
    <td><strong>1353.95</strong></td>
    <td><strong>125 365</strong></td>
    <td><strong>376 095</strong></td>
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