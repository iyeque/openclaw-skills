# Local System Info examples

## Check readiness before a local workload

```bash
uv run --with psutil skills/local-system-info/sysinfo.py summary
uv run --with psutil skills/local-system-info/sysinfo.py memory
uv run --with psutil skills/local-system-info/sysinfo.py disk
```

## Inspect bounded process pressure

```bash
uv run --with psutil skills/local-system-info/sysinfo.py processes --limit 10
```

Usernames are excluded by default. Use `--include-owners` only when owner attribution is explicitly required.
