# Offline-First and Synchronization Blueprint

The Android app remains useful without an active connection.

## Flow
```text
User action → Room/local transaction → Sync queue → Network restored → API → validation → conflict handling → acknowledgement → local reconciliation
```

Use Room for local data and WorkManager for reliable background synchronization. Operations must be retry-safe and idempotent.

Test airplane mode, intermittent connection, Wi-Fi/mobile transitions, process death, restart, duplicate retry, stale records, failed uploads and concurrent edits.

Show `Synced`, `Offline`, `Pending`, `Syncing`, or `Sync failed` to users.
