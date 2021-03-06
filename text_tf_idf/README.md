## Проект по распознаванию токсичности комментариев на основе технологий TF IDF
Интернет-магазин «Викишоп» запускает новый сервис. Теперь пользователи могут редактировать и дополнять описания товаров, как в вики-сообществах. То есть клиенты предлагают свои правки и комментируют изменения других. Магазину нужен инструмент, который будет искать токсичные комментарии и отправлять их на модерацию.

Обучите модель классифицировать комментарии на позитивные и негативные. В вашем распоряжении набор данных с разметкой о токсичности правок.

Постройте модель со значением метрики качества F1 не меньше 0.75.
### Описание данных
Данные находятся в файле toxic_comments.csv. Столбец text в нём содержит текст комментария, а toxic — целевой признак.
## Подход
Лемматизация и очистка корпуса с комментариями. Обучение моделей на основе известных меток "токсичный/не токсичный".
## Использованные фреймворки
* Pandas
* NLTK
* Sklearn
* Catboost
* LightGBM
## Использованные модели
* Стемматизатор Nltk.WordNetLemmatizer
* LogisticRegression
* RandomForestClassifier
* LGBMClassifier
* CatBoostRegressor
## Метрики
Обучены модели машинного обучения на алгоритмах Логистической регрессии, Случайного леса, CatBoost и LGBM. Наилучшие результаты показала модель LGBM - общая метрика F1 на тесте составила 0,955, при этом предсказания на классе "1" имеют метрику F1 = 0,76.
