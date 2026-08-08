# Caderno Temático: Violência no Brasil

PROJETO: Treinando uma IA de Aprendizagem: Explore o Poder do NotebookLM

> **Estudo exploratório utilizando o Gemini Notebook e fontes públicas oficiais**

## 1. Contexto e Objetivos

### Contexto

A violência é um dos principais problemas sociais brasileiros e possui características bastante heterogêneas quando analisada sob diferentes perspectivas, como território, faixa etária, gênero, raça/cor, condição socioeconômica e tipo de violência.

O caderno temático teve como objeto de estudo a **violência no Brasil**, utilizando como principal referência o **Atlas da Violência 2026**, produzido pelo Instituto de Pesquisa Econômica Aplicada (IPEA) em parceria com o Fórum Brasileiro de Segurança Pública (FBSP).

A edição de 2026 representa uma década de publicação do Atlas e utiliza principalmente informações provenientes do **Sistema de Informações sobre Mortalidade (SIM)** e do **Sistema de Informação de Agravos de Notificação (Sinan)**, ambos do Ministério da Saúde.

Um dos pontos que despertou especial interesse durante a pesquisa foi a diferença entre os homicídios oficialmente registrados e os chamados **homicídios ocultos**, estimados a partir das mortes violentas classificadas como de causa indeterminada. Em 2024, o Atlas estima 49.673 homicídios, dos quais 7.083 seriam homicídios ocultos. Isso representa 14,3% dos homicídios estimados naquele ano. 

O estudo também evidencia que a violência não está distribuída de maneira uniforme pelo território brasileiro. Em 2024, por exemplo, metade dos homicídios ocorreu em apenas 99 municípios, aproximadamente 1,8% dos municípios brasileiros.

### Objetivos

O objetivo geral do caderno temático foi utilizar ferramentas de Inteligência Artificial, especialmente o **Gemini Notebook**, como instrumento de apoio à pesquisa, análise e consolidação de conhecimento sobre a violência no Brasil.

Os objetivos específicos são:

- Compreender a evolução da violência letal no Brasil na última década;
- Identificar os principais indicadores utilizados para medir a violência;
- Compreender as diferenças entre homicídios registrados, homicídios estimados e mortes violentas por causa indeterminada;
- Analisar a distribuição territorial dos homicídios;
- Investigar como fatores como idade, gênero e raça/cor estão relacionados à violência;
- Identificar grupos populacionais mais vulneráveis;
- Comparar informações provenientes de diferentes sistemas oficiais;
- Avaliar as limitações e possíveis problemas de qualidade dos dados;
- Utilizar técnicas de engenharia de prompts para extrair diferentes perspectivas de uma mesma base documental;
- Desenvolver um conjunto de prompts reutilizáveis para futuras pesquisas.

---

# 2. Curadoria de Fontes

Para a construção do caderno foram selecionadas fontes públicas, institucionais e abertas, priorizando documentos produzidos por órgãos oficiais ou instituições reconhecidas na produção de estatísticas sobre violência e segurança pública.

## Fonte 1 — Atlas da Violência 2026

**Principal fonte do estudo.**

Instituto de Pesquisa Econômica Aplicada (IPEA) e Fórum Brasileiro de Segurança Pública (FBSP).

O documento apresenta análises sobre homicídios, violência contra jovens, mulheres, população negra, população LGBTQI+, indígenas, idosos, pessoas com deficiência, entre outros grupos.

**Fonte:**

[Atlas da Violência 2026 — IPEA](https://repositorio.ipea.gov.br/server/api/core/bitstreams/6e855a6f-1a5d-494d-90aa-753862e10369/content)

---

## Fonte 2 — Anuário Brasileiro de Segurança Pública 2026

Produzido pelo Fórum Brasileiro de Segurança Pública, reúne informações fornecidas pelas secretarias estaduais de segurança pública, polícias civis, militares e federal, entre outras fontes oficiais.

Foi selecionado para permitir a comparação entre os dados provenientes da área da saúde, utilizados pelo Atlas, e os dados provenientes dos sistemas de segurança pública.

**Fonte:**

[Anuário Brasileiro de Segurança Pública 2026 — FBSP](http://forumseguranca.org.br/wp-content/uploads/2026/07/anuario-2026.pdf)

---

## Fonte 3 — Dados Nacionais de Segurança Pública / Sinesp (Sistema Nacional de Informações de Segurança Pública)

Os dados do Sinesp são produzidos a partir das informações encaminhadas pelos Estados e pelo Distrito Federal e permitem analisar indicadores criminais provenientes da área de segurança pública.

Essa fonte é particularmente importante para compreender as diferenças metodológicas entre os registros da saúde e os registros policiais.

**Fonte:**

[Dados Nacionais de Segurança Pública — Ministério da Justiça e Segurança Pública](https://www.gov.br/mj/pt-br/assuntos/sua-seguranca/seguranca-publica/estatistica)

---

## Fonte 4 — Mapa de Segurança Pública 2026 / Sinesp (Sistema Nacional de Informações de Segurança Pública)

O Mapa de Segurança Pública 2026, elaborado pela Secretaria Nacional de Segurança Pública (Senasp), do Ministério da Justiça e Segurança Pública (MJSP), reúne os principais indicadores criminais e de segurança pública do Brasil, tendo como referência os dados do ano-base de 2025. A publicação apresenta informações sobre diferentes tipos de ocorrências e permite analisar a evolução e a distribuição dos crimes e outros indicadores de segurança pública no território nacional.

Essa fonte é particularmente importante para complementar o Atlas da Violência 2026, pois utiliza informações provenientes dos sistemas de segurança pública. A comparação entre as duas publicações permite investigar diferenças entre os dados produzidos pelas áreas de saúde e segurança pública, além de possibilitar uma análise mais ampla sobre homicídios, criminalidade, distribuição territorial e tendências da violência no Brasil.

**Fonte:**

[Mapa de Segurança Pública 2026 — Ministério da Justiça e Segurança Pública](https://www.gov.br/mj/pt-br/assuntos/sua-seguranca/seguranca-publica/estatistica/download/mapa-de-seguranca-publica-2026.pdf/?utm_source=chatgpt.com)


# 3. Engenharia de Prompts

Uma das etapas mais importantes deste estudo foi utilizar o Gemini Notebook não apenas para obter respostas, mas para experimentar diferentes formas de formular perguntas.

O objetivo foi verificar como pequenas alterações no prompt poderiam produzir respostas com diferentes níveis de profundidade, síntese, comparação e criticidade.

## 3.1. Perguntas exploratórias

### Prompt 01 — Visão geral

> Faça um resumo executivo do Atlas da Violência 2026 em no máximo 15 tópicos. Para cada tópico, apresente o principal achado e indique a página ou seção do documento que sustenta a informação.

**Objetivo:** obter uma visão geral inicial do documento.

---

### Prompt 02 — Principais descobertas

> Quais são as 10 descobertas mais importantes do Atlas da Violência 2026? Priorize descobertas que tenham relevância estatística, social ou para formulação de políticas públicas. Para cada uma, informe os números apresentados no documento e a respectiva fonte.

**Objetivo:** identificar rapidamente os achados de maior relevância.

---

### Prompt 03 — O que mudou?

> Compare os principais indicadores de violência apresentados para 2014 e 2024. Quais melhoraram, quais pioraram e quais permaneceram relativamente estáveis? Apresente os resultados em uma tabela.

**Objetivo:** compreender a evolução da violência ao longo da década.

---

# 3.2. Engenharia de prompts para análise crítica

### Prompt 04 — Homicídios registrados x estimados

> Explique detalhadamente a diferença entre homicídios registrados e homicídios estimados no Atlas da Violência 2026. Por que os dois números são diferentes? Explique também o conceito de homicídio oculto e sua relação com as Mortes Violentas por Causa Indeterminada (MVCI).

**Objetivo:** compreender uma das questões metodológicas mais importantes do Atlas.

---

### Prompt 05 — Investigação da queda dos homicídios

> O Atlas da Violência 2026 indica uma redução dos homicídios no Brasil. Analise criticamente essa conclusão. Quais evidências sustentam a redução? Quais fatores relacionados à qualidade dos dados podem dificultar sua interpretação?

**Objetivo:** evitar uma interpretação superficial da queda dos indicadores.

---

### Prompt 06 — Qualidade dos dados

> Identifique todas as limitações metodológicas mencionadas no Atlas da Violência 2026 que possam afetar a interpretação dos dados sobre homicídios. Classifique essas limitações em: subnotificação, classificação, cobertura, metodologia e qualidade dos registros.

**Objetivo:** transformar o documento em uma análise crítica da própria base de dados.

---

# 3.3. Prompts para análise territorial

### Prompt 07 — Estados

> Quais estados brasileiros apresentaram as maiores taxas de homicídio em 2024? Quais apresentaram as menores? Apresente uma tabela com estado, taxa, número de homicídios e posição no ranking.

**Objetivo:** compreender a distribuição regional da violência.

---

### Prompt 08 — Concentração municipal

> O Atlas afirma que 50% dos homicídios brasileiros ocorreram em apenas 99 municípios em 2024. Explique a importância estatística e social desse fenômeno. O que essa concentração pode indicar sobre políticas públicas de segurança?

**Objetivo:** explorar a concentração territorial da violência.

---

### Prompt 09 — Comparação regional

> Compare Norte, Nordeste, Centro-Oeste, Sudeste e Sul quanto à violência letal. Identifique padrões, diferenças e possíveis hipóteses explicativas apresentadas ou sugeridas pelo Atlas. Separe claramente fatos apresentados no documento de hipóteses interpretativas.

**Objetivo:** estimular uma análise comparativa sem confundir dados com interpretação.

---

# 3.4. Prompts para análise de grupos vulneráveis

### Prompt 10 — Juventude

> Analise a violência contra jovens de 15 a 29 anos no Brasil. Qual é a participação desse grupo no total de homicídios? Como esse indicador evoluiu entre 2014 e 2024? Quais estados apresentaram os maiores problemas?

O Atlas registra que, em 2024, foram contabilizados 19.801 homicídios de jovens de 15 a 29 anos, contra 32.436 em 2014, uma redução de 39,0%. 

---

### Prompt 11 — Raça

> Analise a relação entre raça/cor e homicídios apresentada no Atlas da Violência 2026. Quais grupos são mais afetados? Apresente os indicadores absolutos e relativos e explique por que a análise de taxas é importante.

**Objetivo:** compreender desigualdades raciais na violência letal.

---

### Prompt 12 — Mulheres

> Faça uma análise completa da violência contra as mulheres apresentada no Atlas da Violência 2026. Diferencie homicídio, violência doméstica, violência não letal e violência sexual. Quais são os principais padrões identificados?

**Objetivo:** evitar tratar diferentes formas de violência contra mulheres como um único fenômeno.

---

# 3.5. Prompts para cruzamento entre fontes

### Prompt 13 — Saúde x Segurança Pública

> Compare os dados de violência provenientes do SIM/Sin an e do Sinesp. Explique por que os números podem ser diferentes e quais são as vantagens e limitações de cada fonte.

**Objetivo:** compreender que diferentes sistemas podem produzir estatísticas diferentes sobre o mesmo fenômeno.

---

### Prompt 14 — Auditoria de evidências

> Para cada uma das principais conclusões apresentadas no Atlas da Violência 2026, identifique: (1) dado utilizado, (2) fonte original, (3) metodologia empregada, (4) limitação conhecida e (5) grau de confiança que pode ser atribuído à conclusão.

**Objetivo:** transformar o NotebookLM em uma ferramenta de auditoria documental.

---

# 3.6. Prompt de investigação

### Prompt 15 — Investigação aberta

> Leia integralmente as fontes disponíveis e identifique relações relevantes entre violência, território, idade, gênero, raça e condições sociais que não estejam explicitamente destacadas no resumo executivo. Para cada relação encontrada, apresente as evidências que sustentam a hipótese e deixe claro quando estiver fazendo uma inferência.

**Objetivo:** utilizar a IA para encontrar padrões que poderiam passar despercebidos em uma leitura linear.

---

# 4. "Cicatrizes" — Troubleshooting da Pesquisa

Durante a utilização de IA para análise documental, alguns problemas foram identificados e solucionados. O registro dessas dificuldades é importante porque demonstra que o resultado final não foi simplesmente "gerado pela IA", mas passou por uma avaliação mais crítica e humana.

## Cicatriz 01 — Confusão entre números registrados e estimados

Um dos principais cuidados identificados foi a existência de diferentes números para homicídios.

O Atlas apresenta tanto homicídios registrados oficialmente quanto estimativas que incorporam os chamados homicídios ocultos.

**Problema:** perguntar simplesmente "quantos homicídios ocorreram no Brasil em 2024?" produz respostas diferentes dependendo do indicador considerado.

**Solução:** prompt ajustado para ser mais específico:

> Foi soilicitado para informar separadamente homicídios registrados, homicídios estimados e homicídios ocultos procurando evitar a mistura entre os indicadores.

---

## Cicatriz 02 — Confusão entre fontes

O Atlas utiliza informações provenientes de diferentes sistemas.

**Problema:** a IA pode apresentar como sendo do SIM uma informação que originalmente pertence ao Sinesp ou ao Sinan.

**Solução:**

> Para cada número apresentado, foi solicitado explicitamente a fonte original e não apenas a publicação onde o número foi encontrado.

---

## Cicatriz 03 — Respostas excessivamente genéricas

Perguntas como "explique o Atlas da Violência" produziram respostas muito abrangentes e pouco úteis para uma investigação aprofundada.

**Solução:** realizada a divizão da investigação em perguntas menores e progressivas, explorando cada dimensão separadamente.

---

# 5. Miniguia de Estudo

## 5.1. O que é o Atlas da Violência?

O Atlas da Violência é uma publicação produzida pelo IPEA em parceria com o Fórum Brasileiro de Segurança Pública com o objetivo de analisar a violência no Brasil utilizando principalmente dados do Ministério da Saúde.

A edição de 2026 marca dez anos da publicação e amplia a discussão sobre violência estrutural e seus impactos diferenciados sobre grupos sociais.

---

## 5.2. Principais fontes de dados

O Atlas utiliza principalmente:

**SIM — Sistema de Informações sobre Mortalidade**

Registra óbitos e suas causas. É uma das principais fontes para análise de homicídios.

**Sinan — Sistema de Informação de Agravos de Notificação**

Registra notificações de violência atendidas pelos serviços de saúde e permite analisar formas de violência que não necessariamente chegam ao sistema policial.

**Sinesp**

Sistema utilizado para consolidação de informações de segurança pública provenientes dos Estados e do Distrito Federal.

---

## 5.3. Principais conceitos aprendidos (Glossário)

### Homicídio

Morte provocada intencionalmente por outra pessoa, conforme a classificação utilizada na análise estatística.

### Taxa de homicídio

Número de homicídios proporcional à população, normalmente expresso por **100 mil habitantes**.

A utilização da taxa permite comparar localidades com populações diferentes.

### Homicídio registrado

Homicídio classificado oficialmente como tal no Sistema de Informação sobre Mortalidade.

### Homicídio estimado

Estimativa produzida pelo Atlas incorporando uma parcela das mortes violentas cuja causa permaneceu indeterminada e que, segundo a metodologia utilizada, podem corresponder a homicídios.

### Homicídio oculto

Homicídio que não aparece originalmente classificado como homicídio no SIM, mas que é estimado pelo modelo utilizado pelo Atlas a partir das mortes violentas de causa indeterminada.

Em 2024, foram estimados 7.083 homicídios ocultos, correspondendo a 14,3% dos homicídios estimados daquele ano.

### MVCI — Morte Violenta por Causa Indeterminada

Morte violenta na qual não foi possível determinar adequadamente a causa ou a intencionalidade do óbito.

O aumento das MVCI é uma das principais preocupações metodológicas apresentadas na edição de 2026.

### Letalidade violenta

Conjunto de mortes resultantes de diferentes formas de violência intencional, utilizado para analisar a dimensão mais grave da violência.

### Violência doméstica

Violência praticada no contexto familiar ou doméstico, podendo envolver diferentes tipos de agressão física, psicológica, sexual ou negligência.

### Violência interpessoal

Violência praticada por outra pessoa contra o indivíduo, abrangendo diferentes formas e contextos de agressão.

### Vitimização

Condição ou processo pelo qual uma pessoa é vítima de determinado tipo de violência ou crime.

### Subnotificação

Situação em que parte dos eventos ocorridos não é registrada ou identificada adequadamente pelos sistemas oficiais.

### Série histórica

Conjunto de dados referentes a diferentes períodos que permite analisar tendências e mudanças ao longo do tempo.

### Desigualdade territorial

Diferença na distribuição da violência entre regiões, estados e municípios.

### Letalidade policial

Mortes decorrentes da atuação de agentes de segurança pública.

### Vulnerabilidade

Maior exposição ou suscetibilidade de determinados grupos ou populações a determinados tipos de violência.

---

# 6. Principais aprendizados

A análise do Atlas da Violência 2026 permite destacar alguns aprendizados importantes:

1. **A violência brasileira apresenta tendência de redução nos homicídios**, mas a interpretação dessa redução exige atenção à qualidade dos registros.

2. **Os números oficiais não necessariamente representam toda a violência ocorrida**, devido à subnotificação e aos problemas de classificação.

3. **A análise de taxas é fundamental** para comparar estados e municípios com populações diferentes.

4. **A violência está fortemente concentrada territorialmente**, não sendo distribuída uniformemente pelo país.

5. **Jovens constituem um dos grupos mais afetados pela violência letal**, embora a quantidade de homicídios nesse grupo tenha diminuído significativamente na última década.

6. **A violência possui forte dimensão racial e de gênero**, atingindo grupos populacionais de maneira desigual.

7. **Diferentes sistemas de informação produzem perspectivas diferentes sobre o mesmo fenômeno**, sendo necessário compreender a metodologia antes de comparar números.

8. **Inteligência Artificial não substitui a análise crítica das fontes.** Ela pode acelerar a pesquisa, organizar informações e identificar padrões, mas os resultados precisam ser confrontados com os documentos originais.

---

# 7. Biblioteca de Prompts Reutilizáveis

Os prompts abaixo podem ser reutilizados em futuras pesquisas documentais.

### Resumo executivo

> Resuma o documento em 10 tópicos, priorizando dados quantitativos, conclusões relevantes e informações que possam alterar a interpretação do problema estudado. Para cada tópico, indique a fonte ou página correspondente.

### Extração de indicadores

> Extraia todos os principais indicadores quantitativos relacionados a [TEMA]. Apresente nome do indicador, valor, período, unidade de medida, fonte e página.

### Comparação temporal

> Compare [ANO 1] e [ANO 2] para o indicador [INDICADOR]. Calcule a variação percentual e explique quais mudanças são estatisticamente ou socialmente mais relevantes.

### Comparação territorial

> Compare os estados/municípios quanto ao indicador [INDICADOR]. Apresente ranking, valores absolutos, taxas e variação percentual.

### Análise crítica

> Quais são as principais limitações metodológicas da fonte para responder à pergunta [PERGUNTA]? Diferencie limitações de cobertura, qualidade, classificação, metodologia e atualização.

### Validação

> Verifique se a afirmação "[AFIRMAÇÃO]" é sustentada pelas fontes disponíveis. Apresente as evidências favoráveis, contrárias ou insuficientes e informe onde elas aparecem no documento.

### Fato x inferência

> Separe a resposta em três categorias: fatos explicitamente apresentados pela fonte, interpretações dos autores e inferências que podem ser feitas a partir dos dados.

### Busca de padrões

> Identifique padrões relevantes nos dados relacionados a [VARIÁVEL 1], [VARIÁVEL 2] e [VARIÁVEL 3]. Não estabeleça causalidade sem evidência. Diferencie correlação, associação e causalidade.

### Auditoria de resposta da IA

> Revise sua própria resposta. Identifique possíveis erros factuais, números sem fonte, interpretações não sustentadas e conclusões que possam ter sido extrapoladas além do que os documentos permitem afirmar.

### Síntese final

> Produza uma síntese executiva de [TEMA] utilizando exclusivamente as fontes fornecidas. Para cada conclusão, apresente a evidência correspondente. Não invente informações e indique explicitamente quando os dados forem insuficientes.

---

# 8. Conclusão

A construção deste caderno mostrou que ferramentas como o Gemini Notebook podem ser utilizadas não apenas para resumir documentos, mas como instrumentos de **investigação, comparação, validação e organização do conhecimento**.

O principal aprendizado metodológico foi perceber que a qualidade da resposta depende diretamente da qualidade da pergunta. Prompts genéricos tendem a produzir respostas genéricas, enquanto perguntas estruturadas, que especificam indicadores, períodos, fontes, critérios de comparação e necessidade de evidências, permitem obter resultados muito mais úteis.

Outro aprendizado importante foi a necessidade de manter uma postura crítica em relação às respostas produzidas pela IA. No estudo da violência, por exemplo, conceitos aparentemente semelhantes — como homicídios registrados, homicídios estimados e homicídios ocultos — podem representar indicadores diferentes.

Assim, a IA foi utilizada neste projeto como **ferramenta de apoio à análise**, e não como fonte primária de informação. As conclusões devem sempre ser confrontadas com os documentos e dados originais.

---

## Fontes

- IPEA; FBSP. **Atlas da Violência 2026**.
- Fórum Brasileiro de Segurança Pública. **19º Anuário Brasileiro de Segurança Pública 2025**.
- Ministério da Saúde. **Sistema de Informação sobre Mortalidade — SIM**.
- Ministério da Saúde. **Sistema de Informação de Agravos de Notificação — Sinan**.
- Ministério da Justiça e Segurança Pública. **Dados Nacionais de Segurança Pública — Sinesp**.

---

## Tecnologias e ferramentas utilizadas

- [Gemini notebook](https://notebooklm.google.com/)
- Inteligência Artificial Generativa
- Engenharia de Prompts
- Análise documental
- Dados públicos governamentais
- Markdown / GitHub
