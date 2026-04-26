# Setup Guide

## 1. Install Docker

Install Docker Desktop and ensure it is running.

## 2. Run n8n

```bash
docker run -it --rm -p 5678:5678 -v ~/.n8n:/home/node/.n8n n8nio/n8n
```

## 3. Import Workflows

Open http://localhost:5678
Import:
workflows/data-processing.json
workflows/webhook-api.json

## 4. Connect Google Sheets

Create Google OAuth credentials
Add credentials in n8n

## 5. Prepare Sheets

Create:

Sales
Dealers
Models
Dashboard_Data

## 6. Activate Workflows

Activate both workflows

## 7. Test API

Visit:

http://localhost:5678/webhook/car-sales-dashboard
