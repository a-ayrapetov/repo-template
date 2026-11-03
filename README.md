# tool-name

What it does in one sentence. Read-only: show commands and GET calls only unless stated.

## Run

```
python -m venv .venv
.venv/Scripts/pip install -r requirements.txt
python tool.py --inventory inventory.sample.csv
```

Credentials are prompted at runtime and never stored. Sample data uses RFC 5737 documentation addresses only (192.0.2.0/24, 198.51.100.0/24, 203.0.113.0/24).

## Safety

CI rejects any commit containing a secret (gitleaks) or a private RFC 1918 address.
