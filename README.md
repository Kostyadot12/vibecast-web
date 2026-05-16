# ВайбВиспр · Web

Лендинг и личный кабинет для приложения **[ВайбВиспр](https://github.com/Kostyadot12/vibewispr)** — голосовой диктовки для Mac на русском.

🌐 **Деплой:** GitHub Pages → https://kostyadot12.github.io/vibewispr-web/

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
    ├── api.js          # клиент к VibeWispr Cloud (auto-detect env)
    └── vibewispr-logo.png
```

## Стиль

Брендинг — paper/terracotta editorial 1-в-1 с дизайн-системой Mac-приложения:
- Палитра: cream-paper `#F3EDE1`, ink `#2A241B`, terracotta `#C2674A` / `#A14E33`, moss `#6B7A4B`, gold `#B98A3E`.
- Шрифты: **Fraunces** (display) + **Public Sans** (body) + **JetBrains Mono** (mono) — через Google Fonts CDN.
- Бренд-эмблема — inline SVG `#vc-mark`: тёмный круг с гравированной waveform и coral-точкой.

## Backend

Кабинет и оплата работают через [VibeWispr Cloud](https://github.com/Kostyadot12/vibewispr) backend.
`assets/api.js` авто-детектит окружение:
- `localhost` → `http://localhost:3000`
- иначе → `https://api.vibewispr.ru` (placeholder до деплоя)

## Локально

```bash
python3 -m http.server 8080
# → http://localhost:8080
```

## Лицензия

MIT.
