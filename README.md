# Ollama-Local-LLM-Chat
Local LLM Chat with free internet search, scraping, memory and many other...


ENGLISH:

Local LLM Chat — Your Local AI Assistant with Tools  (english/russian)
Local LLM Chat is a desktop GUI application for chatting with language models via Ollama.
It runs fully locally, requires no internet (except optional search), and provides built‑in tools: web search, page reading, PDF/text file handling, long‑term memory, and more.

End‑user friendly — download a single executable (or run from source) and use it without a console.

No Python knowledge needed — packaged as one binary for Linux.

Full data control — all requests and files stay on your computer.

✨ Features
💬 Smart Chat
Supports any Ollama model (Llama 3, Mistral, Gemma, LFM2, etc.)

Markdown formatting (code, lists, quotes, links) with syntax highlighting

Collapsible “Thought” blocks for models using <think>

Adaptive UI (dark/light theme, switch on the fly)

🛠 Built‑in Tools (Function Calling)
🌐 Web Search via SearXNG (local metasearch) — finds news, articles, documents

📄 Web Scraping (scrape_url, extract_links, search_page) — extracts text, links, metadata

📁 File Handling – read_file (text files), read_pdf (via pypdf)

🧠 Long‑Term Memory (memory_write/read/delete) — model remembers preferences, facts, corrections

🔌 Simple Ollama Integration
Auto‑detects native tool support per model

Compatibility mode for LFM2 (Liquid) via special tags

Unload models and restart Ollama from the UI

⚡ Performance & Convenience
Streaming responses — text appears gradually, no UI jitter

Stats — time‑to‑first‑token (TTFT), generation speed, token count

History autosave — all dialogs are saved and restored on startup

Edit messages — fix your query or regenerate assistant replies

Export chat to .txt for archiving

🚀 Quick Start
Install Ollama — download from ollama.com and pull a model, e.g.:

bash
ollama pull llama3.2:3b
Install dependencies (Python 3.10+, pip):

bash
pip install pypdf beautifulsoup4 pygments requests pyqt6
Run — download the latest release or clone the repo and execute:

bash
python main.py
Optional — run a local SearXNG instance (default: http://localhost:8080/search) for web search.

Chat! — type a message, attach files (📎), and hit Send.

🛠️ Example Usage
“Find latest space news and save my preference to memory.”
→ Model calls search, returns headlines, then writes to memory.

“Read config.yaml and tell me its settings.”
→ Calls read_file and processes the content.

“Summarise the article at https://example.com/article.”
→ Calls scrape_url, extracts text, and summarises.

⚙️ Technical Details
Language: Python 3.10+

GUI: PyQt6

HTTP: requests, BeautifulSoup4

Code highlighting: Pygments (optional)

PDF: pypdf (optional)

APIs: Ollama (REST), SearXNG (POST/json)

The app auto‑detects native tool support via /api/show. If not available, it falls back to text‑based tool parsing.

📦 License
MIT — free to use, modify, and distribute.

🙏 Credits
Ollama for local LLM execution

SearXNG for private metasearch

PyQt for the GUI framework

⭐ Star the project on GitHub if you find it useful!
Issues and suggestions welcome in Issues.

РУССКИЙ:

Local LLM Chat — ваш локальный AI‑ассистент с инструментами
Local LLM Chat — это десктопное приложение с графическим интерфейсом для общения с языковыми моделями через Ollama.
Работает полностью локально, не требует интернета (кроме опционального поиска) и предлагает встроенные инструменты: веб‑поиск, чтение страниц, работа с PDF и текстовыми файлами, долговременная память и другое.

Для конечного пользователя — скачайте исполняемый файл и пользуйтесь без консоли.

Не требует знания Python — упаковано в один бинарник для Linux.

Полный контроль над данными — всё остаётся на вашем компьютере.

✨ Возможности
💬 Умный чат
Поддержка любых моделей Ollama (Llama 3, Mistral, Gemma, LFM2 и др.)

Markdown‑разметка с подсветкой синтаксиса

Сворачиваемые блоки «Мысли» для моделей с <think>

Тёмная/светлая тема, переключение на лету

🛠 Встроенные инструменты (Function Calling)
🌐 Поиск в интернете через SearXNG (локальный метапоиск)

📄 Чтение веб‑страниц (scrape_url, extract_links, search_page)

📁 Работа с файлами – read_file (текстовые), read_pdf (через pypdf)

🧠 Долговременная память (memory_write/read/delete) — модель запоминает предпочтения, факты, исправления

🔌 Простая интеграция с Ollama
Автоопределение нативной поддержки инструментов у модели

Режим совместимости для LFM2 (Liquid)

Выгрузка модели и перезапуск Ollama из интерфейса

⚡ Производительность и удобство
Стриминг ответов — текст появляется постепенно

Статистика — TTFT, скорость, количество токенов

Автосохранение истории — диалоги восстанавливаются при запуске

Редактирование сообщений и регенерация ответа

Экспорт чата в .txt

🚀 Быстрый старт
Установите Ollama — скачайте с ollama.com и загрузите модель, например:

bash
ollama pull llama3.2:3b
Установите зависимости (Python 3.10+, pip):

bash
pip install pypdf beautifulsoup4 pygments requests pyqt6
Запустите — скачайте последний релиз или клонируйте репозиторий и выполните:

bash
python main.py
Опционально — запустите локальный SearXNG (по умолчанию http://localhost:8080/search) для веб‑поиска.

Общайтесь! — введите сообщение, прикрепите файлы (📎) и нажмите «Отправить».

🛠️ Примеры использования
«Найди последние новости о космосе и сохрани моё предпочтение в память.»
→ Модель выполняет поиск, возвращает заголовки, затем вызывает memory_write.

«Прочитай config.yaml и расскажи, какие там настройки.»
→ Вызывается read_file, содержимое отправляется модели.

«Что написано в статье по ссылке https://example.com/article? Выдели основные тезисы.»
→ Модель вызывает scrape_url, извлекает текст и обрабатывает его.

⚙️ Технические детали
Язык: Python 3.10+

GUI: PyQt6

HTTP: requests, BeautifulSoup4

Подсветка кода: Pygments (опционально)

PDF: pypdf (опционально)

API: Ollama (REST), SearXNG (POST/json)

Приложение автоматически определяет нативную поддержку инструментов через /api/show. Если её нет — включает текстовый fallback (парсинг инструментов из ответа модели).

📦 Лицензия
MIT — разрешено использовать, модифицировать и распространять без ограничений.

🙏 Благодарности
Ollama за локальный запуск LLM

SearXNG за приватный метапоиск

PyQt за отличный GUI‑инструментарий

⭐ Поставьте звёздочку на GitHub, если проект полезен!
Сообщения об ошибках и предложения приветствуются в Issues.


