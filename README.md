# Avelis 4.0 — release candidate

Local-first personal finance planning PWA. Romanian interface. Static deployment via GitHub Pages (/docs). No financial profiles, real transactions, credentials or analytics in this repository. The demo uses fictional data.

## Privacy and recovery
Financial data is encrypted at rest in IndexedDB (AES-GCM 256, PBKDF2 SHA-256 with 600,000 iterations). Decrypted data is available while the vault is unlocked; the hosting origin serves executable application code. No independent security audit has been performed. Export encrypted backups, retain your passphrase, and do not share plaintext profile files. Clearing browser data may delete the vault. GitHub may process standard web access logs as hosting provider. No application telemetry, bank connection, external model API or automatic cross-device sync. Backups can be transferred manually.

## Calculations
Forecasts depend on user-entered assumptions and are not financial advice. Import supports Revolut CSV, Raiffeisen XLSX, and generic RON CSV. Review classifications, file coverage, duplicates and transfer matches. Historical aggregates and individual transaction totals are separate. Nominal-rate equal-payment amortization excludes unentered fees and insurance. The assistant uses deterministic rules, not a general LLM.

## Release status
Release candidate, not independently audited. Regression tests cover simulated UI and calculation logic; real-device Safari/installation, accessibility, encrypted migration and XLSX decompression still require browser/device verification. English localization and automatic cross-device sync are not implemented.
