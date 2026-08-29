# Odoo 19 Custom Ecosystem & API Documentation

Цей репозиторій містить публічну документацію, специфікації OpenAPI (Swagger) та інструкції з інтеграції для кастомних модулів Odoo 19.

# Odoo 19 Custom Ecosystem & API Documentation

🚀 **[ВІДКРИТИ ІНТЕРАКТИВНИЙ SWAGGER UI](https://berluskuni.github.io/odoo-api-docs/docs/)**

---


## 🗺 Дорожня карта розробки (Roadmap)

- [x] **`core_api_connector`** — REST API для CRM, Каталогу товарів та Замовлень.
- [ ] **`nova_poshta_connector`** — Інтеграція з Новою Поштою (генерація ТТН, трекінг, відділення).
- [ ] **`telegram_bot_notifier`** — Telegram-бот для сповіщень та оперативного управління замовленнями.
- [ ] **`telephony_connector`** — Інтеграція з IP-АТС (Binotel/Ringostat), авто-картка клієнта при дзвінку.
- [ ] **`stock_sync_connector`** — Синхронізація складських залишків із маркетплейсами (Prom, Rozetka).
- [ ] **`prro_tax_connector`** — Автоматична фіскалізація чеків (ПРРО Checkbox / Вчасно).
- [ ] **`payment_gateway_ukraine`** — Еквайринг та авто-звірка платежів (Monobank / LiqPay).



Швидкий старт (Core API Connector)

Базовий URL для локального середовища: `http://localhost:8069/api/v1`

### Авторизація
Усі захищені ендпоінти вимагають заголовок `X-API-KEY`:
```bash
Header: X-API-KEY <your_secret_key>

