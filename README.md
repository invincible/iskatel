# RutubeSearch
## Поисковая система для Rutube (ЦП 2023)

**Идея**: 

Наша команда предлагает решение для точного поиска видео на платформе с помощью комбинированного подхода к обработке текста и вывода релевантного результата через веб-интерфейс на основе Flask. Данное решение устойчиво к ошибкам и опечаткам пользователей.

Технические особенности:

1. Обработка текста:
- YandexSpeller
- RegEx
- transliterate
- pymorphy2
2. Векторный поиск кандидатов (TFIDF, FastText)
3. Многоуровневое ранжирование:
- Алгоритм BM25
- Catboostranker - ранжирование по доп. фичам
4. На выходе релевантный поиск с высокой скоростью

Стек решения: Python, Docker, RAPIDS, Flask, Bootstrap.

## Файлы проекта
[./EDA-final.ipynb](https://github.com/invincible/iskatel/blob/main/EDA-videos2.ipynb) Разведочный анализ данных;

[./rutube_tfidf_comments.ipynb](https://github.com/invincible/iskatel/blob/main/rutube_gpu_tfidf_bm25_CATBOOSTRANKER.ipynb) Код основного решения;

[./bm25_catboost.csv](https://github.com/invincible/iskatel/blob/main/bm25_catboost.csv) Файл с рекомендациями;

Репозиторий вебинтерфейса:
https://github.com/invincible/search_autocomplete
