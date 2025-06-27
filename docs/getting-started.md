# Быстрый старт

## Аутентификация

```bash
curl -X POST https://api.smarthome.local/auth      -H "Content-Type: application/json"      -d '{"username": "user", "password": "pass"}'
```

Ответ:

```json
{
  "access_token": "eyJhbGciOiJIUzI1NiIsInR5cCI6..."
}
```