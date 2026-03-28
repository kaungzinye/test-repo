---
title: "Canvas Engine"
tags: ["core", "rendering"]
links: ["API Gateway", "Database"]
created: 2024-03-28T08:00:00.000Z
modified: 2024-03-28T09:00:00.000Z
---
# Canvas Engine

## Overview
Core rendering engine for the infinite canvas. Syncs state via the [[API Gateway]] and persists to the [[Database]].

## Architecture
- Metal-backed rendering pipeline
- Loro CRDT for real-time sync
- Gesture recognizers for touch input

## Performance
- 60fps target
- Spatial indexing with R-tree
- Lazy node loading