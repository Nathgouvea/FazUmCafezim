FazUmCafezim — Requisitos do Website (para Cursor)

Objetivo: Criar um site estático de uma única página (one-page) para a marca brasileira FazUmCafezim, usando HTML5 + TailwindCSS + JavaScript vanilla e hospedagem no GitHub Pages. O site deve ser minimalista, moderno, levemente lúdico e escrito inteiramente em Português do Brasil.

⸻

1. Navegação
   • Navbar fixo no topo (position: sticky) com transição de cor ao rolar.
   • À esquerda: logo (SVG ou PNG fornecido).
   • À direita: âncoras suaves (#hero, #sobre, #cafes, #preferencias, #contato).
   • Mobile: botão hamburguer que expande menu vertical.

<header id="navbar" class="fixed top-0 w-full bg-[#F2EAE5]/70 backdrop-blur-lg">
  <!-- Container Flex -->
</header>

⸻

2. Seções (ordem e IDs)

Ordem ID Descrição resumida
1 #hero Banner de boas-vindas em 100 vh, CTA WhatsApp
2 #sobre História e valores da marca + imagem
3 #cafes Grade de cards com cafés em destaque
4 #preferencias Formulário para coletar gostos de café
5 #contato Localização, horário e formulário de contato
6 #footer Rodapé compacto

2.1 Hero (#hero)
• Altura full-screen.
• Fundo cor #F2EAE5 ou imagem hero (imagem fornecida).
• Título <h1> (Playfair Display): “Bem-vindo ao FazUmCafezim”.
• Subtítulo <p> (Inter): frase acolhedora (~12 palavras).
• Botão CTA: “Pedir café no WhatsApp” → link com message template.
• Ícone seta suave para rolar (animação bounce).

2.2 Sobre (#sobre)
• Grid 2 colunas (mobile col-reverse → img abaixo).
• Foto do interior do café / grãos.
• Texto (~120 palavras) reforçando cultura, origem e frescor.
• Destaque “Feito com ️☕ + ♥ desde 2020”.

2.3 Cafés em Destaque (#cafes)
• Título <h2>: “Nossos Cafés”.
• Cards responsivos (Tailwind grid md:grid-cols-3 gap-6).
• Cada card:
• Imagem 1:1 (object-cover, bordas arredondadas).
• Nome (Playfair Display, font-semibold).
• Descrição curta (Inter, 2 linhas).
• Badge opcional “Popular” (verde #819872).
• Botão fantasma “Quero experimentar” que abre WhatsApp com nome do café.
• Placeholder: 6 cafés (Expresso, Coado, Capuccino, Latte, Cold Brew, Mocha).

2.4 Formulário de Preferências (#preferencias)
• Título: “Conte pra gente seu tipo de café!”.
• Campos: 1. Nome (text) 2. Email 3. Tipo de café favorito (select: Expresso, Coado, Capuccino, etc.) 4. Como prefere beber? (checkbox múltiplo ou radios) 5. Mensagem extra (textarea opcional) 6. Checkbox GDPR: “Aceito receber novidades ☕️”
• Botão “Enviar”.
• Integração via Formspree (método POST).

2.5 Contato & Localização (#contato)
• Flex duas colunas (stack mobile):
• Mapa iframe (Google Maps) – Endereço fictício: “Rua dos Cafezais 123, Belo Horizonte – MG”.
• Bloco de horário:

Seg – Sex 08:00–19:00
Sáb 09:00–18:00
Dom Fechado

    •	Formulário rápido (Nome, Email, Mensagem) → Formspree.
    •	Botões icônicos:
    •	WhatsApp (abre chat)
    •	Instagram (link @fazumcafezim)

2.6 Footer (#footer)
• Fundo #503E2D, texto #F2EAE5.
• Direitos autorais © 2025, links pequenos para redes.

⸻

3. Estilo Visual

3.1 Paleta de Cores

Principais (usar mais):
• #F2EAE5 creme claro
• #A78B6C marrom claro
• #503E2D marrom café (texto)

Secundárias (acento – usar com moderação):
• #819872, #917154, #B5C1A1, #E0D0B8, #DEDFCF, #F2E3E2, #E3C0BB

3.2 Tipografia
• Headings: Playfair Display 600-700.
• Corpo: Inter 400-500.
• Tamanhos sugeridos: h1 3xl, h2 2xl, p base.

3.3 Componentes
• Botões Tailwind classes: px-5 py-3 rounded-full font-medium transition.
• Cards: shadow-lg rounded-2xl overflow-hidden hover:scale-[1.02].
• Formulários: inputs border border-[#A78B6C]/40 focus:border-[#A78B6C] rounded-lg px-4 py-2.

3.4 Acessibilidade
• HTML semântico (<main>, <section>…), aria-label em ícones.
• Contraste mínimo AA (preferir texto em #503E2D).
• alt descritivo em todas as imagens.

⸻

4. Funcionalidades

Item Descrição
Smooth Scroll JS scrollIntoView({behavior:"smooth"})
Formulários Uso de Formspree (POST) para email sem backend
WhatsApp CTA https://wa.me/55XXXXXXXXXX?text=...
Menu Mobile Toggle classe hidden via JS
Lazy-load imgs loading="lazy"

⸻

5. Estrutura de Arquivos

└── fazumcafezim/
├── index.html
├── assets/
│ ├── img/
│ └── icons/
├── css/
│ └── style.css (se necessário customizar além do Tailwind)
└── README.md (como fazer deploy no GitHub Pages)

⸻

6. Deploy no GitHub Pages
   1. Criar repositório fazumcafezim-site.
   2. Commit inicial com index.html.
   3. Ativar GitHub Pages → branch main, folder /.
   4. Aguardar URL <user>.github.io/fazumcafezim-site.

⸻

7. Observações Finais
   • Todo o conteúdo textual deve estar em pt-BR e em linguagem acolhedora.
   • Evitar jargões técnicos aos usuários.
   • Código comentado para fácil manutenção.
   • Focar em performance (<100 KB CSS, imagens otimizadas WebP).

⸻

Entregáveis: index.html totalmente funcional, arquivos auxiliares e instruções no README.
