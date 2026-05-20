# QA

## Checklist funcional

- [x] App carrega com ingredientes iniciais e receitas ranqueadas
- [x] Usuario adiciona ingredientes separados por virgula
- [x] Ingrediente duplicado gera aviso
- [x] Chips podem ser removidos
- [x] Filtros alternam entre ativo e inativo
- [x] Botao limpar reseta ingredientes e filtros
- [x] Modal de receita abre e fecha por botao, overlay e tecla Escape
- [x] TheMealDB e chamada sem chave
- [x] Fallback aparece se a chamada externa falhar

## Checklist visual

- [x] Layout responsivo em desktop e mobile
- [x] Cards com imagens reais ou fallback visual
- [x] Estados de carregamento para API
- [x] Estado vazio para resultados
- [x] Feedback tactil em botoes
- [x] Tipografia consistente

## Checklist deploy

- [x] `.nojekyll` presente
- [x] Workflow de Pages usa `actions/configure-pages`
- [x] Workflow publica a raiz do repo
- [x] Branch esperada: `main`
