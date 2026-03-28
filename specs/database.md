---
title: "Database"
tags: ["backend", "storage"]
links: ["API Gateway"]
created: 2024-03-28T08:00:00.000Z
modified: 2024-03-28T09:00:00.000Z
---
# Database

## Overview
PostgreSQL with pgvector for embeddings. All reads and writes go through the [[API Gateway]].

## Tables
- `users` — User accounts
- `canvases` — Canvas documents
- `nodes` — Architecture nodes

## Access
The [[Canvas Engine]] reads canvas state from the database via the gateway.

## Migrations
Managed via Supabase CLI.