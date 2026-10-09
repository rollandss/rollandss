# Артем Макаренко

<a href="https://rollandss.github.io/uk/"><img src="https://readme-typing-svg.demolab.com?font=Inter&weight=600&size=20&pause=1200&color=E8590C&vCenter=true&width=560&height=32&lines=Full-stack+%D1%80%D0%BE%D0%B7%D1%80%D0%BE%D0%B1%D0%BD%D0%B8%D0%BA+%C2%B7+Next.js%2C+TypeScript%2C+Postgres;SaaS+%D0%BC%D0%BE%D0%BD%D1%96%D1%82%D0%BE%D1%80%D0%B8%D0%BD%D0%B3%D1%83+%D1%86%D1%96%D0%BD+%D0%B4%D0%BB%D1%8F+%D0%BF%D1%80%D0%BE%D0%B4%D0%B0%D0%B2%D1%86%D1%96%D0%B2;%D0%9E%D0%B1%D0%BB%D1%96%D0%BA+%D0%B7%D0%B0%D1%80%D0%BF%D0%BB%D0%B0%D1%82+%D0%B4%D0%BB%D1%8F+%D0%BC%D0%B5%D1%80%D0%B5%D0%B6%D1%96+%D0%BC%D0%B0%D0%B3%D0%B0%D0%B7%D0%B8%D0%BD%D1%96%D0%B2;n8n%2C+Telegram-%D0%B1%D0%BE%D1%82%D0%B8%2C+%D0%B2%D0%BB%D0%B0%D1%81%D0%BD%D0%B0+%D1%96%D0%BD%D1%84%D1%80%D0%B0%D1%81%D1%82%D1%80%D1%83%D0%BA%D1%82%D1%83%D1%80%D0%B0" alt="Full-stack розробник · Next.js, TypeScript, Postgres"></a>

Роблю вебпродукти, якими бізнес користується щодня: моніторинг цін для продавців на маркетплейсах, облік зарплат і приходів для мережі магазинів, систему тестування. Веду їх від ідеї до продакшену, разом із серверною частиною, автоматизацією й власною інфраструктурою.

🌐 [rollandss.github.io](https://rollandss.github.io/uk/) · [English version](README.md)

<p><img src="https://skillicons.dev/icons?i=nextjs,react,ts,tailwind,nodejs,postgres,mongodb,prisma,redis,docker,linux,vercel,git&perline=13" alt="Next.js, React, TypeScript, Tailwind, Node.js, Postgres, MongoDB, Prisma, Redis, Docker, Linux, Vercel, Git"></p>

## Продукти в продакшені

### PriceCortex

<a href="https://www.pricecortex.com"><img src="assets/pricecortex.webp" width="420" alt="PriceCortex screenshot"></a>

B2B SaaS, що відстежує ціни конкурентів на Rozetka та Prom.ua для інтернет-продавців.

- Щоденний збір цін працює в n8n з FlareSolverr на сервері Hetzner
- Тривоги про демпінг, правила ціноутворення й автоперецінка через Seller API маркетплейсу
- AI-пошук аналогів; доступи до Seller API зашифровані AES-256-GCM
- Ролі в команді, тарифи з оплатою через LiqPay, понад 200 unit-тестів для логіки цін і перецінки

**Стек:** Next.js 16, React 19, Tailwind 4, shadcn/ui, Neon Postgres, NextAuth v5, n8n, OpenAI, LiqPay, Vitest  
[Відкрити](https://www.pricecortex.com) · Приватний репозиторій, код на запит

### Oblik Stores

<a href="https://oblik-stores.vercel.app"><img src="assets/oblik-stores.webp" width="420" alt="Oblik Stores screenshot"></a>

Облік для мережі винних магазинів: зарплати, приходи коштів і графіки роботи.

- Зарплата кожного працівника рахується з графіка змін, ставки й бонусів
- Закриття місяця, журнал змін з відновленням, автоматичні резервні копії на пошту
- Відомості на виплату й статистика в Excel; витрати магазинів можна вносити з Telegram-бота
- Тести запускаються під час збірки на Vercel, тож зламаний розрахунок не потрапить у продакшен

_Внутрішній інструмент з реальними даними бізнесу, тому на скріншоті лише сторінка входу._

**Стек:** Next.js 16, Better Auth, Drizzle ORM, Turso, ExcelJS, Resend, Telegram Bot API, Vitest  
[Відкрити](https://oblik-stores.vercel.app) · Приватний репозиторій, код на запит

### Tests System

<a href="https://tests-system-vert.vercel.app"><img src="assets/tests-system.webp" width="420" alt="Tests System screenshot"></a>

Платформа для створення й проходження тестів з ролями для учнів, викладачів і адмінів.

- Випадковий вибір питань, автозбереження прогресу й детальний аналіз результатів
- Імпорт тестів з файлів Word і PDF
- Рейтинг топ-5, чат-кімнати й оголошення
- Rate limiting, валідація вводу, security-заголовки й моніторинг помилок через Sentry

**Стек:** Next.js 16, Prisma, Neon Postgres, Upstash Redis, Sentry, Zod, Brutal UI  
[Відкрити](https://tests-system-vert.vercel.app) · Приватний репозиторій, код на запит

### Birthday Notificator

<a href="https://notificator-lake.vercel.app"><img src="assets/notificator.webp" width="420" alt="Birthday Notificator screenshot"></a>

Нагадування про дні народження в Telegram і на email, налаштовані один раз.

- Спільний бот підключається одним кліком, або можна додати власного Telegram-бота
- Нагадування за 1, 3 чи 7 днів одним дайджестом на день
- Імпорт і експорт CSV, API-ключі для кожного користувача, вибір години сповіщень
- Токени ботів зашифровані AES-256-GCM; повторні виклики cron безпечні

**Стек:** Next.js 16, NextAuth v5, Upstash Redis, Resend, Telegram Bot API, react-hook-form  
[Відкрити](https://notificator-lake.vercel.app) · Приватний репозиторій, код на запит

## Менші проєкти

| | |
|---|---|
| <img src="assets/brutal-ui.webp" width="260" alt="Brutal UI screenshot"> | **Brutal UI**<br>Бібліотека React-компонентів у стилі необруталізму: 39 типізованих компонентів і демо-сайт. Використана в Tests System.<br><sub>React, TypeScript, Tailwind CSS, Next.js</sub><br>[Відкрити](https://brutal-ui-one.vercel.app) · [Код](https://github.com/rollandss/brutal-ui) |
| <img src="assets/training.webp" width="260" alt="Stodenka screenshot"> | **Stodenka**<br>Програма тренувань на турніку на 100 днів: короткий пост на кожен день, лог підходів і повторів, адмінка з редактором постів.<br><sub>Next.js 16, Prisma, Postgres, TipTap, jose</sub><br>[Відкрити](https://training-olive-three.vercel.app) · [Код](https://github.com/rollandss/training) |
| <img src="assets/crm.webp" width="260" alt="Скріншот дашборду CRM"> | **CRM для e-commerce**<br>Замовлення, товари, клієнти й доставка для інтернет-магазину. Підтягує замовлення з Prom.ua і Rozetka, створює відправлення Новою поштою, Укрпоштою й Meest, аналітика продажів, 2FA і журнал дій.<br><sub>Next.js 16, Prisma, Postgres, NextAuth + TOTP, Recharts, Jest</sub><br>Приватний репозиторій, код на запит |
| <img src="assets/mayno.webp" width="260" alt="Скріншот QR-етикеток Mayno"> | **Mayno**<br>Облік обладнання: таблиця з пошуком і фільтрами в URL, друк QR-етикеток, що відкривають картку предмета, історія змін із календарем, вигрузка в Excel.<br><sub>Next.js 16, Prisma, SQLite, Auth.js, TanStack Table, Vitest, Playwright</sub><br>Приватний репозиторій, код на запит |
| <img src="assets/calendar.webp" width="260" alt="Staff Calendar screenshot"> | **Staff Calendar**<br>Перша версія календаря змін для мережі винних магазинів, з нотатками й експортом у PDF. Згодом переросла в Oblik Stores. Імена на скріншоті замінені.<br><sub>Next.js, PDF export</sub> |

## З чим працюю

- **Фронтенд:** React 19, Next.js 16 (App Router, Server Actions), TypeScript, Tailwind CSS, shadcn/ui
- **Бекенд і дані:** Postgres (Neon), MongoDB, Prisma, Drizzle, Turso/libSQL, Redis (Upstash), Zod
- **Авторизація й оплати:** NextAuth v5, Better Auth, JWT, LiqPay
- **Автоматизація:** n8n, Telegram-боти, cron, email через Resend
- **Інфраструктура:** Vercel, Hetzner, Docker, Tailscale, Linux (Arch)
- **Якість:** Vitest, ESLint, Sentry, rate limiting, AES-256-GCM для збережених секретів

## Звʼязатися

[GitHub](https://github.com/rollandss) · [Facebook](https://www.facebook.com/makar.artemenko) · [Instagram](https://www.instagram.com/rollandss05/)

<img src="https://komarev.com/ghpvc/?username=rollandss&label=%D0%9F%D0%B5%D1%80%D0%B5%D0%B3%D0%BB%D1%8F%D0%B4%D0%B8%20%D0%BF%D1%80%D0%BE%D1%84%D1%96%D0%BB%D1%8E&color=e8590c&style=flat" alt="Перегляди профілю">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/rollandss/rollandss/output/github-snake-dark.svg">
  <img alt="Змійка, що зʼїдає мій графік контрибуцій" src="https://raw.githubusercontent.com/rollandss/rollandss/output/github-snake.svg">
</picture>
