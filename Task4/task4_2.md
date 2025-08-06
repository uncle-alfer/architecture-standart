# 2. Крупные задачи по системам

| Система / команда | Крупные таски |
| ----------------- | ------------- |
| **Rate-Service** | • Добавить публикацию события `RateUpdated` (если ещё не сделано).<br>• Расширить CI/CD: контрактное тестирование события. |
| **Rate-Distribution Service** (новая) | • Проектирование, разработка и деплой в k8s.<br>• PostgreSQL schema + миграции.<br>• Kafka consumer + REST API + FileExport job.<br>• Метрики Prometheus + алерты.<br>• Тесты (unit 70 %, интеграция > 50 %). |
| **Система кол-центра (банк)** | • REST-endpoint `/rates` (bulk upsert).<br>• Изменения БД: таблица _rates_.<br>• Обновление UI карточки клиента.<br>• Ограничения RBAC (только чтение). |
| **Партнёрский кол-центр** | • Подготовить SFTP-пользователя (банк).<br>• Импорт CSV (парсер, валидация).<br>• Загрузка по расписанию (cron). |
| **Infra / DevOps** | • Развёртывание SFTP-шлюза (active-passive).<br>• Helm-чарты Rate-Distribution.<br>• Grafana дашборд + Alertmanager.<br>• Резервное копирование PostgreSQL. |
