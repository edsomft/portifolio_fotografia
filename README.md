# Nyx Studio — Portfólio de Fotografia

Trabalho avaliativo de HTML, CSS, Flexbox e CSS Grid — IFCE Campus Aracati, Desenvolvimento Web.

## Tema
Site institucional/portfólio para um estúdio de fotografia autoral (retrato, arquitetura e still life). Proposta visual: minimalista e sofisticada, paleta escura fosca com detalhe em âmbar, cantos arredondados.

## Integrante(s)
- [Seu Nome] — trabalho individual, com fluxo colaborativo simulado (ver seção "Colaboração" abaixo)

## Como executar
Não há build nem dependências. Basta abrir o arquivo `index.html` diretamente no navegador (duplo clique), ou usar uma extensão tipo "Live Server" no VS Code para recarregamento automático.

Estrutura de arquivos:
```
/
├── index.html          → página inicial (home)
├── detalhes.html        → página "Trabalhos"
├── contato.html          → página "Contato"
├── style.css              → CSS único, usado pelas 3 páginas
└── img/                     → imagens do site
```

## Colaboração (fluxo simulado)
Trabalho individual. O fluxo colaborativo (branches + Pull Requests) foi simulado usando duas contas próprias do mesmo estudante:
- **[Nome Conta 1]** ([email-conta-1]) — estrutura HTML, header/hero, responsividade, contato
- **[Nome Conta 2]** ([email-conta-2]) — CSS variables/tema, cards/galeria, animations/float/modal, página de trabalhos

Cada funcionalidade foi desenvolvida em uma branch própria e integrada à `main` via Pull Request.

## Uso de IA generativa
Foi utilizado o Claude (Anthropic) como ferramenta de apoio ao estudo: explicação de propriedades CSS, sugestões de estrutura de código e apoio na organização do fluxo Git com múltiplas contas. Todo o código entregue foi revisado e é compreendido pelo estudante.

## Mapa do checklist técnico

| Requisito | Onde está |
|---|---|
| Flexbox | `style.css` - `.main-nav ul`, `.cards-list`, `.hero`, `.project-detail`, `.contact` |
| CSS Grid | `style.css` - `.gallery-grid`, `.project-detail__grid` |
| Media queries (responsividade) | `style.css` - `@media (max-width: 1024px)`, `@media (max-width: 640px)`, `@media (max-width: 768px)` |
| Media queries (CSS3) | `style.css` - `@media (prefers-reduced-motion: reduce)` |
| CSS Variables | `style.css` - `:root` (`--color-*`, `--space-*`, `--radius-*`) |
| Image modal | `index.html` - `.modal` / `.modal__content` (galeria); `style.css` - `.modal:target` |
| Animations | `style.css` - `@keyframes fadeInUp`, aplicado em `.hero h1`, `.hero p` |
| Backgrounds | `style.css` - `.hero` (`radial-gradient` + cor sólida) |
| CSS Units relativas | `style.css` - `rem`, `%`, `vh`, `vw`, `clamp()` em `h1`, `h2`, `.hero` |
| Pseudo-elements | `style.css` - `.main-nav a::after`, `.about::after` |
| Pseudo-classes | `style.css` - `:hover`, `:focus-visible`, `:target`, `:focus` |
| Float | `index.html` - `.about-img`; `style.css` - `.about-img { float: left }` |
| Position + z-index | `style.css` - `.site-header` (`sticky`), `.modal` (`fixed` + `z-index`) |

## Checklist de páginas
- [x] 3 páginas HTML navegáveis entre si (`index.html`, `detalhes.html`, `contato.html`)
- [x] Cabeçalho/menu, seção de destaque, seções de conteúdo, cards e galeria (home)
- [x] Página de Contato com formulário
- [x] Layout testado em desktop, tablet e mobile