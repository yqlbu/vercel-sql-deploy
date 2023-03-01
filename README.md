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
# generate config
datasette publish vercel test.db \
  --project=test-sqlite \
  --generate-vercel-json > vercel.json

# deploy with config
datasette publish vercel test.db \
  --project=test-sqlite \
  --vercel-json=vercel.json
```
