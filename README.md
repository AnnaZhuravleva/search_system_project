# search_system

- Проект простого поисковика по базе данных документов posts.csv
- В репозитории находится готовая к установке библиотека такого поисковика. Документация находится в файле [README.txt](https://github.com/AnnaZhuravleva/search_system_project/blob/main/README.txt)и [docs.json](https://github.com/AnnaZhuravleva/search_system_project/blob/main/search_system/documentation/docs.json).
- Данные хранятся в posts.csv файле (БД), поисковой индекс находится в Elasticsearch cloud (в пробной демоверсии данные хранятся до 16/02/2021). К сожалению, из-за нехватки памяти мне не удалось развернуть Elasticsearch на локальном ПК, поэтому я воспользовалась облачной версией базы данных. (Использовать облачную базу данных не очень хорошо, но другого ПК у меня нет и память освободить невозможно). С локального ПК также не удалось подключиться к облачной БД (выскакивала ошибка Connection Error, найти способ исправить которую мне не удалось, что тоже плохо). Однако я воспользовалась [Google Colab](https://colab.research.google.com/drive/1E0yF11tYLqNP1YKX2qmGFZqQHjb5_Qgd?usp=sharing), где все хорошо подключалось, - там реализована рабочая версия программы, которая отличается от данной библиотеки лишь парой деталей, при помощи которых я подключала Flask в Google Colab. Она спокойно подключается к облачной базе данных и находит документ по запросу.
- Для установки библиотеки необходимо скачать исходные файлы или [установочный пакет](https://github.com/AnnaZhuravleva/search_system_project/blob/main/dist/search_system-1.0.tar.gz), перейти в папку search_system и из командной строки запустить установку. 
```
>>> python3 setup.py install --user
```
- Пример запуска поисковика
```
>>> import search_system
>>> search_system.start()
```
После выполнения данной команды нужно открыть localhost http://127.0.0.1:5000/ и ввести запрос в окно поиска.
