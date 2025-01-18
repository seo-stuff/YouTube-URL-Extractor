# NotebookLM Автоматизация

Набор скриптов для автоматизации работы с источниками в NotebookLM и конвертации данных из Telegram.

## Содержание

- [Описание скриптов](#описание-скриптов)
- [Установка](#установка)
- [Использование](#использование)
- [Требования](#требования)

## Описание скриптов

### notebooklm_urls.py
Скрипт для автоматизации добавления веб-сайтов в качестве источников в NotebookLM.
- Читает URLs из файла urls.txt
- Генерирует JavaScript код для автоматизации добавления источников
- Поддерживает массовое добавление URLs

### notebooklm_youtube.py
Скрипт для автоматизации добавления YouTube видео в качестве источников.
- Извлекает все видео из YouTube канала или плейлиста
- Сохраняет ссылки в отдельный файл
- Генерирует JavaScript код для автоматического добавления видео в NotebookLM

### tg-json-txt.py
Скрипт для конвертации экспортированной истории чата Telegram из JSON в текстовый формат.
- Обрабатывает экспортированный JSON файл из Telegram
- Извлекает текстовые сообщения
- Сохраняет результат в текстовый файл

## Установка

1. Клонируйте репозиторий
```bash
git clone [URL репозитория]
cd [название репозитория]
```

2. Установите зависимости
```bash
pip install yt-dlp
```

## Использование

### Для добавления веб-сайтов:
1. Создайте файл urls.txt и добавьте в него URLs (по одному на строку)
2. Запустите скрипт:
```bash
python notebooklm_urls.py
```
3. Используйте сгенерированный файл url_automation.js в консоли браузера на странице NotebookLM

### Для добавления YouTube видео:
1. Запустите скрипт:
```bash
python notebooklm_youtube.py
```
2. Введите URL YouTube канала или плейлиста
3. Используйте сгенерированный файл youtube_automation.js в консоли браузера

### Для конвертации Telegram истории:
1. Экспортируйте историю чата из Telegram в формате JSON
2. Переименуйте файл в result.json
3. Запустите скрипт:
```bash
python tg-json-txt.py
```

## Требования
- Python 3.6+
- yt-dlp (для работы с YouTube)
- Доступ к NotebookLM
- Современный веб-браузер с поддержкой JavaScript

## Автор
- **Иван Зимин**
  - YouTube: Иван Зимин | SEO (@seo_stuff)
  - Telegram: Иван Зимин | SEO (@heymoneymaker)
