# Data storage

## Confirmed direction

- LocalStorage: user preferences and lightweight configuration.
- IndexedDB through Dexie.js: Bug Briefs records and other structured application data.

## Proposed handling

- Keep data in the current browser profile on the current device.
- Store only fields needed for the approved user flow.
- Define a versioned schema and migration/backup approach before shipping persisted data.
- Handle unavailable storage, quota errors, corrupt records, and interrupted writes without silently discarding user data.
- Make clear when a user action exports data outside browser storage.
- Do not store credentials, API keys, or hosted inference secrets. Hosted inference is out of scope.

## Model artifacts

Model downloads and caches are separate from user records. Their source, storage location, persistence, cache clearing, and offline behavior need an approved design. Model assets may have terms distinct from the runtime package.

**Pending:** schema, retention/deletion behavior, export/import format, migrations, storage limits, model cache location, and corporate data handling standards.

See [security rules](../rules/SECURITY.md).
