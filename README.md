# Odoo 19 Custom Ecosystem & API Documentation

Цей репозиторій містить публічну документацію, специфікації OpenAPI (Swagger) та інструкції з інтеграції для кастомних модулів Odoo 19.

## 📦 Модулі в екосистемі

| Модуль | Опис | Статус |
| :--- | :--- | :--- |
| **`core_api_connector`** | REST API ендпоінти для CRM, Каталогу та Замовлень | 🟢 Active |
| **`stock_sync_connector`** | Синхронізація складських залишків | 🟡 Planned |
| **`telegram_bot_notifier`** | Сповіщення про нові замовлення у Telegram | 🟡 Planned |

---

## 🚀 Швидкий старт (Core API Connector)

Базовий URL для локального середовища: `http://localhost:8069/api/v1`

### Авторизація
Усі захищені ендпоінти вимагають заголовок `X-API-KEY`:
```bash
Header: X-API-KEY <your_secret_key>

