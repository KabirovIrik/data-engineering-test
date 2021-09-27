# data-engineering-test

## Задание
Собрать 1000 фото людей со следующими свойствами:
- Размер изображения не менее 256х256
- На фото должен быть один человек
- На человеке должны быть очки

## Решение

- Для распознования лиц воспользуемся моделью из библиотеки OpenCV. Модель будет распозновать количество лиц и определять размеры лица с помощью bounded box.
- Для распознования очков тоже воспользуемся OpenCV или другой моделью. Например, моделью https://www.kaggle.com/jorgebuenoperez/computer-vision-application-of-cnn/notebook для соревнования <a href="https://www.kaggle.com/jeffheaton/glasses-or-no-glasses" target="_blank">glasses-or-no-glasses</a>
- Картинки возьмём отсюда https://github.com/NVlabs/ffhq-dataset (для отбора были использованны не все фотографии)

<a href="test.ipynb">Скрипт</a> <br>
<a href="result2/">Фотографии</a> - результат
![image](https://user-images.githubusercontent.com/24974700/134824372-5045d281-c499-4a6e-87ed-91897321c907.png)



## Итог
- Модель распознавания лиц OpenCV плохо выявляет частично скрытые лица
- Модель детектирования очков тоже плохо работает
