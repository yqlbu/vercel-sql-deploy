# vercel-sql-deploy

## Bootstrap

```bash
./install
```

## Run locally

```bash
./venv/bin/python3 main.py
```
## Deploy

```bash
datasette publish vercel test.db \
  --project=test-sqlite \
  --generate-vercel-json > vercel.json
```
