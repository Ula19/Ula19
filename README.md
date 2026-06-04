<h1 align="center">Hi, I'm Ulugbek 👋</h1>
<h3 align="center">Backend Developer · Python · Async services & Web APIs · From Uzbekistan 🇺🇿</h3>

<p align="center">
  I build production-ready backends — from high-load async Telegram services to REST APIs.
  <br/>
  Started with Python in 2024, currently working as a backend developer and going deep into <b>microservices</b>.
</p>

<p align="center">
  <a href="mailto:Toshev.2000@icloud.com">
    <img src="https://img.shields.io/badge/Email-Toshev.2000@icloud.com-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/>
  </a>
  <a href="https://github.com/Ula19">
    <img src="https://img.shields.io/badge/GitHub-Ula19-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub"/>
  </a>
</p>

---

### 🧑‍💻 About me

- 🛠️ **Backend developer** focused on Python — both **async services** and **web APIs**.
- ⚡ Shipped **40+** real, end-to-end Python projects: async Telegram services backed by PostgreSQL, Docker and external APIs.
- 🌱 Currently learning **microservices** and deepening my knowledge of distributed systems.
- 🐧 Comfortable in **Linux** (daily-driving Kali on a second machine) and deploying apps to a VPS.
- 🧩 I care about clean architecture: layered design, async I/O, migrations, rate-limiting and config via env.

---

### 🧰 Tech Stack

<p align="center">
  <a href="https://skillicons.dev">
    <img src="https://skillicons.dev/icons?i=py,fastapi,django,postgres,redis,docker,nginx,linux,bash,git,github&perline=11" alt="Tech stack icons"/>
  </a>
</p>

<p align="center"><i>Plus, from real projects:</i></p>

<p align="center">
  <img src="https://img.shields.io/badge/aiogram_3-2CA5E0?style=flat-square&logo=telegram&logoColor=white" alt="aiogram 3"/>
  <img src="https://img.shields.io/badge/SQLAlchemy_2_(async)-D71F00?style=flat-square&logo=sqlalchemy&logoColor=white" alt="SQLAlchemy 2"/>
  <img src="https://img.shields.io/badge/Alembic-6BA81E?style=flat-square&logo=alembic&logoColor=white" alt="Alembic"/>
  <img src="https://img.shields.io/badge/Celery-37814A?style=flat-square&logo=celery&logoColor=white" alt="Celery"/>
  <img src="https://img.shields.io/badge/JWT_Auth-000000?style=flat-square&logo=jsonwebtokens&logoColor=white" alt="JWT"/>
  <img src="https://img.shields.io/badge/OpenAPI-6BA539?style=flat-square&logo=openapiinitiative&logoColor=white" alt="OpenAPI"/>
  <img src="https://img.shields.io/badge/Gunicorn-499848?style=flat-square&logo=gunicorn&logoColor=white" alt="Gunicorn"/>
  <img src="https://img.shields.io/badge/FFmpeg-007808?style=flat-square&logo=ffmpeg&logoColor=white" alt="FFmpeg"/>
</p>

---

### 🚀 What I work with

```text
Backend
├── Async services      aiogram 3 · asyncio · long-running workers
├── Web & REST APIs     Django REST Framework · FastAPI · JWT auth · OpenAPI (drf-spectacular)
├── Data layer          PostgreSQL · SQLAlchemy 2 (async / asyncpg) · Alembic migrations · Redis
├── Background jobs      Celery · APScheduler (scheduled digests, periodic tasks)
├── Media processing    FFmpeg · Pillow (transcoding, compression, image ops)
├── Integrations        REST/3rd-party APIs (TMDB, OpenWeatherMap, CoinGecko, Wallhaven, HIBP, ...)
└── Delivery            Docker · Docker Compose · Linux · Nginx · VPS deploy · Git / GitHub Flow
```

---

### 📌 Featured projects

A few projects that show different sides of my backend work — full list is in the [repositories tab](https://github.com/Ula19?tab=repositories).

**🌐 Web backends (REST APIs)**

| Project | What it does | Stack highlights |
| --- | --- | --- |
| [**BIRGA**](https://github.com/Ula19/BIRGA) | Ride-sharing / carpooling REST API — user accounts, trips, in-app chat and reviews | `Django` · `DRF` · `SimpleJWT` · `drf-spectacular (OpenAPI)` · `django-filter` |
| [**marketplace**](https://github.com/Ula19/marketplace) | Multi-vendor e-commerce REST API — sellers, shop, profiles and reviews | `Django` · `DRF` · `async (adrf)` · `JWT` · `PostgreSQL` · `Docker` · `Nginx` · `Gunicorn/Uvicorn` |

**🤖 Async Telegram services**

| Project | What it does | Stack highlights |
| --- | --- | --- |
| [**telegram-youtube-downloader-bot**](https://github.com/Ula19/telegram-youtube-downloader-bot) | YouTube video/Shorts/audio downloader, 144p→4K, 2 GB files, proxy balancing (SOCKS5 ↔ WARP) | `aiogram 3` · `yt-dlp` · `uvloop` · `PostgreSQL` · `Local Bot API` |
| [**telegram-instagram-downloader-bot**](https://github.com/Ula19/telegram-instagram-downloader-bot) | Reels/Stories/posts/IGTV downloader with `file_id` caching (TTL 30d) and multi-protocol proxies | `aiogram 3` · `Cobalt API` · `gallery-dl` · `SQLAlchemy 2` · `pydantic-settings` |
| [**telegram-reddit-downloader-bot**](https://github.com/Ula19/telegram-reddit-downloader-bot) | Reddit media downloader: DASH audio+video merge, galleries, crosspost resolution | `aiogram 3` · `yt-dlp` · `FFmpeg` · `WARP proxy` |
| [**telegram-shazam-downloader-bot**](https://github.com/Ula19/telegram-shazam-downloader-bot) | Recognizes a song from audio/video and returns the track with cover & metadata | `aiogram 3` · `shazamio` · `yt-dlp` · `proxy chain` |
| [**telegram-tempmail-bot**](https://github.com/Ula19/telegram-tempmail-bot) | Disposable emails read inside Telegram; provider-router with automatic failover | `aiogram 3` · `aiohttp` · `mail.tm / guerrillamail` · `PostgreSQL` |

> 🤖 In total my repositories include **40+ Telegram services** across three areas:
> **media downloaders** (YouTube, Instagram, TikTok, VK, Reddit, Pinterest, Twitch, RUTUBE…),
> **media processing** (compress, crop, blur, voice changer, TTS, stickers),
> and **utilities** (QR, PDF tools, exchange rates, temp-mail, weather, passwords).

---

### 🏗️ How I build things

Most of my services follow a consistent, layered structure that keeps logic testable and easy to extend:

```text
handlers/      → routing & user interaction
services/      → business logic (the actual domain work)
middlewares/   → cross-cutting concerns (rate-limit, subscription checks, i18n)
keyboards/     → UI components
database/      → models + CRUD (SQLAlchemy 2, async)
utils/         → helpers, command setup, config
```

Common patterns across projects: **async I/O end-to-end**, **per-user rate limiting**,
**multi-language interfaces** (RU / UZ-Latin / UZ-Cyrillic / EN), **Alembic migrations**,
**env-based configuration**, and **Docker Compose** deployment.

---

### 📊 GitHub Stats

<p align="center">
  <a href="https://github.com/Ula19">
    <img src="https://streak-stats.demolab.com/?user=Ula19&theme=tokyonight&hide_border=true" alt="GitHub streak"/>
  </a>
</p>

---

### 📫 Contact

- **Email:** [Toshev.2000@icloud.com](mailto:Toshev.2000@icloud.com)
- **GitHub:** [@Ula19](https://github.com/Ula19)

<p align="center"><i>Always building, always learning. 🚀</i></p>

