# О проекте

**SmartHome API** — это API-платформа для управления устройствами умного дома.

## Возможности

- Управление освещением, климатом и безопасностью.
- Получение телеметрии с устройств.
- Простое и удобное REST API.

## Статус

- [x] Авторизация
- [x] Управление устройствами
- [ ] Работа с webhooks (в разработке)

## 📊 Диаграмма архитектуры

<div class="mermaid">
flowchart TD
    User -->|Запрос| API[API Gateway]
    API --> Auth{Auth Service}
    API --> Devices[Device Service]
    API --> Telemetry[Telemetry Service]
    Auth -->|Токен| User
</div>

<script>
document.addEventListener("DOMContentLoaded", function() {
  if (window.mermaid) {
    mermaid.initialize({ startOnLoad: true });
  }
});
</script>