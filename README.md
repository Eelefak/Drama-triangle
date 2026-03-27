# Drama Triangle — Vercel Deployment

## Struktura
```
drama-triangle/
  api/
    chat.js        ← serverless function (proxy do Anthropic API)
  public/
    index.html     ← cała gra
  vercel.json      ← konfiguracja routingu
```

## Wdrożenie — 3 kroki

### 1. Wgraj na GitHub
Utwórz nowe repozytorium i wgraj ten folder.

### 2. Połącz z Vercel
- Wejdź na vercel.com
- "Add New Project" → wybierz repozytorium
- Framework Preset: **Other**
- Root Directory: zostaw puste
- Kliknij Deploy

### 3. Dodaj klucz API
W Vercel → Settings → Environment Variables dodaj:
```
ANTHROPIC_API_KEY = sk-ant-...twój klucz...
```

Potem: Deployments → Redeploy

## Gotowe
Link do gry jest automatycznie generowany przez Vercel.
Możesz go udostępnić komukolwiek.
