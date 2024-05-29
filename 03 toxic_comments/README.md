# Определение токсичных комментариев
[HTML](https://github.com/Qeecky/Portfolio/blob/main/03%20toxic_comments/toxic_comments.html) [ipynb](https://github.com/Qeecky/Portfolio/blob/main/03%20toxic_comments/toxic_comments.ipynb)

## Описание проекта
Интернет-магазин запускает новый сервис. Теперь пользователи могут редактировать и дополнять описания товаров, как в вики-сообществах. То есть клиенты предлагают свои правки и комментируют изменения других. Магазину нужен инструмент, который будет искать токсичные комментарии и отправлять их на модерацию.

## Навыки и инструменты
- Python
- sklearn.pipeline.Pipeline
- torch
- transformers
- torch.utils.data.Dataset, DataLoader
- tqdm.notebook
- sklearn.model_selection.train_test_split, GridSearchCV
- sklearn.linear_model.LogisticRegression
- catboost.CatBoostClassifier
- sklearn.metrics.f1_score

## Общий вывод
Я проведел анализ комментариев на токсичность.
Предобработка данным не понадобилась, за исключением переопределения индекса
Для построения эмбеддингов и векторизации текстов я применил BERT, поэтому я написал собсвенный класс, а также цикл для токенизации текстов
Далее я обучил несколько модей:
Получил значние метрики f1-score 0.9461 при кросс-валидации и 0.9452 на тестовой выборке - при кросс валидации такое допустимо. Лучшая модель - логистическая регрессия
