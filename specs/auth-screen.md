---
title: "Auth Screen"
tags: ["auth", "frontend"]
links: ["API Gateway", "User Profile"]
created: 2024-03-28T08:00:00.000Z
modified: 2024-03-28T09:00:00.000Z
---
# Auth Screen

## Overview
Handles user authentication via Sign in with Apple. Authenticated tokens are forwarded to the [[API Gateway]] for session validation.

## Requirements
- Apple OAuth flow
- Token storage in Keychain
- Session persistence

## Related
Once authenticated, the user lands on their [[User Profile]] page.

## Technical Notes
```swift
func authenticate() async throws {
    let credential = try await appleSignIn()
    await store(credential)
}
```