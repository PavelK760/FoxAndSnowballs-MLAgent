<h1 align="center">Fox-and-Snow/DAinGameDev-project  
  
  
### Этот проект являётся проектной работой по курсу АНАЛИЗ ДАННЫХ И ИСКУССТВЕННЫЙ ИНТЕЛЛЕКТ [in GameDev] 2022г. Проект реализован на Unity с использованием приницпов обучения искусственного интеллекта. 
## Суть проекта проста:
- На небольшой трассе в 4 полосы разполагается 14 лисичек, каждая из которых является агентом, обучающимся пересекать дорогу как можно быстрее
- По прямой линии вдоль трассы летят случайным образом генерирующиеся снежки. 
- Задача агентов научиться пересекать трассу так, чтобы не задевать снежки, при том делать это максимально быстро.
- При соприкосновении со снежками, по истечении времени или при пересечении дороги, каждый агент заканчивает свой проход (поколение) и начинает свой путь сначала.
- Награду агенты получают за то, что быстрее пересекают трассу или оказываются ближке к противоположному концу трассы, чем в прошлый проход.
- Каждая секунда промедления штрафуется, вынуждая агенты проходить трассу как можно быстрее. Так же агенты штрафуются за столкновение со снежками или уход с трассы.

## Установка и работа с проектом:
  Проект создавался на версии Unity 3.3.0, рекомендуется использовать эту версию.
  После установки проект уже можно запускать, однако запуск должен производиться через GitHub. 
  Важнейшие файлы находятся в папке Assets, там же находятся и скрипты и папка с результатами обучения. Текстур паки же напротив очень легко удаляются и сновсятся с проекта, не задевая корневой функционал.
  
## Принципы работы ИИ:
  Агент получает следующие параметры вознаграждения:
   - +5 за пересечение дороги
   - +0.05 если текущая пройденная дистанция больше, предыдущей
   - -5 за столкновение со снежком
   - -0.005 если текущая дистанция до цели не изменилась или увеличилась по отношению к предыдущей проверке (каждую секунду) 
  Параметры поведения Агентов:
   - Перемещение (3 возможных варианта: Вперёд, Назад, Без движения)
   - Повороты (3 возможных варианта: Вправо, Влево, Без движения)
    
#### Проект создали:
- Карабанов Павел Александрович
- Довгий Вадим Юрьевич
- РИ210942
