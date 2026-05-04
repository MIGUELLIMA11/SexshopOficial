# 🔥 Chama Viva

> **Atividade de UX | Faculdade**  
> Primeira dobra (first fold) de um site para o tema: **Sexshop para Idosos (60+)**

---

## 📋 Sobre o Projeto

O **Chama Viva** é um protótipo de landing page desenvolvido como atividade prática da disciplina de UX. O desafio era criar a **primeira dobra** de um site para um dos temas propostos, justificando as decisões de design com base em persona, acessibilidade e boas práticas de UX.

**Tema escolhido:** Sexshop para o público 60+  
**Abordagem:** Quebrar o tabu com humor respeitoso, linguagem clara e design totalmente acessível para a terceira idade.

---

## 🎯 Decisões de Design

### 🔤 Tipografia
| Fonte | Uso | Justificativa |
|-------|-----|---------------|
| **Playfair Display** | Títulos e headings | Serif elegante, associada à maturidade e sofisticação. O italic no H1 adiciona personalidade sem perder seriedade |
| **Inter** | Corpo do texto | Alta legibilidade em telas, formas abertas, excelente para usuários 60+ com base de 18px |

### 🎨 Paleta de Cores
| Token | Hex | Uso | Justificativa |
|-------|-----|-----|---------------|
| Terracota | `#b55a3a` | Principal / ações | Tom quente e acolhedor, associado à maturidade e vitalidade. Diferente do rosa clichê do setor — passa seriedade |
| Verde-musgo | `#4a6741` | Secundária / confiança | Remete à saúde e equilíbrio. Usado em badges e botão de atendimento |
| Creme | `#fdf7f2` | Fundo | Reduz fadiga ocular comparado ao branco puro — ideal para 60+ |
| Tinta | `#261a14` | Texto | Marrom-escuro (não preto puro) — menos agressivo, mas contraste WCAG AA mantido |

### 📝 Conteúdo
- **Headline com humor:** *"A aposentadoria foi só o começo."* — convida sem embaraçar
- **Subheadline honesta:** Diz explicitamente que o site foi feito para o público 60+, com letras grandes, sem enrolação e consultora de verdade
- **Diferenciais em lista:** Responde antecipadamente às objeções mais comuns da persona (vergonha, dificuldade com tecnologia)
- **Card produto destaque:** Ancora com produto concreto e avaliação visível
- **Tom humorístico controlado:** Frases como *"a vizinha vai continuar sem saber"* — leve, nunca sensacionalista

### ♿ Acessibilidade
- **Base 18px** — tamanho acima do padrão para conforto visual da persona
- **Skip-link** — pula o header, essencial para usuários de teclado e leitores de tela
- **Foco visível** — outline de 3px em terracota em todos os elementos interativos (`*:focus-visible`)
- **Landmarks semânticos** — `<header>`, `<main>`, `<footer>`, `aria-labelledby` em todas as seções
- **WCAG AA** — Tinta sobre creme = ratio ~14:1 | Botões brancos sobre terracota = ~4.6:1
- **Botões grandes** — `min-height: 52px` para quem tem motricidade reduzida
- **Responsivo** — colapsa para coluna única em telas ≤ 820px

---

## 🗂️ Estrutura do Projeto

```
📁 Ux - Atividade/
├── 📄 index.html          # Página principal (primeira dobra)
├── 🎨 styles.css          # Estilos — tokens, componentes, responsivo
├── 📝 justificativa.md    # Justificativa detalhada das escolhas de UX
└── 📖 README.md           # Este arquivo
```

---

## 🧱 Estrutura da Página

```
┌─────────────────────────────────────┐
│  HEADER — topbar sticky             │
│  Logo | Nav | Botão Consultora      │
├─────────────────────────────────────┤
│  HERO — primeira dobra              │
│  ┌────────────────┬───────────────┐ │
│  │  copy          │  card produto │ │
│  │  pill badge    │  destaque     │ │
│  │  H1 + subtítulo│  avaliação    │ │
│  │  diferenciais  │  CTA          │ │
│  │  CTAs + selos  │               │ │
│  └────────────────┴───────────────┘ │
├─────────────────────────────────────┤
│  FAIXA — garantias (trust strip)    │
├─────────────────────────────────────┤
│  COLEÇÕES — 3 cards                 │
├─────────────────────────────────────┤
│  COMO FUNCIONA — 3 passos           │
├─────────────────────────────────────┤
│  DEPOIMENTO — citação destaque      │
├─────────────────────────────────────┤
│  FOOTER                             │
└─────────────────────────────────────┘
```

---

## 🚀 Como visualizar

Basta abrir o `index.html` diretamente no navegador — sem dependências, sem build, sem frameworks.

```bash
# Opção 1: abre direto
start index.html

# Opção 2: VS Code com Live Server
code .
```

---

## 👤 Persona

**Nome:** Dona Sônia, 68 anos  
**Perfil:** Aposentada, usa celular para WhatsApp e notícias. Considera o tema tabu mas tem curiosidade. Desconfia de sites genéricos que não falam a língua dela. Prefere atendimento humano a chatbot.

**Dores:**
- Sites do setor são jovens demais, font minúscula, linguagem explícita
- Medo de ser julgada ao comprar
- Dificuldade com navegações complexas

**O que a Chama Viva resolve:**
- Letra grande, linguagem clara e sem siglas
- Embalagem discreta e entrega sigilosa (mencionado 3x na hero)
- Consultora humana por WhatsApp

---

## 🏫 Contexto Acadêmico

**Disciplina:** User Experience (UX)  
**Atividade:** Criar a primeira dobra de um site, justificando as escolhas de fonte, cores, conteúdo e acessibilidade  
**Ferramenta de referência:** Figma / Prototipação  
**Apresentação:** Para a turma, com possível presença de convidados

---

*Desenvolvido por [MIGUELLIMA11](https://github.com/MIGUELLIMA11)*
