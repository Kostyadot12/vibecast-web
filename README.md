# ВайбКаст · Web

Лендинг и личный кабинет для приложения **[ВайбКаст](https://github.com/Kostyadot12/vibecast)** — голосовой диктовки для Mac на русском.

🌐 **Деплой:** GitHub Pages → https://kostyadot12.github.io/vibecast-web/

## Структура

```
.
├── index.html          # главный лендинг
├── pricing.html        # тарифы
├── login.html          # вход
├── register.html       # регистрация
├── account.html        # личный кабинет (требует backend)
└── assets/
    ├── styles.css      # paper/terracotta editorial стиль
    ├── api.js          # клиент к VibeFlow Cloud (auto-detect env)
    └── vibeflow-logo.png
```

## Стиль

Брендинг — paper/terracotta editorial 1-в-1 с дизайн-системой Mac-приложения:
- Палитра: cream-paper `#F3EDE1`, ink `#2A241B`, terracotta `#C2674A` / `#A14E33`, moss `#6B7A4B`, gold `#B98A3E`.
- Шрифты: **Fraunces** (display) + **Public Sans** (body) + **JetBrains Mono** (mono) — через Google Fonts CDN.
- Бренд-эмблема — inline SVG `#vc-mark`: тёмный круг с гравированной waveform и coral-точкой.

## Backend

Кабинет и оплата работают через [VibeFlow Cloud](https://github.com/Kostyadot12/vibecast) backend.
`assets/api.js` авто-детектит окружение:
- `localhost` → `http://localhost:3000`
- иначе → `https://api.vibeflow.app` (placeholder до деплоя)

## Локально

```bash
python3 -m http.server 8080
# → http://localhost:8080
```

## Лицензия

MIT.
