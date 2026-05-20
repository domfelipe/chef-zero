# ChefZero

ChefZero e um app estatico para encontrar receitas com ingredientes que ja existem em casa. Ele combina um motor local de busca por ingredientes com uma integracao real e sem chave com a API publica TheMealDB para carregar a Inspiracao do Dia.

## Entrega

- App 100% estatico para GitHub Pages
- Busca local com ranking por encaixe, tempo e custo
- Dados mockados ricos para evitar dependencia de API paga
- Integracao keyless com TheMealDB via `fetch`
- Fallback elegante quando a API externa falha
- Workflow GitHub Actions para deploy automatico
- Documentacao das etapas de Planejamento, Execucao, Red Team, QA e Finalizacao

## Deploy

O deploy roda automaticamente a cada `push` na branch `main` usando `.github/workflows/deploy.yml`.

URL esperada:

```text
https://domfelipe.github.io/chef-zero/
```

## Arquivos

```text
.
├── index.html
├── README.md
├── .nojekyll
├── .github/workflows/deploy.yml
└── docs/
    ├── FINALIZACAO.md
    ├── PLANEJAMENTO.md
    ├── QA.md
    └── REDTEAM.md
```

## Desenvolvimento local

```bash
python3 -m http.server 4173
```

Abra `http://localhost:4173`.
