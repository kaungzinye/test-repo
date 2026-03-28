---
title: "API Gateway"
tags: ["backend", "networking"]
links: ["Auth Screen", "Database"]
created: 2024-03-28T08:00:00.000Z
modified: 2024-03-28T09:00:00.000Z
---
# API Gateway

## Overview
Central routing layer for all API calls. Receives auth tokens from the [[Auth Screen]] and validates sessions.

## Endpoints
- `POST /auth` — Authentication
- `GET /users/:id` — User profile
- `PUT /canvas` — Canvas sync

## Dependencies
Persists all data to the [[Database]]. Serves canvas state to the [[Canvas Engine]] over WebSocket.

## Rate Limiting
100 requests per minute per client.