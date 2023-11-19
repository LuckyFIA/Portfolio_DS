# Прогнозирование количества заказов такси на следующий час
[pdf](https://github.com/LuckyFIA/Portfolio_DS/blob/main/Taxi%20Service/taxi_service.pdf) [ipynb](https://github.com/LuckyFIA/Portfolio_DS/blob/main/Taxi%20Service/taxi_service.ipynb)
## Описание проекта
Требуется построить модель способную спрогнозировать количество заказов такси на следующий час, чтобы привлекать больше водителей в период пиковой нагрузки.
## Инструменты
- **python**
- **pandas**
- **numpy**
- **statsmodels**
- **sklearn**
- **lightgbm**
- **matplotlib**
## Вывод
Проведено исследование временного ряда на предмет трендовых и сезонных закономерностей. При помощи  `cross_val_score`  и  `GridSearchCV`  проведено обучение с кросвалидацией для следующих моделей:
 - LinearRegression;
 - RandomForestRegressor;
 - LGBMRegressor.  
 
 На основе метрики RMSE, выявленной при кросвалидации, выбрана лучшая модель -  `LGBMRegressor`, для которой провели финальное тестирование на тестовой выборке.
