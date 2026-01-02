# Direct Message Integration Update

**Version:** 2.5.10  
**Module:** DM Integration

---

## Objective

Enable secure, user-initiated direct messaging while respecting user privacy settings and Discord permission restrictions.

---

## New Features (v2.5.10)

### Direct Message Integration
- Detects explicit user requests for direct messages (e.g., “dm me”)
- Initiates a private DM session when permissions allow
- Handles disabled or blocked DMs gracefully
- Provides user feedback instead of failing silently
- Ensures DMs are only sent when explicitly requested

---

## Version 2.5 Update — 2.5.10

### Added: Direct Message Handling

This update introduces controlled DM functionality that:
- Responds only to clear user intent
- Attempts to open a direct message channel with the user
- Falls back to a public response if DMs are disabled
- Maintains compliance with Discord’s privacy and permission model

---

## Patch Notes

### v2.5.10 — DM Integration

#### Features
- Keyword-based detection for DM requests
- Automatic DM initiation with the requesting user
- Exception handling for `discord.Forbidden`
- User-facing notification when DMs cannot be delivered
