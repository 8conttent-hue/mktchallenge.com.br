# CLAUDE.md — MKTCHALLENGE

Site gerado pelo **SF (Site Factory)** em 15/04/2026.

## Contexto do Site

**Nome:** MKTCHALLENGE
**Nicho:** Marketing Digital
**Keywords:** As jornadas de compra dos clientes nao comecam mais com uma ligacao
**Paleta de cores:** gold | **Fonte:** montserrat

As jornadas de compra dos clientes não começam mais com uma ligação de telefone, mas sim com um clique ou um toque na tela de um smartphone. O mercado atual exige a melhoria de processos operacionais ultrapassados ou mal executados, a criação de novos modelos de negócios e a integração da experiência do cliente por meio da tecnologia. A quarta revolução industrial, com foco em inteligência, tecnologia e dados, já está acontecendo. Tudo isso é realizado através de uma boa estratégia e execução  de um projeto de marketing digital. Vamos criar o seu? Basta me Enviar um E-mail. Sobre As jornadas de compra dos clientes não começam mais com uma ligação de telefone, mas sim com um clique ou um toque na tela de um smartphone. O mercado atual exige a melhoria de processos operacionais ultrapassados ou mal executados, a criação de novos modelos de negócios e a integração da experiência do cliente por meio da tecnologia. A quarta revolução industrial, com foco em inteligência, tecnologia e dados, já está acontecendo. Tudo isso é realizado através de uma boa estratégia e execução  de um projeto de marketing digital.



## Componentes visuais usados

| Seção | Variante |
|-------|----------|
| Header | Header-B |
| Hero | Hero-G |
| Features | Features-I |
| About Section | About-D |
| Posts | Posts-J |
| Footer | Footer-H |
| Página Sobre | Sobre-B |
| Página Contato | Contato-C |

## Estrutura do projeto

```
src/
  sections/        # Layout escolhido pelo SF — Header, Hero, Features, About, Posts, Footer, Sobre, Contato
  data/            # JSONs com todo o conteúdo editável
  content/blog/    # Posts em Markdown
  pages/           # Rotas Astro (index, sobre, contato, blog, privacidade, termos)
  layouts/         # BaseLayout com fonte e cores dinâmicas
  styles/          # global.css com variáveis CSS de cor
public/
  images/          # hero.jpg, about.jpg, blog/*.jpg — inseridos automaticamente via Pexels
```

## O que editar

### Textos e conteúdo
- **`src/data/home.json`** — hero (título, subtítulo, botão), features (título, items), about section (título, desc, stats), posts
- **`src/data/sobre.json`** — conteúdo completo da página Sobre (hero, texto, missão)
- **`src/data/contato.json`** — título, subtítulo, email, tempo de resposta
- **`src/data/siteConfig.json`** — nome, slug, email, redes sociais, menu

### Imagens
Imagens já estão em `public/images/` (via Pexels). Para substituir, mantenha os mesmos nomes de arquivo:
- `hero.jpg` — imagem de fundo do Hero
- `about.jpg` — imagem da seção About (home)
- `sobre.jpg` — imagem de fundo da página Sobre
- `blog/{slug}.jpg` — imagens dos posts

### Posts do blog
Arquivos em `src/content/blog/`. Ajuste o tom de voz, adicione dados específicos do nicho e personalize conforme a identidade do site.

### Cores
Variáveis em `src/styles/global.css`: `--color-primary`, `--color-accent`, `--color-dark`.

## Deploy

```bash
bun install
bun run build
# Faça upload da pasta dist/ para Netlify, Vercel ou hosting estático
```
