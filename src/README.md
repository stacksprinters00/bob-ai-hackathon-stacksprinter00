# Source Code


[services - Copy.py](https://github.com/user-attachments/files/32251674/services.-.Copy.py)

[schemas - Copy.py](https://github.com/user-attachments/files/32251671/schemas.-.Copy.py)

[risk_engine - Copy.py](https://github.com/user-attachments/files/32251668/risk_engine.-.Copy.py)

[mitre - Copy.py](https://github.com/user-attachments/files/32251666/mitre.-.Copy.py)

[main - Copy.py](https://github.com/user-attachments/files/32251663/main.-.Copy.py)

[ingestion - Copy.py](https://github.com/user-attachments/files/32251659/ingestion.-.Copy.py)

[database - Copy.py](https://github.com/user-attachments/files/32251654/database.-.Copy.py)

[correlation - Copy.py](https://github.com/user-attachments/files/32251649/correlation.-.Copy.py)

[config - Copy.py](https://github.com/user-attachments/files/32251646/config.-.Copy.py)

[bluf - Copy.py](https://github.com/user-attachments/files/32251644/bluf.-.Copy.py)
[ai_assistant.py](https://github.com/user-attachments/files/32251643/ai_assistant.py)


## Structure Guidelines

Organize your code logically. Here are common patterns — use whatever fits
your project:

### Web Application
```
src/
  backend/        ← API server code
  frontend/       ← UI code
  shared/         ← Shared utilities/types
```

### Data / AI Project
```
src/
  data/           ← Data ingestion / preprocessing
  models/         ← ML model code
  api/            ← Serving layer
  notebooks/      ← Jupyter notebooks (exploration)
```

### CLI / Script-based Tool
```
src/
  cli/            ← CLI entry points
  lib/            ← Core logic
  utils/          ← Helpers
```

## Important Files to Include

- `requirements.txt` or `package.json` — dependency manifest
- `.env.example` — template for environment variables (NEVER commit `.env`)
- Any database migration files
- Configuration files

## What NOT to Include in src/

- `.env` files with real secrets
- Large binary files (use Git LFS or link externally)
- `node_modules/` or `venv/` (these are in `.gitignore`)
- Build artifacts (`dist/`, `build/`, `__pycache__/`)
