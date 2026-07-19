# 👋 Привет! Я Григорий Кожанов (Gregory Kozhanov)

🧠 ML Engineer / NLP Engineer • 16+ лет инженерного опыта  
🌍 Астрахань, Россия — готов к удалённой работе  
✉️ Почта: [astgregory@bk.ru](mailto:astgregory@bk.ru)  
💬 Telegram [@astgregory](https://t.me/astgregory)  
💼 GitHub: [astgregory](https://github.com/astgregory)

---

## О себе

Инженер с сильной инженерной базой и переходом в ML/NLP: 16 лет решал задачи надёжности и воспроизводимости в критически важных системах (РЖД), сейчас применяю этот подход к ML‑пайплайнам и деплою моделей.

Мой фокус — не просто «обучить модель», а сделать решение стабильным и воспроизводимым: от предобработки датасетов и fine‑tuning трансформеров до упаковки в исполняемый файл и интеграции с UI.

Ключевые инженерные принципы в работе:
- **Воспроизводимость**: виртуальные окружения, `.env`, версионирование кода, логирование метрик.
- **Надёжность**: мониторинг, обработка ошибок, стабильность в проде.
- **Измеримость**: всегда фиксирую метрики (perplexity, latency, точность) и делаю выводы.

Английский — B1 (средний), родной язык — русский.

---

## Стек технологий

### ML / Deep Learning
- PyTorch, Hugging Face Transformers
- Fine‑tuning GPT, BERT и BERT‑подобных моделей
- Обучение на CUDA, training loops, callbacks, early stopping
- Оценка качества: perplexity, метрики генерации, ручные оценки

### NLP и RAG
- Text generation, masking, sequence classification
- Document chunking, эмбеддинги, поиск по векторам, RAG‑пайплайны
- Работа с датасетами: WikiText‑2, Google Drive (PDF/TXT), предобработка и токенизация

### Backend, UI, интеграция
- Python, Django, HTMX
- Flutter, Flet (интеграция ML с UI)
- PostgreSQL, MySQL, SQL

### Инструменты и процессы
- Google Colab, PyCharm Pro, Cline
- Linux, virtualenv, .env, Git
- PyInstaller, анализ логов сборки, исправление зависимостей
- Docker (базовый уровень)

---

## Проекты (от наиболее значимых к базовым)

### AIChatFlutter — мультиплатформенный чат с аналитикой и безопасной работой с API

**Задача:** доработать форк `neuro-fill/AIChatFlutter` до уровня готового к использованию приложения: добавить контроль расходов, усилить безопасность API‑ключей, повысить отказоустойчивость.  

**Решение:** внедрил экран статистики и график расходов, реализовал шифрование и валидацию API‑ключей с блокировкой чата до валидации, разделил логику на сервисы (API, БД, аналитика), добавил graceful fallback и таймауты, настроил экспорт данных в JSON.  

**Результат:** приложение стабильно работает на Android, iOS, Windows и Linux; пользователь видит стоимость каждого сообщения и динамику расходов, риск утечки ключей минимизирован.  

**Стек:** Flutter, Dart, Provider, локальное хранилище, HTTP‑клиент.  

🔗 [Репозиторий](https://github.com/astgregory/AIChatFlutter)  
📄 [Инструкция по сборке и запуску](https://github.com/astgregory/AIChatFlutter/blob/main/INSTALL.md)

### RAG‑нейроконсультант по документам (Google Drive)

**Задача:** создать AI‑ассистента для ответов по корпоративным документам.  

**Решение:** RAG‑подход: чанкинг текста, векторизация, поиск по эмбеддингам, генерация ответа. Интеграция с Google Drive API.  

**Результат:** точность ответов по тестовым вопросам — 78–82% (ручная оценка), latency < 1.2 сек.  

**Стек:** Python, PyTorch, transformers, Hugging Face, Google Drive API.  

🔗 [Репозиторий](https://github.com/astgregory/NeuralLabOnGhatGPT)

### PacmanReinforcementLearning — обучение агента RL

**Задача:** обучить агента играть в Pacman с помощью методов reinforcement learning.  

**Решение:** реализована среда, агент, цикл обучения и базовая оценка стратегии.  

**Стек:** Python, Gym/аналоги, PyTorch.  

🔗 [Репозиторий](https://github.com/astgregory/PacmanReinforcementLearning)

### django_htmx — веб‑приложение на Django + HTMX

**Задача:** сделать динамический интерфейс без тяжёлого JS, используя HTMX.  

**Решение:** настроен Django‑проект, добавлены HTMX‑запросы, реализованы CRUD‑операции с минимальной перезагрузкой страницы.  

**Стек:** Django, HTMX, PostgreSQL/MySQL, Docker.  

🔗 [Репозиторий](https://github.com/astgregory/django_htmx)

---

## Образование и курсы

- **Высшее образование:** Ростовский государственный университет путей сообщения, факультет автоматики, телемеханики и связи на железнодорожном транспорте. Специальность: «Автоматика, телемеханика и связь на железнодорожном транспорте» (инженер путей сообщения), 2010.  
- **Профессиональная переподготовка:** «Разработчик нейросетей», ООО «Опора стандарт», 2026. Программа ДПО: Python (ООП), анализ данных, ML, компьютерное зрение, NLP, рекомендательные системы, основы и современные нейронные сети.  
- Сертификат: диплом о прохождении программы ДПО по профессиональной переподготовке «Разработчик нейросетей» (2026).

---

## Опыт и инженерные навыки (перенос из инженерной практики в ML)

Из 16‑летнего опыта в РЖД в ML‑работу напрямую переносятся:
- **Системный поиск причин отказов** → отладка ML‑пайплайнов, разбор ошибок сборки, анализ логов PyInstaller.
- **Контроль параметров и метрик состояния** → мониторинг и observability ML‑сервисов.
- **Документирование изменений и регламенты** → ML Ops, воспроизводимость экспериментов, версионирование.
- **Обеспечение бесперебойной работы** → стабильность и надёжность ML‑сервисов в проде.

---

<b>My GitHub Stats</b>

<a href="http://www.github.com/astgregory"><img src="https://github-readme-stats.vercel.app/api?username=astgregory&show_icons=true&hide=&count_private=true&title_color=3382ed&text_color=22c55e&icon_color=6366f1&bg_color=181824&hide_border=true&show_icons=true" alt="astgregory's GitHub stats" /></a>

<a href="http://www.github.com/astgregory"><img src="https://github-readme-streak-stats.herokuapp.com/?user=astgregory&stroke=22c55e&background=181824&ring=3382ed&fire=3382ed&currStreakNum=22c55e&currStreakLabel=3382ed&sideNums=22c55e&sideLabels=22c55e&dates=22c55e&hide_border=true" /></a>

<a href="https://github.com/astgregory" align="left"><img src="https://github-readme-stats.vercel.app/api/top-langs/?username=astgregory&langs_count=10&title_color=3382ed&text_color=22c55e&icon_color=6366f1&bg_color=181824&hide_border=true&locale=en&custom_title=Top%20%Languages" alt="Top Languages" /></a>

