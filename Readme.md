# Инструкция по использованию и запуску Postman - коллекции для работы с issues в GitHub


## Документация по работе с API GitHub issues

[API GitHub issues](https://docs.github.com/en/rest/issues/issues?apiVersion=2022-11-28#about-issues) — один из самых популярных трекеров ошибок в мире. GitHub issues предоставляет владельцам репозитория возможность организовывать, помечать и связывать вопросы с определенными этапами разработки

[Ссылка на репозиторий](https://github.com/HitryDmitry34/4u)

## Методы API GitHub issues, используемые в Postman - коллекции

- Создание вопроса `Create an issue`
- Получение списка вопросов `Get an issue`
- Редактирование вопроса `Update an issue`
- Удаление вопроса  - В документации [REST API](https://docs.github.com/en/rest/issues/issues?apiVersion=2022-11-28#lock-an-issue) отсутствует информация о методе для удаления Issue

## Запуск коллекции в Postman
Обязательное условие для запуска: 

`Получить personal access tokens на GitHub` c необходимыми доступами для работы с репозиторием

`Скачать Postman - коллекцию` [GitHub.postman_collection.json](https://github.com/HitryDmitry34/4u/files/13841046/GitHub.postman_collection.json)

### Настройка авторизации и переменных коллекции
1. Установить для коллекции тип авторизации `Bearer Token`(в названии коллекции Edit->таба Authorization->Type)
2. Вставить personal access tokens в поле `Token`
3. В переменных коллекции указать:
    - `BaseURL` - https://api.github.com
    - `Login` - логин для github
    - `Repo` - название репозитория
    - `issuesN` - оставить пустым (значение будет сгенерировано после выполнения теста)
         
### Запуск коллекции
1. Нажать правой кнопкой на название коллекции
2. Выбрать команду "Run collection"
3. Нажать "Run GitHub"

`Ожидаемый результат:`

![image](https://github.com/HitryDmitry34/4u/assets/142909352/f192c96c-1ff6-4fdb-ac62-50f36ffad1ea)
