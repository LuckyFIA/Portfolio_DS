# Построение модели определения стоимости автомобиля
[pdf](https://github.com/LuckyFIA/Portfolio_DS/blob/main/Determining%20Cost%20Cars/determining_cost_cars.pdf) [ipynb](https://github.com/LuckyFIA/Portfolio_DS/blob/main/Determining%20Cost%20Cars/determining_cost_cars.ipynb)
## Описание проекта
На основе исторических данных необходимо построить модель для определения стоимости автомобиля
## Инструменты
- **python**
- **pandas**
- **seaborn**
- **sklearn**
- **lightgbm**
- **catboost** 
## Вывод
Исследование проводилось для трех моделей: `RandomForestRegressor`, `LGBMRegressor`, `CatBoostRegressor`.  
В результате при помощи `GridSearchCV` были подобраны оптимальные параметры, проведено обучение моделей а так же проанализирована скорость работы и качество моделей.  
