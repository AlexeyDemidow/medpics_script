## Cкрипт для автоматического поиска и скачивания медицинских изображений с сайта https://openi.nlm.nih.gov.

---
### Основные этапы:

1. Поиск изображений:
   - Выполнить поиск по ключевым словам на сайте.
   - Собрать ссылки на страницы с результатами поиска.
2. Парсинг статей:
   - Перейти на каждую найденную страницу с результатом.
   - Извлечь ссылку на оригинальную статью.
   - Перейти на страницу оригинальной статьи.
   - Найти ссылки на все изображения внутри статьи.
3. Скачивание изображений:
   - Сохранять изображения в указанную папку на локальном компьютере.
   - Проверять наличие папки и создавать её при необходимости.

---
### Требования:

- Код должен быть структурированным и читаемым.
- Должна быть предусмотрена обработка исключений (например, ошибки сети, неверные URL и т.д.).
- Пользователь должен иметь возможность задавать количество страниц для парсинга и путь для сохранения изображений.

---
Результат:

- Папка с именем в виде номера статьи внутри с медицинскими изображениями, соответствующими введённым ключевым словам.

---
### Установка и запуск

- `git clone ` - клонируем репозиторий
- `pip install -r requirements.txt` - устанавливаем зависимости
- Используется chromedriver.exe версии 125
- Запускаем `main.ipynb`