# Pixis — Gateway de Pagamentos

Landing page da Pixis em Next.js 14 (App Router) + TypeScript.

## Como rodar localmente

Você precisa ter o **Node.js 18.17+** instalado.
Baixe em: https://nodejs.org

### 1. Instalar dependências

Abra o terminal na pasta do projeto e rode:

```bash
npm install
```

### 2. Rodar em modo desenvolvimento

```bash
npm run dev
```

Acesse: http://localhost:3000

### 3. Build de produção

```bash
npm run build
npm run start
```

## Como hospedar (gratuito) na Vercel

A forma mais rápida de colocar no ar:

1. Crie uma conta em https://vercel.com (pode usar GitHub)
2. Suba esse projeto para o GitHub
3. Na Vercel, clique em "Add New Project" e selecione o repositório
4. Clique em "Deploy" — pronto! Em ~1 minuto está no ar com domínio gratuito

Depois você pode apontar o domínio `pixispay.com.br` para a Vercel
nas configurações do seu registrador (Registro.br, etc).

## Estrutura

```
pixis-nextjs/
├── app/
│   ├── globals.css      # Estilos globais e variáveis
│   ├── layout.tsx       # Layout raiz
│   └── page.tsx         # Página principal
├── components/
│   ├── Navbar.tsx       # Navegação fixa
│   ├── Hero.tsx         # Seção principal com orb 3D
│   ├── Ticker.tsx       # Banner rolante
│   ├── Features.tsx     # Grid de 6 features
│   ├── Stats.tsx        # Números em destaque
│   ├── Segments.tsx     # Tabs interativas (client component)
│   ├── PixUsdt.tsx      # Conversão PIX ↔ USDT
│   ├── CTA.tsx          # Call to action final
│   ├── Footer.tsx       # Rodapé
│   ├── ScrollReveal.tsx # Animações ao rolar
│   └── PixisLogo.tsx    # Logo SVG
├── package.json
├── tsconfig.json
└── next.config.js
```

## Personalização

- **Cores**: edite as variáveis CSS em `app/globals.css`
- **Textos**: cada componente em `/components` tem seu próprio texto
- **Logo**: edite `components/PixisLogo.tsx`
- **Links de contato**: hoje apontam para `#cta` — troque por links reais

## Stack

- Next.js 14 (App Router)
- React 18
- TypeScript
- CSS Modules
- Fonte: DM Sans (Google Fonts)
