# Security policy

This policy applies to every repository in the [cutoptim](https://github.com/cutoptim) organization and to the
CutOptim services they talk to (`cutoptim.com`, `api.cutoptim.com`).

## Reporting a vulnerability

Please **do not open a public issue**. Write to **[security@cutoptim.com](mailto:security@cutoptim.com)** (English or
Hungarian) with the affected repository or URL, the steps to reproduce, and the impact you expect.

Our disclosure policy is on
[cutoptim.com/security](https://cutoptim.com/security#vulnerability-disclosure); the machine-readable contact is
[`/.well-known/security.txt`](https://cutoptim.com/.well-known/security.txt).

## Scope notes

- The SDKs are clients only: they never ship a secret, and an API key belongs in your own environment variables.
- Webhook payloads are signed; verify them with the SDK's `verifyWebhook` before trusting them.
