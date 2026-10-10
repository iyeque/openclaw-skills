# Security policy

## Scope

This repository contains local OpenClaw skills. Each skill is intentionally bounded and documents whether it reads local data, writes files, executes processes, or sends information to an external service.

## Reporting a vulnerability

Do not disclose sensitive details in a public issue. Use GitHub's private vulnerability reporting if enabled, or contact the maintainer privately through the GitHub profile. Include the affected skill, version, platform, reproduction steps, impact, and a minimal proof of concept.

## Capability boundaries

- Audio Processing is local by default; remote TTS requires an explicit network flag.
- Unified Web Search requires explicit flags for both Tavily network access and local workspace search, and blocks obvious credential-like network queries.
- Device Control uses fixed actions and an application allowlist; it does not run arbitrary shell commands.
- Local System Info is read-only; usernames are excluded unless explicitly requested.
- PDF Reader reads only the user-selected PDF and does not access the network or mutate files.

Please avoid posting credentials, private documents, audio recordings, or personal data in issues or pull requests.
