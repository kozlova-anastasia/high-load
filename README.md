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
4. Пописки
5. Публикация историй
6. Просмотр историй

## 1.4 Метрики

| Метрика | Значение | Описание |
| :--- | :--- | :--- |
| MAU | 3 млрд [[2]](https://www.statista.com/statistics/272014/global-social-networks-ranked-by-number-of-users/) | Количество пользователей в месяц |
| DAU | 500 млн [[3]](https://www.demandsage.com/instagram-statistics/) | Количество пользователей в день |
| Посты в месяц | 17 шт [[4]](https://buffer.com/resources/instagram-engagement-rate/) | Среднее кол-во публикаций в месяц |
| Тип публикуемого контента | 5.3 - фото, 2.4 - карусель, 2.3 - reels [[5]](https://metricool.com/instagram-research-study-2023/) | Распределение контента на 10 публикаций |
| Удаление поста через неделю после публикации | 35% [[7]](https://arxiv.org/abs/2008.11317) | Из всех удаленных постов 35% приходятся на первую неделю после публикации |
| Тип контента в stories | 57% фото, 43% видео [[10]](https://www.socialinsider.io/social-media-benchmarks/instagram-stories-benchmarks/) | Распределение контента в сторис |
| Кол-во подписчиков | 1k - 10k [[9]](https://mention.com/en/reports/instagram/followers/) | Медианное значение кол-ва подписчиков на один аккаунт |

# 2. Расчет нагрузки

## 2.1 Продуктовые метрики
### Итоговая сводная таблица
| Метрика | Значение |
| :--- | :--- |
| MAU | 3 млрд [[2]](https://www.statista.com/statistics/272014/global-social-networks-ranked-by-number-of-users/) |
| DAU | 500 млн [[3]](https://www.demandsage.com/instagram-statistics/) |
| Средний размер хранилища пользователя | 118.42 Гб |
| Среднее количество действий пользователя в день |  |

### Средний размер хранилища пользователя
Исходя из [[2]](https://www.statista.com/statistics/272014/global-social-networks-ranked-by-number-of-users/) и [[3]]( https://www.demandsage.com/instagram-statistics/) посчитаем средний возраст одного аккаунта Instagram
| Год | Число аккаунтов | Разница с предыдущим годом | Возраст |
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
13 \cdot 110 + 12 \cdot 90 + 11 \cdot 170 + 10 \cdot 130 + 9 \cdot 200 + 8 \cdot 300 + 7 \cdot 100 + 6 \cdot 200 + 5 \cdot 700 + 4 \cdot 300 + 3 \cdot 100 + 1 \cdot 600
}{
3000
} = 5.793
$$

Найдем средний объем данных для пользователя:
| Тип данных | Среднее кол-во в месяц, шт | Размер 1 единицы | Средний срок хранения (лет) | Всего, шт | Всего | Расчет |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| Фото | 9.01 | 1.1 Мб [[6]](https://tinyimagepro.com/blog/compress-photos-for-social-media/) | 5.793 | 626.34 | 688.97 Мб | Кол-во: 17 постов * 0.53 доля постов с фото (раздел 1.4) |
| Видео (reels) | 3.91 | 150 Мб | 5.793 | 271.81 | 40.77 Гб | Кол-во: 17 постов * 0.23 для постов с видео (раздел 1.4) |
| Stories | 17 [[10]](https://www.socialinsider.io/social-media-benchmarks/instagram-stories-benchmarks/) | 65.13 Мб | 5.793 | 1 181.77 | 76.97 Гб | Кол-во Мб: 1.1 Мб * 0.57 + 150 Мб * 0.43 (раздел 1.4) |
| **Итого** |  |  |  | **2 079.92** | **118.42 Гб** |

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