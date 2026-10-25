# Maintenance changes

## 2026-10-25

- Detect filename components above 255 UTF-8 bytes, including multibyte names
  previously missed by character-only length checks. This is a portable heuristic,
  not a guarantee for every filesystem. JSON schema and character counts unchanged.
- Add ASCII, UTF-8, legacy Latin-1, and CLI-redaction regression coverage.
- Preserve historical migration hashes; record new hashes in
  [the dated maintenance receipt](docs/MAINTENANCE_2026-10-25.json).
