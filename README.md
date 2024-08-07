# Обучение модели классификации комментариев


[ipynb](https://github.com/Alexandra1624/13_classification_of_comments/blob/main/13_classification_of_comments.ipynb)

## Описание проекта

Интернет-магазин запускает новый сервис. Теперь пользователи могут редактировать и дополнять описания товаров, как в вики-сообществах. То есть клиенты предлагают свои правки и комментируют изменения других. Требуется инструмент, который будет искать токсичные комментарии и отправлять их на модерацию.


## Навыки и инструменты

- ![](https://img.shields.io/badge/-Python-bgreen)
- ![](https://img.shields.io/badge/-Pandas-blue)
- ![](https://img.shields.io/badge/-Nympy-B8860B)
- ![](https://img.shields.io/badge/-Scikit--learn-808000)
- ![](https://img.shields.io/badge/-nltk-grey)

## Вывод

Комментарии были очищены от лемматизированы.

Был выявлен дисбаланс классов (почти в 9 раз). Поэтому в модели добавлена строка class_weight='balanced'. Для взвешивания классов.

Обучены 3 модели:

+ Дерево решений
+ Случайный лес
+ Логистическая регрессия
Наилучший результат показала модель Логистическая регрессия. F1-мера = 0.7643600180913613.

На тестовой выборке эта модель показала качество немного хуже. F1-мера = 0.7445323406235459
