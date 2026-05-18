# ✨ Ainda Dá

> **Atividade de UX | Faculdade**  
> Primeira dobra (first fold) de um site para o tema: **Sexshop para Idosos (60+)**

---

## 📋 Sobre o Projeto

O **Ainda Dá** é um protótipo de landing page desenvolvido como atividade prática da disciplina de UX. O desafio era criar a **primeira dobra** de um site para um dos temas propostos, justificando as decisões de design com base em persona, acessibilidade e boas práticas de UX.

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

### ♿ Acessibilidade Técnica (WCAG)
- **Base 18px** — tamanho acima do padrão para conforto visual da persona
- **Skip-link** — pula o header, essencial para usuários de teclado e leitores de tela
- **Foco visível** — outline de 3px em terracota em todos os elementos interativos (`*:focus-visible`)
- **Landmarks semânticos** — `<header>`, `<main>`, `<footer>`, `aria-labelledby` em todas as seções
- **WCAG AA** — Tinta sobre creme = ratio ~14:1 | Botões brancos sobre terracota = ~4.6:1
- **Botões grandes** — `min-height: 52px` para quem tem motricidade reduzida
- **Responsivo** — colapsa para coluna única em telas ≤ 820px

### 🛠️ Recursos de Acessibilidade Interativa (implementados no site)

Além das práticas passivas de WCAG, a página conta com **controles ativos** que a própria usuária opera — sem precisar configurar o navegador ou o sistema operacional.

#### ⚙️ Widget de Ajuda Retrátil
Botão fixo no canto inferior direito, sempre visível. Ao clicar em **"⚙ Ajuda"**, um painel surge acima com quatro opções:

| Botão | Função | Justificativa |
|---|---|---|
| **A+** | Aumenta a fonte em 2px por clique (máx. 28px) | Presbiopia é universal após os 60 — a maioria não sabe aumentar o zoom no navegador |
| **A−** | Diminui a fonte (mín. 16px) | Permite reverter caso o tamanho fique grande demais |
| **◐** | Ativa modo alto contraste (fundo escuro, letras brancas) | Para quem tem sensibilidade à luz ou dificuldade visual severa |
| **✋** | Para todas as animações da página | Vertigem e desorientação causadas por movimento são comuns nesta faixa etária |
| **🔊** | Lê o conteúdo da página em voz alta (Web Speech API, pt-BR) | Para quem tem visão muito reduzida ou simplesmente prefere ouvir; para imediatamente ao clicar de novo |

O painel fecha com **ESC** ou ao clicar no mesmo botão. Ao abrir, o foco vai direto para o `A+` — sem precisar navegar com Tab.

O widget foi posicionado à **direita**, acima do botão de WhatsApp, para não cobrir nenhum conteúdo da página.

#### ↑ Botão Voltar ao Topo
Fixo no canto inferior **esquerdo**, aparece após 400px de scroll. Idosas não sabem rolar de volta ao início — muitas fecham e reabrem o site. O botão some automaticamente quando já estão no topo.

#### 📊 Barra de Progresso de Scroll
Faixa fina em terracota no topo da tela que avança conforme a usuária rola a página. Remove a ansiedade silenciosa de *"quanto falta para acabar?"* — muitas idosas param de explorar por não saber se o conteúdo vai continuar.

#### 💬 Botão WhatsApp Flutuante
Fixo no canto inferior direito, sempre visível, independente da rolagem. Resolve o problema de a usuária não conseguir encontrar de volta o botão de contato após rolar a página. No mobile pequeno exibe só o ícone para não ocupar a tela.

#### 🛡️ Diálogo de Confirmação do WhatsApp
Antes de abrir o aplicativo, um modal explica: *"Você vai abrir o WhatsApp agora — o site vai continuar aberto."* Dois botões grandes: **Sim, abrir o WhatsApp** / **Voltar ao site**. Fecha com ESC ou clique fora do card.

Esta é a adição mais crítica para retenção: o susto de "o site sumiu" ao ser redirecionado para outro app é uma das causas mais comuns de abandono definitivo no público 60+.

#### 🌙 Modo Alto Contraste
Ativado pelo widget, aplica uma paleta invertida via classe CSS no `<body>` — fundo escuro, letras brancas, terracota mais vivo. Não recarrega a página.

### 👵 Acessibilidade Específica para Idosas 60+

A acessibilidade para este público vai além dos critérios WCAG — envolve barreiras **visuais, motoras, cognitivas e emocionais** que se somam.

#### 👁️ Visual
| Decisão | Problema que resolve |
|---|---|
| Fundo creme `#fdf7f2` (não branco puro) | Reduz fadiga ocular causada por presbiopia e sensibilidade à luz — comum após os 60 |
| `line-height: 1.7` no corpo do texto | Texto espaçado compensa a dificuldade de rastrear linhas longas com acuidade reduzida |
| `letter-spacing: 0.01em` nos parágrafos | Pequeno espaçamento entre letras melhora legibilidade para quem tem catarata leve |
| Evitar itálico no corpo do texto | Itálico em corrida é mais difícil de ler com presbiopia — reservado só ao H1 como destaque |

#### 🤚 Motora
| Decisão | Problema que resolve |
|---|---|
| `min-height: 52px` em botões | Alvos de toque generosos para quem tem tremor ou artrite nas mãos |
| Sem interações hover-only | Menus e tooltips que só funcionam com hover excluem usuários de toque (celular) |
| CTA principal alto no hero | Evita rolagem — muitas idosas param de explorar ao não encontrar o botão imediatamente |
| WhatsApp como canal principal | Interface já conhecida e usada no dia a dia; elimina aprendizado de nova ferramenta |

#### 🧠 Cognitiva
| Decisão | Problema que resolve |
|---|---|
| Um único CTA principal por seção | Reduz a paralisia da escolha — múltiplos botões geram ansiedade e abandono |
| Hierarquia clara H1 → subtítulo → lista | Conteúdo escaneável: idosas costumam ler em F-pattern, não linha a linha |
| Linguagem sem siglas ou jargões | Termos como "vibrador" ou "lubrificante" são usados diretamente, sem eufemismos técnicos |
| Diferenciais como lista curta | Blocos de texto corrido têm maior taxa de abandono neste grupo etário |

#### 💬 Emocional / Psicológica
Esta é a camada mais negligenciada — e a mais crítica para o público feminino 60+.

| Decisão | Barreira que remove |
|---|---|
| Consultora **feminina** | Mulheres desta geração têm mais conforto em falar sobre intimidade com outras mulheres |
| "Sem julgamento" explícito no subtítulo | Nomear o medo diretamente diminui sua intensidade — a persona já sente vergonha antes de entrar no site |
| Discreção mencionada **3× na hero** | A preocupação com a opinião de filhos, vizinhos e familiares é real e precisa ser respondida logo |
| Tom de humor leve, nunca explícito | Quebra o tabu sem causar constrangimento — a persona ri antes de sentir vergonha |
| Avaliação de produto visível | Social proof de outras mulheres na mesma faixa etária valida que "não é só eu" |
| Sem imagens sexuais na primeira dobra | O impacto visual imediato determinaria o abandono imediato neste grupo; confiança vem antes |

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
│  Logo | Início · Coleções ·         │
│         Como funciona | Consultora  │
├─────────────────────────────────────┤
│  HERO (#inicio) — primeira dobra    │
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
│  COLEÇÕES (#colecoes) — 3 cards     │
├─────────────────────────────────────┤
│  COMO FUNCIONA (#como-funciona)     │
├─────────────────────────────────────┤
│  DEPOIMENTO — citação destaque      │
├─────────────────────────────────────┤
│  FOOTER                             │
└─────────────────────────────────────┘

  [barra de progresso — topo, fixed]  
  [↑ Voltar ao topo — canto inf. esq] 
  [⚙ Ajuda — canto inferior direito]  
  [💬 WhatsApp — canto inferior direito]
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

**O que a Ainda Dá resolve:**
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
