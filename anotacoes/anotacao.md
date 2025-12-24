# Anotação: LP One Piece — plano de estudos e desenvolvimento

Objetivo

- Criar uma landing page tematizada em One Piece para praticar HTML, CSS e JS.
- Focar em HTML semântico, acessibilidade, SEO e performance.
- Usar técnicas CSS modernas (Flexbox, Grid, custom properties, container queries) e JS para interações acessíveis.

Critérios de aceitação

- Estrutura semântica completa (header, nav, main, sections, footer).
- Navegação totalmente acessível por teclado; contrastes dentro do WCAG AA.
- Lighthouse ≥ 90 em Performance / Accessibility / Best Practices / SEO (meta mínimo).
- Página leve (< 200 KB de assets críticos) e responsiva.

Estrutura sugerida (HTML)

- header: logo, título, nav (links ancorados)
- main
  - hero (h1, CTA)
  - features / diferenciais (section com articles)
  - galeria / destaque (imagens otimizadas)
  - sobre / lore breve (conteúdo temático, sem violar direitos)
  - contato / newsletter (form acessível)
- aside: links relacionados / créditos
- footer: copyright, sitemap, links sociais
- usar landmarks ARIA quando necessário

Acessibilidade (A11Y) — checklist

- Uso correto de headings (h1 → h2 → h3...)
- Textos alternativos descritivos nas imagens; indicar licenciamento das imagens do One Piece
- Foco visível e ordem de tabulação natural
- Roles e aria-labels mínimas e sem excessos
- Componentes interativos acessíveis (botões, formulários, modais)
- Testes com leitor de tela e teclado

SEO — checklist básico

- Title único e descritivo; meta description objetivo
- Headings semânticos e conteúdo indexável
- URLs amigáveis e canônico
- Open Graph e meta para redes sociais
- Sitemap.xml e robots.txt
- Schema.org básico (Organization/BreadcrumbList onde fizer sentido)
- Conteúdo relevante e palavras-chave naturais (evitar keyword stuffing)

Performance — práticas

- Otimizar imagens (WebP/AVIF), usar srcset e lazy-loading
- Inline critical CSS mínimo; carregar restante async/defer
- Minificar CSS/JS e usar compressão (gzip/ brotli)
- Evitar grandes dependências; preferir vanilla JS quando possível
- Pré-carregar fontes essenciais (font-display: swap)

CSS — tópicos a praticar

- Layouts com Grid e Flexbox (ex.: grid para seções, flex para nav)
- Custom properties e temas (variáveis para cores e espaçamentos)
- Técnicas modernas: gap, clamp(), min()/max(), container queries (quando suportado)
- Controle de stacking com z-index; pseudo-elementos ::before/::after
- Metodologias leves (BEM ou utility-first minimal) para manutenção
- Responsividade Mobile First e breakpoints fluidos

JavaScript — interações e boas práticas

- Progressive enhancement: site funcional sem JS
- Menu off-canvas acessível (aria-expanded, trap focus)
- Modais e lightbox acessíveis (focus trap, Esc para fechar)
- Animações sutis com prefers-reduced-motion
- Validação de formulário e feedback acessível
- Lazy-load de componentes ou módulos dinamicamente
- Testes manuais e com Lighthouse/axe

Assets e licença

- Usar imagens/oficiais apenas se houver licença; preferir assets próprios, fan-art livre ou placeholders
- Declarar fonte dos assets no projeto

Ferramentas e workflow

- Git + GitHub; deploy: GitHub Pages / Netlify / Vercel
- Lighthouse, Chrome DevTools, axe-core
- Prettier, ESLint, Stylelint
- Otimizadores: Squoosh, ImageOptim
- CI básico para linting/build

Tarefas iniciais (prioridade)
- [x] Criar repositório e README
- [x] Esboçar wireframe (mobile / desktop)
- [ ] Estrutura HTML semântica base
- [ ] Estilizar layout básico com CSS custom properties + Grid/Flex
- [ ] Implementar nav acessível e hero com CTA
- [ ] Otimizar imagens e rodar Lighthouse
- [ ] Adicionar interações JS (menu, modal, smooth scroll)
- [ ] Testes de acessibilidade e ajustes

Notas rápidas

- Priorizar conteúdo e acessibilidade antes de micro-efeitos.
- Documentar decisões (por que usar X ou Y) no README.
- Evitar uso de material protegido sem permissão; prefira assets originais.

Referências rápidas

- MDN (HTML/CSS/JS), WebAIM (acessibilidade), Google Lighthouse, W3C ARIA, Schema.org

Plano de estudo sugerido (2–4 semanas)

- Semana 1: HTML semântico + wireframe + layout base
- Semana 2: CSS moderno (Grid/Flex/vars) + responsividade
- Semana 3: Acessibilidade e SEO on-page + otimização de imagens
- Semana 4: JS para interações + testes e deploy

Fim da anotação — começar implementando o skeleton HTML e o wireframe.

---