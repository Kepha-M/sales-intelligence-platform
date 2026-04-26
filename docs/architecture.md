# Architecture

## Overview
This system automates sales reporting using a lightweight data pipeline.

## Flow

Google Sheets (Sales Data)
        ↓
n8n (Data Processing Workflow)
        ↓
Aggregated Reports
        ↓
Cache (Dashboard_Data Sheet)
        ↓
Webhook API
        ↓
Frontend Dashboard (Lovable)

## Components

- Data Source: Google Sheets
- Automation Engine: n8n
- Cache Layer: Google Sheets
- API Layer: n8n Webhook
- Frontend: Lovable

## Key Design Decisions

- Caching to improve performance
- Separation of processing and API workflows
- JSON-based data exchange