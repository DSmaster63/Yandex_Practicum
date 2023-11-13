#  Прогнозирование заказов такси
Компания «Чётенькое такси» собрала исторические данные о заказах такси в аэропортах. 
____
**Описание данных:** Данные лежат в файле `taxi.csv`. Количество заказов находится в столбце `num_orders` (от англ. *number of orders*, «число заказов»).
____
**Цель:** Чтобы привлекать больше водителей в период пиковой нагрузки, нужно спрогнозировать количество заказов такси на следующий час.
____
**Задача:** Построить модель для такого предсказания. Для этого нужно:

1. Загрузить данные и выполнить их ресемплирование по одному часу.
2. Проанализировать данные.
3. Обучить разные модели с различными гиперпараметрами. Сделать тестовую выборку размером 10% от исходных данных.
4. Проверить данные на тестовой выборке и сделать выводы.
____
**Используемые инструменты:**
* функции библиотеки Pandas;
* графики, гистограммы и тепловые карты, доступные в библиотеке matplotlib и seaborn;
* ресемплинг (*resample*), анализ по тренду, сезонности (*statsmodels.tsa.seasonal.seasonal_decompose*) и скользящему среднему(*rolling*);
* функция для добавления дополнительных признаков с целью лучшего прогнозирования при работе с временными рядами; 
* функции и модели библиотеки sklearn для работы с данными и регрессией (train_test_split, DecisionTreeRegressor, RandomForestRegressor, LinearRegression, DummyRegressor);
* бустинговые модели lgbm и catboost;
* подбор оптимальных гиперпараметров моделей с помощью RandomizedSearchCV и TimeSeriesSplit, а также лучшего лага и окна скользящего среднего;
* проверка модели на адеквантость с помощью константной модели DummyRegressor