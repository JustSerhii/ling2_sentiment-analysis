Sentiment Analysis відгуків про ліки
Мета
Розробка системи автоматичної класифікації відгуків користувачів про лікарські засоби за тональністю з використанням BERT fine-tuning.
Задачі
•  Реалізація sentiment analysis на основі попередньо навченої моделі BERT
•  Класифікація відгуків на три категорії: 
a.  Позитивні
b.  Середні
c.  Негативні
Технічна реалізація
Архітектура моделі
•  Базова модель: BERT
•  Додатковий класифікаційний шар для визначення трьох класів
•  Fine-tuning попередньо навченої моделі для специфічної задачі
Параметри навчання
•  Обчислювальна платформа: GPU
•  Оптимізатор: AdamW
•  Scheduler: Linear learning rate schedule
•  Метрики оцінки: Accuracy, F1-score
Розподіл даних
•  Датасет розділено на:
•  Тренувальний набір: дані до 2017 року
•  Тестові набори: 
o  Дані до 2017 року
o  Дані за 2017 рік
•  Оригінальний датасет на kaggle: 
o  https://www.kaggle.com/datasets/jessicali9530/kuc-hackathon-winter-2018/data
Очікувані результати
•  Створення моделі, здатної автоматично визначати тональність відгуків про ліки
•  Досягнення високої точності класифікації на тестових даних
•  Можливість практичного застосування для аналізу нових відгуків

Посилання на використані джерела
Література на яку ми опиралися:
Q. T. Nguyen, T. L. Nguyen, N. H. Luong and Q. H. Ngo, " Tutorials on Sentiment Analysis using Pre-trained Language Models: Fine-tuning BERT"2020 7th NAFOSTED Conference on Information and Computer Science (NICS), Ho Chi Minh City, Vietnam, 2020, pp. 302-307, doi: 10.1109/NICS51282.2020.9335899. keywords: {Deep learning;Computer science;Sentiment analysis;Analytical models;Bit error rate;Neural networks;Task analysis;sentiment analysis;BERT;pre-trained language model;deep learning},

Орієнтир очікуваної точності(тут використано інший спосіб sentiment analysis) на цьому датасеті:
https://www.kaggle.com/code/debanjanpan/drugs-review-sentiment
