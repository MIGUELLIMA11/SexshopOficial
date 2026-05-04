# Justificativa da Primeira Dobra — Chama Viva 🔥

**Tema:** Sexshop para o publico 60+, abordando intimidade e bem-estar com humor respeitoso,
linguagem clara e design acessivel. O nome "Chama Viva" remete a vitalidade e a ideia de que
o prazer nao tem data de validade — quebrando o tabu de forma acolhedora.

---

## Fonte

- **Titulo: Playfair Display (serif, italic)**
  Fonte classica e elegante, associada a maturidade e sofisticacao. O italic no titulo
  ("foi so o *comeco.*") adiciona expressividade e um toque humano sem pieguice.
  Transmite seriedade ao publico 60+, que recebe sites voltados a eles como "para velhinhos".

- **Corpo: Inter (sans-serif)**
  Alta legibilidade em telas, espacamento de letras excelente e formas abertas.
  Escolhida por ser direta, moderna e confortavel de ler, especialmente com o
  tamanho-base de 18 px adotado para acessibilidade.

---

## Cores

- **Terracota (#b55a3a)** — cor principal/acao
  Tom quente e acolhedor que remete a maturidade, terra e vitalidade. Diferente do rosa
  cliche do setor, passa seriedade sem frieza. Contraste AA sobre fundo claro.

- **Verde-musgo (#4a6741)** — cor secundaria/confianca
  Associado a saude, natureza e equiibrio. Usado nos elementos de suporte (badge "online",
  botao de atendimento) para transmitir que o servico e cuidadoso e humano.

- **Creme (#fdf7f2)** — fundo
  Fundo suave, nao-branco, que reduz fadiga ocular. Preferivel ao branco puro para
  publico com maior sensibilidade visual — e transmite aconchego, nao esterilidade.

- **Tinta (#261a14)** — texto
  Marrom-escuro no lugar de preto puro: menos agressivo ao olho, mas com contraste
  suficiente para WCAG AA.

---

## Conteudo

- **Headline com toque humano**: "A aposentadoria foi so o *comeco.*"
  Direta, otimista e com leve ironia — quebra o tabu sem embaracar, convida a continuar lendo.

- **Subheadline honesta**: Explicita que o site foi feito para esse publico, com letras grandes,
  sem enrolacao e consultora de verdade. Isso reduz a desconfianca tipica do usuario 60+.

- **Diferenciais em lista**: Entrega discreta, consultoria humana, acessibilidade de interface.
  Responde antecipadamente as objecoes mais comuns da persona (vergonha, dificuldade com tecnologia).

- **Card produto destaque**: Ancora o usuario com um produto concreto, avaliacao visivel e botao
  claro. Mostra o que esperar sem palavras desnecessarias.

- **Tom humoristico controlado**: Frases como "a vizinha vai continuar sem saber" e
  "a curiosidade da vizinha fica pra ela" trazem leveza sem sensacionalismo — adequado
  para uma apresentacao academica com possivel presenca de convidados.

---

## Acessibilidade

- **Tamanho-base 18 px**: Padrao maior que o habitual (16 px) para conforto visual do publico 60+.
- **Skip-link**: Permite pular o header e ir direto ao conteudo — essencial para usuarios de
  teclado e leitores de tela.
- **Foco visivel** (`*:focus-visible`): Outline de 3 px em terracota em todos os elementos
  interativos — usuarios de teclado sabem onde estao.
- **Aria-labels e landmarks semanticos**: `<header role="banner">`, `<main id="conteudo">`,
  `aria-labelledby` nas secoes, `role="list"` na faixa de garantias, `role="img"` na avaliacao
  de estrelas — estrutura navegavel por leitor de tela.
- **Contraste WCAG AA**: Tinta (#261a14) sobre creme (#fdf7f2) = ratio ~14:1.
  Botoes brancos sobre terracota = ratio ~4.6:1 (passa AA).
- **Botoes grandes** (`min-height: 52px`): Area de clique adequada para quem tem motricidade reduzida.
- **Responsivo**: Layout de duas colunas colapsa para uma coluna em telas menores que 820 px,
  preservando a hierarquia de informacao no celular.
