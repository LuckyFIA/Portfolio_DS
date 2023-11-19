# Анализ текстов
[pdf](https://github.com/LuckyFIA/Portfolio_DS/blob/main/%D0%A1omments%20%D0%A1lassification/comments_classification.pdf) [ipynb](https://github.com/LuckyFIA/Portfolio_DS/blob/main/%D0%A1omments%20%D0%A1lassification/comments_classification.ipynb)
## Описание проекта
Требуется анализировать комментарии пользователей на английском языке и выделять токсичные, чтобы отправить на модерацию.
## Инструменты
- **python**
- **pandas**
- **numpy**
- **sklearn**
- **lightgbm**
- **catboost**
## Вывод

При помощи нейросети BERT были подготовлены признаки.
Используя  `GridSearchCV`  провели обучение с кросвалидацией для следующих моделей:
-   LogisticRegression;
-   LGBMClassifier;
-   RandomForestClassifier.

На основе метрики F1, выявленной при кросвалидации, выбрана лучшая модель -  `RandomForestClassifier`, для которой проведено финальное тестирование на тестовой выборке:
-   Качество предсказания (F1): 0.958;
-   Время обучения модели: 3.13 сек;
-   Время предсказания модели: 0.019 сек.
