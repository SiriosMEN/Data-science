# распознавание лиц с помощью ResNet50 
Обучение модели в GPU-тренажёре. В проекте сохранен результат вывода тренажера на экран.
## Описание проекта
Сетевой супермаркет «Хлеб-Соль» внедряет систему компьютерного зрения для обработки фотографий покупателей. Фотофиксация в прикассовой зоне поможет определять возраст клиентов, чтобы:
Анализировать покупки и предлагать товары, которые могут заинтересовать покупателей этой возрастной группы;
Контролировать добросовестность кассиров при продаже алкоголя.
### Построена модель, которая по фотографии определит приблизительный возраст человека. 
Используется набор фотографий людей с указанием возраста.
### Использованные фреймворки:
* Pandas
* TensorFlow.Keras
* Matplotlib.pyplot

### Использованные библиотеки:
* ImageDataGenerator
* Keras.models.Sequential
* Keras.layers.Conv2D, AveragePooling2D, Flatten, Dense
* Keras.optimizers.Adam

### Метрики
* MAE
* RMSE

### Из интересного:
Использованы предобученные веса сети imagenet
