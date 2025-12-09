# n8n VPS Setup

Повна конфігурація n8n для розгортання на VPS з використанням Cloudflare Tunnel для безпечного доступу.

## Опис

Ця конфігурація включає:

- **n8n** (v2.0.0) - платформа автоматизації workflow
- **PostgreSQL 15** - база даних для зберігання даних n8n
- **Cloudflared** - Cloudflare Tunnel для безпечного доступу до n8n через HTTPS

## Передумови

- Docker та Docker Compose встановлені на сервері
- Cloudflare Tunnel налаштований та отриманий `TUNNEL_TOKEN`
- Домен налаштований в Cloudflare

## Швидкий старт

1. Перейменуйте `.env.example` на `.env` та введіть свої змінні

2. Запустіть контейнери:

```bash
docker-compose up -d
```
