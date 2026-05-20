# Planejamento

## Produto

ChefZero resolve uma dor comum: decidir o que cozinhar com o que ja existe em casa, reduzindo desperdicio e evitando depender de uma API de receitas paga.

## Publico

Pessoas que cozinham em casa, estudantes, familias pequenas e qualquer usuario que queira economizar tempo e dinheiro antes de comprar mais ingredientes.

## Escopo

- Primeira tela ja e o app funcional.
- Usuario adiciona ingredientes disponiveis.
- App ranqueia receitas locais por encaixe, custo e tempo.
- TheMealDB alimenta a Inspiracao do Dia sem API key.
- Se a API falhar, a experiencia principal continua ativa.

## Stack

- HTML5
- Tailwind CSS via CDN
- JavaScript puro
- Lucide via CDN para icones
- GitHub Pages via GitHub Actions

## Estrategia de dados

O motor principal usa uma base mockada estruturada porque APIs gratuitas de receitas costumam exigir chave para buscas combinadas por ingredientes. A integracao real fica na TheMealDB, que e publica e keyless, mantendo o requisito de conexao com API sem secrets.
