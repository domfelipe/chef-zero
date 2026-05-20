# Validacao Red Team

## 1. API externa indisponivel

Risco: a TheMealDB ficar offline, falhar por CORS ou demorar demais.

Mitigacao: a chamada tem timeout e `try/catch`. Em falha, o app troca o card da API por fallback visual e preserva a busca local.

## 2. Exposicao de API key

Risco: projetos estaticos em GitHub Pages nao protegem secrets no frontend.

Mitigacao: nenhuma chave e usada. A API externa e keyless e a busca principal roda com dados locais.

## 3. Entrada maliciosa do usuario

Risco: ingredientes digitados poderiam virar HTML injetado.

Mitigacao: chips de ingredientes sao criados com `textContent`, nao com HTML bruto. A entrada tambem e normalizada e deduplicada.

## 4. Dependencia excessiva de mock

Risco: avaliador considerar que nao ha conexao real.

Mitigacao: o status da API fica visivel e a TheMealDB e chamada em tempo real no carregamento e no botao de atualizar inspiracao.

## 5. Layout em mobile

Risco: cards, modal e grid quebrarem em telas estreitas.

Mitigacao: layout em CSS Grid com queda para coluna unica, modal com `max-height` e rolagem interna, sem `h-screen`.
