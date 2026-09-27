# tutor-bot

Скелет Telegram-бота на Python 3.11+ (aiogram + Anthropic Claude).

## Требования

- Python 3.11 или новее

## Установка

```bash
python -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate
pip install -r requirements.txt
```

## Настройка

Скопируйте `.env.example` в `.env` и заполните значения:

```bash
cp .env.example .env
```

Переменные окружения:

- `TELEGRAM_TOKEN` — токен Telegram-бота (получить у [@BotFather](https://t.me/BotFather))
- `ANTHROPIC_API_KEY` — ключ Anthropic API
- `CLAUDE_MODEL` — идентификатор модели Claude

## Запуск

```bash
python bot.py
```

## Структура проекта

```
tutor-bot/
├── bot.py             # точка входа бота
├── claude_client.py   # клиент Anthropic Claude API
├── prompts.py         # промпты и шаблоны сообщений
├── storage.py         # хранилище данных
├── tools/             # инструменты обработки DXF/SVG
│   ├── dxf_validator.py
│   ├── dxf_render.py
│   └── svg_gen.py
├── requirements.txt
└── .env.example
```
