# Alloc-PDF-to-text

## Quickstart (Ubuntu)

1. Clone

```bash
git clone <REPO_URL>
cd Alloc-PDF-to-text
```

2. Setup (venv + deps)

```bash
bash setup.sh
```

3. Run (local)

```bash
source alloc-pdf/bin/activate
cd src
uvicorn main:app --host 0.0.0.0 --port 8010 --reload
```

## Docker Image

```bash
docker build -t alloc-pdf:local .
docker run --rm -p 8010:8010 alloc-pdf:local
```

## Docker Compose

This repo does not use docker-compose. Use the `docker build` and `docker run` commands above.
