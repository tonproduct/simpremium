# Benchmarking Competitivo — Simpremium
**Estudo de concorrentes para embasar o redesign da plataforma**
Abril 2026 | Documento interno

---

## Sobre este documento

Este estudo analisa 5 concorrentes diretos da Simpremium no segmento de chips internacionais para viagem no Brasil. O objetivo é identificar oportunidades concretas de design e UX que fundamentem as decisões do redesign da plataforma.

**Metodologia:** análise direta das interfaces (homepage, páginas de plano, fluxo de compra), complementada por pesquisa de reputação e avaliações de usuários.

**Concorrentes analisados:**
1. AmericaChip — `americachip.com`
2. Nomad Global — `nomadglobal.com`
3. SC Conecta — `scconecta.com.br`
4. O Meu Chip — `omeuchip.com`
5. A Casa do Chip — `acasadochip.com`

---

## Parte 1 — Diagnóstico da Simpremium

Antes de olhar para fora, é necessário entender onde a Simpremium está hoje.

### 1.1 O que funciona

| Ponto positivo | Observação |
|---|---|
| Suporte 24h via WhatsApp | Mencionado em depoimentos como decisivo para a compra |
| Reviews visíveis (4.5★ / 230+ avaliações) | Volume de prova social acima da maioria dos concorrentes |
| Cobertura ampla | 184 países no eSIM, 170+ no chip físico — melhor do grupo |
| Preço competitivo | A partir de USD 1 (eSIM) — mais barato que todos os analisados |
| Número brasileiro mantido | Diferencial emocional importante para o viajante |
| Pré-ativação agendada | Reduz ansiedade pré-viagem |
| Parcelamento em 12x | Facilita ticket maior |

### 1.2 Gaps críticos identificados

**Gap 1 — Taxa de ativação escondida**
A taxa de ativação de USD 5,95 aparece apenas no subtotal do checkout, não durante a seleção de plano. Isso causa surpresa negativa no momento de maior intenção de compra.

> 📍 *Screenshot sugerido: tela de checkout com a taxa aparecendo no subtotal*

**Gap 2 — Seletor de 180+ países sem tratamento**
A seleção de destino é um dropdown com 180+ países em ordem alfabética, sem busca otimizada, sem agrupamento por região, sem destinos populares em destaque. É o primeiro passo do fluxo e já cria atrito.

> 📍 *Screenshot sugerido: dropdown aberto mostrando a extensão da lista*

**Gap 3 — Três modelos de plano sem explicação**
Existem planos com modelos distintos — "ilimitado", "franquia diária" e "franquia total" — para o mesmo destino. A diferença não é explicada na página de seleção; o usuário precisa rolar até o FAQ do rodapé para entender.

> 📍 *Screenshot sugerido: cards de planos para o mesmo destino com modelos diferentes*

**Gap 4 — Página de eSIM sem preços**
A página `/esim/` é uma página informativa sobre compatibilidade de dispositivos. Não exibe preços, planos disponíveis nem CTA de compra. O usuário que chega por busca orgânica por "esim internacional" não consegue converter na página.

> 📍 *Screenshot sugerido: página /esim/ atual vs. página /chip-fisico/ para comparação*

**Gap 5 — Mobile oculta conteúdo de confiança**
O CSS da Simpremium tem `@media screen (max-width: 700px) .infos { display: none }`, o que esconde seções inteiras de conteúdo no celular. Como a maioria dos viajantes pesquisa e compra pelo celular, esse gap afeta diretamente a conversão.

> 📍 *Screenshot sugerido: side-by-side desktop vs. mobile mostrando o conteúdo faltando*

**Gap 6 — Reviews posicionadas no meio-final do scroll**
As avaliações de clientes aparecem tarde na jornada, depois de elementos menos persuasivos. Prova social tem maior impacto quando aparece logo após o hero, enquanto o usuário ainda está formando opinião.

---

## Parte 2 — Análise dos Concorrentes

---

### 2.1 AmericaChip
**`americachip.com`**

**Perfil:** Se posiciona como "a maior empresa de roaming do Brasil". 500.000+ clientes em 5 anos de mercado. Nota 8.2/10 no Reclame Aqui — melhor do segmento.

#### O que fazem bem

**Navegação geográfica como estrutura principal**
O menu principal é organizado por destino (EUA, Europa, Mundi, América do Sul), não por tipo de produto. Isso espelha o modelo mental do viajante: a primeira pergunta é "para onde eu vou?", não "quero chip físico ou eSIM?".

> 📍 *Screenshot sugerido: menu da AmericaChip mostrando a estrutura por destino*

**Preço âncora visível imediatamente**
Cada card de plano exibe "A PARTIR DE: $31,00" em destaque acima do fold. O usuário sabe o custo mínimo antes de clicar, o que reduz o abandono por surpresa de preço.

> 📍 *Screenshot sugerido: card de plano da AmericaChip com preço âncora em destaque*

**3 passos visuais no fluxo de compra**
A página de checkout apresenta uma progressão visual numerada: (1) escolher plano → (2) finalizar pedido → (3) receber. Isso reduz ansiedade em compras de serviço onde o produto não é físico ou imediato.

> 📍 *Screenshot sugerido: seção dos 3 passos da AmericaChip*

**Prova social quantificada**
"500 mil viajantes brasileiros" aparece com destaque na homepage, acompanhado de depoimentos. Não é apenas "clientes satisfeitos" — é um número concreto que transmite autoridade de mercado.

#### O que é fraco
- Não há conversão de preço para BRL em tempo real
- Chip vs. eSIM requer clicar em links separados — sem comparação lado a lado
- FAQ com 12+ itens sem hierarquia visual — informação overload

---

### 2.2 Nomad Global
**`nomadglobal.com`**

**Perfil:** Fintech com ecossistema completo para o viajante brasileiro (conta em dólar, cartão, chip, seguro, investimentos). 3,5 milhões de usuários. App 4.7★ na App Store. É o produto de maior maturidade de UX do grupo — mesmo sendo um produto diferente, é o melhor benchmark de qualidade de design.

#### O que fazem bem

**Conversor de moeda interativo**
A Nomad tem um componente de conversão BRL/USD/EUR em tempo real embutido na página. O usuário digita o valor em reais e vê instantaneamente quanto vai custar em dólar. Isso elimina o maior atrito de precificação do segmento: a ambiguidade cambial.

> 📍 *Screenshot sugerido: componente de conversor da Nomad com inputs bidirecionais*

**Seção de trust consolidada**
Em vez de espalhar selos e números pelo site, a Nomad concentra todos os trust signals em uma seção dedicada antes do rodapé: 3,5M usuários, 4.7★ App Store, 4.5★ Google Play, certificações regulatórias. A concentração amplifica o impacto — o usuário lê tudo de uma vez no momento de maior hesitação (pré-conversão).

> 📍 *Screenshot sugerido: seção de trust da Nomad com todos os indicadores*

**Tipografia com hierarquia rigorosa**
DM Sans 600–700 para títulos (48px), 400 para corpo (18–24px). Ritmo visual consistente com espaçamento de 24–40px entre seções. O resultado é uma página que "respira" e guia o olho sem esforço.

**Gamificação de benefícios (Nomad Pass)**
Um programa de fidelidade que mostra reduções progressivas de taxa — "Ganhe R$ 0,25 OFF" por nível. Conecta ação (comprar) a recompensa mensurável sem parecer artificial. Para um produto de chip recorrente (toda viagem), fidelização é estratégica.

#### O que é fraco
- Chip internacional não tem página própria acessível — está dentro do ecossistema Nomad
- Complexidade do produto (fintech) pode confundir quem quer só um chip

---

### 2.3 SC Conecta
**`scconecta.com.br`**

**Perfil:** Operador especializado com 62.000 linhas ativas e 48.000 clientes. Interface multilíngue (PT/EN/ES). Nota positiva pela feature de date picker — a mais avançada do grupo em termos de fluxo de compra.

#### O que fazem bem

**Date picker integrado ao hero**
Antes de ver qualquer plano, o usuário informa as datas de início e fim da viagem. O sistema então calcula automaticamente o custo total com base na duração selecionada (preço por dia × dias). O resultado: o usuário chega na tela de planos já sabendo exatamente quanto vai pagar pelo período real da sua viagem — sem surpresas.

Detalhes técnicos relevantes:
- Período mínimo de 5 dias
- Ativação gratuita ao meio-dia do dia anterior à viagem
- Cálculo: `preço por dia × número de dias selecionados`

> 📍 *Screenshot sugerido: date picker do SC Conecta no hero + resultado dos planos com preço total calculado*

**Prova social com números concretos e específicos**
Em vez de "clientes satisfeitos", usam: `+120 países`, `+62.000 linhas ativas`, `+48.000 clientes`. A especificidade dos números transmite mais credibilidade do que arredondamentos.

**Reforço de suporte em múltiplos pontos**
"Suporte 24h via WhatsApp" aparece 3 vezes na mesma página — no hero, no card de plano e no footer. A repetição não é redundância: é ancoragem. Para serviços de conectividade onde algo pode dar errado no exterior, o suporte é argumento de venda, não apenas de pós-venda.

#### O que é fraco
- Apenas 3 planos disponíveis — portfólio mais limitado que os concorrentes
- Sem comparação chip físico vs. eSIM na mesma tela

---

### 2.4 O Meu Chip
**`omeuchip.com`**

**Perfil:** Plataforma com foco em Brasil e EUA. Diferencial estratégico de bundle com seguro viagem via Zurich/Universal Assistance.

#### O que fazem bem

**Bundle chip + seguro viagem como diferencial de produto**
Todo plano vem com "SEGURO VIAGEM GRÁTIS" no título do card. O seguro está integrado ao produto, não é um add-on opcional. Isso transforma o chip de commodity em solução completa de viagem — e justifica preço ligeiramente mais alto que concorrentes sem seguro.

> 📍 *Screenshot sugerido: card de plano do O Meu Chip com "SEGURO VIAGEM GRÁTIS" no título*

**Sistema de abas para organizar 3 ofertas**
Chips físicos, eSIM e Seguro Viagem são organizados em abas na mesma página. O usuário não precisa navegar para páginas diferentes — compara tudo em uma única tela. Isso reduz a taxa de abandono por navegação fragmentada.

> 📍 *Screenshot sugerido: sistema de abas do O Meu Chip*

**Navegação geográfica com imagens de fundo**
As seções por destino (EUA, Europa, América do Sul, Global) usam imagens de fundo evocativas de cada região. É mais do que organização — é uma experiência visual que conecta o produto à emoção da viagem.

#### O que é fraco
- Sem conversão de preço para BRL
- Reviews e prova social praticamente ausentes — apenas Instagram feed
- Nota baixa no Reclame Aqui (baixo índice de solução de reclamações)

---

### 2.5 A Casa do Chip
**`acasadochip.com`**

**Perfil:** Empresa paulistana fundada em 2019. Forte presença em blogs de viagem. Parceiros visíveis: T-Mobile, Vodafone, Orange, AT&T. 165+ avaliações Google com nota 4.4–4.5. Nota 6.2/10 no Reclame Aqui.

#### O que fazem bem

**Simulador de plano por perfil de uso**
O site oferece um simulador interativo onde o usuário informa: destino, duração e intensidade de uso (leve, moderado, intenso). O sistema recomenda o plano ideal. Isso elimina a paralisia de decisão em catálogos com múltiplos SKUs — e reduz contato de suporte para dúvidas de pré-compra.

> 📍 *Screenshot sugerido: interface do simulador da Casa do Chip*

**Cupons de influenciadores integrados ao produto**
Códigos de desconto de criadores de conteúdo de viagem (`VAMBORA`, `VICIADAEMVIAJAR`, `VAMOSFUGIR10`) são parte da estratégia de aquisição. O campo de cupom no checkout é o ponto de entrada de um canal de marketing de baixo CAC que também gera prova social orgânica.

**Logos de operadoras parceiras visíveis**
T-Mobile, Vodafone, Orange, AT&T aparecem como parceiros. Isso responde a uma dúvida técnica recorrente do viajante: "em qual rede eu vou conectar?" — sem precisar consultar suporte.

> 📍 *Screenshot sugerido: seção de parceiros da Casa do Chip*

**Desconto PIX com destaque**
5% de desconto no pagamento via PIX é exibido como badge nos cards de preço. Incentiva o método mais econômico para a empresa e gera percepção de vantagem para o usuário.

**Tutorial em vídeo para instalação de eSIM**
Vídeo no YouTube embarcado na página de produto mostrando o passo a passo de instalação. Reduz o volume de chamados de suporte pós-venda sobre ativação — que é a principal categoria de reclamação no Reclame Aqui do segmento.

#### O que é fraco
- Nota 6.2/10 no Reclame Aqui (vs. 8.2 da AmericaChip) — reputação é o principal gap
- Principais reclamações: queda de conexão em áreas rurais, reembolsos demorados

---

## Parte 3 — Comparativo Geral

| Critério de design / UX | Simpremium | AmericaChip | Nomad | SC Conecta | O Meu Chip | Casa do Chip |
|---|:---:|:---:|:---:|:---:|:---:|:---:|
| Navegação por destino como estrutura principal | ⚠️ | ✅ | ✅ | ✅ | ✅ | ✅ |
| Preço âncora visível no card sem clicar | ⚠️ | ✅ | ✅ | ✅ | ✅ | ✅ |
| Conversor BRL em tempo real | ❌ | ❌ | ✅ | ⚠️ | ❌ | ❌ |
| Data picker integrado ao fluxo de compra | ❌ | ❌ | ❌ | ✅ | ❌ | ❌ |
| Simulador "qual plano é pra mim?" | ❌ | ❌ | ❌ | ❌ | ❌ | ✅ |
| Reviews/prova social na 2ª dobra | ❌ | ✅ | ✅ | ✅ | ❌ | ⚠️ |
| Prova social com números concretos | ⚠️ | ✅ | ✅ | ✅ | ❌ | ⚠️ |
| Trust badges / segurança visível | ❌ | ✅ | ✅ | ⚠️ | ❌ | ⚠️ |
| Chip vs. eSIM comparável na mesma tela | ❌ | ❌ | ❌ | ❌ | ✅ | ⚠️ |
| Bundle com produto complementar | ❌ | ❌ | ✅ | ❌ | ✅ | ❌ |
| Parceiros / operadoras visíveis | ❌ | ❌ | ✅ | ❌ | ✅ | ✅ |
| Tutorial de ativação de eSIM | ⚠️ | ⚠️ | ❌ | ⚠️ | ❌ | ✅ |
| Custo total sem taxa surpresa no checkout | ❌ | ✅ | ✅ | ✅ | ✅ | ✅ |
| Suporte WhatsApp com destaque | ✅ | ✅ | ❌ | ✅ | ❌ | ✅ |
| Desconto PIX explícito | ❌ | ❌ | ❌ | ❌ | ❌ | ✅ |
| Experiência mobile sem perda de conteúdo | ❌ | ✅ | ✅ | ✅ | ⚠️ | ✅ |

**Legenda:** ✅ Implementado | ⚠️ Parcial | ❌ Ausente

---

## Parte 4 — Oportunidades de Design para o Redesign

As oportunidades abaixo estão ordenadas por impacto esperado em conversão e são fundamentadas diretamente nas análises acima.

---

### Oportunidade 1 — Transparência total de custo desde o início
**Prioridade: Alta | Referência: SC Conecta + AmericaChip**

A taxa de ativação de USD 5,95 deve aparecer no card de plano, não apenas no checkout. Idealmente, o preço exibido já inclui a taxa, com nota explicativa. O mesmo vale para a conversão em BRL: exibir o equivalente aproximado em reais reduz a barreira de decisão para usuários que não sabem a cotação do dólar.

**Impacto esperado:** Redução de abandono no checkout por surpresa de custo.

---

### Oportunidade 2 — Substituir dropdown por seletor visual de destino
**Prioridade: Alta | Referência: AmericaChip + O Meu Chip**

Substituir a lista de 180+ países por uma grade visual com os 8–10 destinos mais vendidos (EUA, Europa, Ásia, Global, América do Sul, etc.) + campo de busca para outros destinos. A lógica é a mesma de todos os concorrentes: o viajante pensa em região, não em país específico.

**Impacto esperado:** Redução do tempo para seleção de plano; melhora em mobile.

---

### Oportunidade 3 — Date picker que calcula o custo total da viagem
**Prioridade: Alta | Referência: SC Conecta**

Permitir que o usuário informe as datas da viagem antes de ver os planos. O sistema calcula automaticamente o custo total (preço por dia × dias selecionados). O usuário chega na tela de seleção de plano sabendo o custo real da viagem, não o custo por dia.

**Impacto esperado:** Redução de abandono por incerteza de custo total; experiência personalizada.

---

### Oportunidade 4 — Reviews subindo para a 2ª dobra
**Prioridade: Alta | Referência: AmericaChip + Nomad**

A Simpremium tem 230+ avaliações com nota 4.5 — melhor que a maioria dos concorrentes. Esse ativo está posicionado tarde demais no scroll. Mover para logo após o hero, com número de avaliações, nota e 2–3 depoimentos em destaque.

**Impacto esperado:** Maior persuasão no início da jornada, quando o usuário ainda está decidindo se confia na marca.

---

### Oportunidade 5 — Simulador "qual plano é para mim?"
**Prioridade: Média | Referência: A Casa do Chip**

Um fluxo de 3 perguntas — destino, duração, intensidade de uso — que recomenda um plano específico. Resolve a paralisia de decisão causada pelos múltiplos SKUs (ilimitado, franquia diária, franquia total para o mesmo destino).

**Impacto esperado:** Redução de contato de suporte para dúvidas pré-compra; aumento de confiança na decisão de compra.

---

### Oportunidade 6 — Página de eSIM com produto real
**Prioridade: Alta | Referência: problema interno**

A página `/esim/` atual não tem preços nem CTAs de compra. É uma página informativa que não converte. Deve ser redesenhada como página de produto — com planos, preços, comparação com chip físico e CTA direto.

**Impacto esperado:** Captura de usuários que chegam por busca orgânica por "esim internacional" — hoje esse tráfego não converte.

---

### Oportunidade 7 — Corrigir mobile: nunca esconder conteúdo de credibilidade
**Prioridade: Alta | Referência: problema interno**

Remover o `display: none` no mobile para elementos de informação e prova social. Todo trust signal deve estar visível no celular. É o device onde a maioria dos viajantes pesquisa e toma a decisão de compra.

**Impacto esperado:** Redução de abandono mobile; paridade de experiência com desktop.

---

### Oportunidade 8 — Seção de trust consolidada
**Prioridade: Média | Referência: Nomad Global**

Criar uma seção dedicada que concentre: número de clientes atendidos, países cobertos, nota de avaliações, logos de operadoras parceiras e selos de segurança de pagamento. Localizar antes do footer para impactar o usuário no momento de maior hesitação.

**Impacto esperado:** Aumento de credibilidade; redução de abandono por desconfiança.

---

### Oportunidade 9 — Logos de operadoras parceiras visíveis
**Prioridade: Média | Referência: A Casa do Chip + O Meu Chip**

T-Mobile, Vodafone, Orange, AT&T, Claro — quais redes o usuário vai usar? Essa é uma dúvida técnica frequente. Exibir os logos das operadoras parceiras por região responde a pergunta sem requerer suporte.

---

### Oportunidade 10 — Desconto PIX com badge visual
**Prioridade: Baixa | Referência: A Casa do Chip**

Exibir `PIX — 5% de desconto` como badge nos cards de preço. Incentiva o método mais econômico para a empresa e gera percepção de vantagem para o usuário.

---

## Parte 5 — Resumo Executivo

A Simpremium tem ativos competitivos reais: melhor cobertura do grupo (184 países no eSIM), preço mais agressivo (a partir de USD 1), suporte 24h que os clientes elogiam e um volume de reviews acima dos concorrentes. O problema não é o produto — é a **plataforma não comunicar o valor do produto com clareza**.

Os concorrentes não têm produto melhor. Têm interfaces que removem fricção em três pontos críticos da jornada do viajante:

1. **"Quanto vai me custar?"** — respondido com preço total, sem surpresas
2. **"Qual plano é o certo pra mim?"** — respondido com navegação por destino + simulador
3. **"Posso confiar nessa empresa?"** — respondido com prova social posicionada estrategicamente

O redesign da Simpremium tem a oportunidade de ser a melhor experiência do segmento — combinando o conversor de moeda do Nomad, o date picker do SC Conecta, o simulador da Casa do Chip e a navegação geográfica da AmericaChip. Nenhum concorrente fez tudo. A Simpremium pode.

---

*Documento produzido com base em análise direta das interfaces em abril de 2026.*
*Próximo passo sugerido: mapeamento das telas atuais da Simpremium com anotações de oportunidade por página.*
