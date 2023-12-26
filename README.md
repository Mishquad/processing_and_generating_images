# Обработка и генерация изображений ДЗ-2
# Иванов Михаил Витальевич

#### Метрики
True Positive Rate (TPR): 0.9213934804898576
True Negative Rate (TNR): 0.9115961800818554


ChatGPT подсказал несколько интересных идей по поводу аугментаций и подбора порога MSE :)
- изображение "урезано" по бокам слева и справа на 15%, т.к. на фото есть лишние объекты.
- пробовал отражения и центрирование, но не очень помогло в кач-ве. 
- Известная нейросеть (упомянута выше) подсказала, что можно попробовать удалить оттенки RGB, остановился на удалении Green/Blue, Red стал GreyScale.
- Размытие изображения позволило сгладить краевые части пролива и улучшить качество.
- Сложилось впечатление, что в данном случае больше помогли аугментации, направленные на (извиняюсь, если некорректно звучит) модификации существующего изображения (цвета, размытие), нежели изменение позиционирования.


