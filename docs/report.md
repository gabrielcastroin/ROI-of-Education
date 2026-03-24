# ROI of Education


**Gabriel Castro Inacio, gabriel.inacio.1622289@sga.pucminas.br**

**Lucas Diniz Leão, ldleao@sga.pucminas.br**

**Nathalia Ramalho Abranches de Araujo, nathalia.araujo.1637955@sga.pucminas.br**

**Rafael de Alcantara Aguiar Cruz, rafael.alcantara.1622297@sga.pucminas.br**

**Daniel Guerra Costa, daniel.costa.1647250@sga.pucminas.br**

---

Professores:

**Marco Paulo Soares Gomes**

**Gabriel Barbosa Fonseca**

---

_Curso de Ciência de Dados, Unidade Praça da Liberdade_

_Instituto de Informática e Ciências Exatas – Pontifícia Universidade de Minas Gerais (PUC MINAS), Belo Horizonte – MG – Brasil_

---

## Resumo

O investimento em educação é amplamente reconhecido como um dos principais motores do desenvolvimento socioeconômico de um país. No Brasil, entretanto, a relação entre o gasto público educacional e indicadores como o Produto Interno Bruto (PIB), o Índice de Desenvolvimento Humano (IDH) e o mercado de trabalho ainda carece de análises preditivas aprofundadas. Este trabalho propõe uma análise histórica e multivariada dessas relações, integrando bases de dados oficiais sobre investimento em educação, crescimento do PIB, evolução do IDH e indicadores complementares ao longo das últimas décadas. A partir dessa análise exploratória, são desenvolvidos modelos preditivos capazes de, por um lado, projetar os impactos do investimento educacional atual sobre os indicadores econômicos e sociais futuros e, por outro, estimar tendências de investimento com base no comportamento histórico e seus possíveis efeitos no desenvolvimento do país. Os resultados indicam que variações no investimento em educação apresentam correlação significativa com melhorias no IDH e no crescimento econômico em horizontes de médio e longo prazo, reforçando a importância de políticas públicas consistentes na área.._

---


## Introdução

###    Contextualização
O desenvolvimento socioeconômico de uma nação está intrinsecamente ligado à qualidade e ao volume de investimentos realizados em sua educação. Organismos internacionais como a Organização para a Cooperação e Desenvolvimento Econômico (OCDE) e o Programa das Nações Unidas para o Desenvolvimento (PNUD) reconhecem a educação como um dos pilares fundamentais para a redução da desigualdade, o crescimento da produtividade e a melhoria das condições de vida da população. Segundo o relatório Education at a Glance (OCDE, 2023), países que sustentam maior investimento por aluno ao longo do tempo tendem a apresentar indicadores econômicos e sociais mais robustos no médio e longo prazo.

No contexto brasileiro, essa relação ganha contornos ainda mais relevantes diante da magnitude e da complexidade do sistema educacional do país. O Brasil possui mais de 47 milhões de alunos matriculados na educação básica pública, distribuídos entre três esferas de governo — União, estados e municípios —, o que torna a alocação eficiente de recursos um desafio estrutural de governança. Entre 2014 e 2023, o investimento público total em educação oscilou entre 4,1% e 5,1% do PIB, atingindo R$ 540 bilhões em 2023, conforme dados do Anuário Brasileiro da Educação Básica (Todos pela Educação, 2025). Apesar do volume expressivo, o gasto médio por aluno da educação básica no Brasil é de US$ 3.668 — menos de um terço da média dos países da OCDE, que é de US$ 11.914.

###    Problema

Embora o investimento em educação seja reconhecido como vetor de desenvolvimento, a relação quantitativa entre o gasto educacional público e os indicadores macroeconômicos e sociais do Brasil ainda carece de análises sistemáticas baseadas em dados históricos de longo prazo. Decisões de política pública sobre alocação orçamentária na área da educação são frequentemente tomadas sem o suporte de modelos analíticos que evidenciem o impacto esperado dessas escolhas sobre variáveis como o Produto Interno Bruto (PIB), o Índice de Desenvolvimento Humano (IDH) e a taxa de desemprego. Essa lacuna dificulta a formulação de políticas educacionais orientadas por evidências e limita a capacidade do Estado de antecipar os efeitos de variações no investimento sobre o desenvolvimento nacional.

###    Objetivo geral

Desenvolver uma análise preditiva baseada em dados históricos brasileiros para investigar e quantificar a relação entre o investimento público em educação e indicadores socioeconômicos — como PIB, IDH e taxa de desemprego —, projetando cenários futuros a partir de tendências identificadas nos dados.

####    Objetivos específicos

Coletar, tratar e integrar bases de dados oficiais sobre investimento educacional, crescimento do PIB, evolução do IDH e taxa de desemprego no Brasil em séries históricas de longo prazo.

Construir um modelo de regressão múltipla para identificar e mensurar as correlações entre o investimento em educação e os indicadores socioeconômicos selecionados.

Desenvolver um modelo de série temporal para projetar a evolução dos indicadores socioeconômicos com base nas tendências históricas de investimento educacional.

Comparar os resultados dos modelos e interpretar os achados sob a perspectiva da governança pública e da formulação de políticas educacionais.


###    Justificativas

A escolha deste tema justifica-se pela relevância estratégica que o investimento em educação representa para o planejamento de longo prazo do Estado brasileiro. Em um cenário de restrições fiscais recorrentes, gestores públicos necessitam de instrumentos analíticos que embasem decisões sobre onde e como alocar recursos de forma a maximizar retornos sociais e econômicos. A aplicação de técnicas de ciência de dados a dados públicos disponíveis permite não apenas compreender padrões históricos, mas também antecipar consequências de diferentes trajetórias de investimento — contribuindo diretamente para uma governança mais orientada por evidências.
Além disso, o trabalho se insere em um campo interdisciplinar que articula ciência de dados, economia e políticas públicas, contribuindo para a disseminação de práticas analíticas no setor público brasileiro, ainda incipiente no uso sistemático de modelos preditivos para planejamento educacional.



##    Público alvo

O principal público-alvo desta análise é o Governo Federal brasileiro, especialmente os gestores e técnicos vinculados ao Ministério da Educação (MEC), ao Ministério da Fazenda e à Casa Civil, responsáveis pelo planejamento orçamentário e pela formulação de políticas educacionais nacionais. Esses perfis possuem conhecimento técnico em gestão pública e economia, mas não necessariamente em ciência de dados ou modelagem preditiva, o que reforça a importância de apresentar os resultados de forma clara, interpretável e orientada à tomada de decisão.
Como público secundário, destacam-se pesquisadores acadêmicos das áreas de economia da educação, políticas públicas e ciência de dados, bem como organismos de controle como o Tribunal de Contas da União (TCU) e instituições de pesquisa como o Ipea, que podem utilizar os modelos e metodologias desenvolvidos como referência para análises complementares.



**Persona 1 — Gestor de Política Pública**

| Atributo | Descrição |
|---|---|
| **Nome** | Carlos Mendes |
| **Idade** | 45 anos |
| **Cargo** | Diretor de Orçamento — Ministério da Educação |
| **Formação** | Administração Pública / Ciências Econômicas |
| **Relação com tecnologia** | Intermediária — usa Excel, relatórios e painéis de BI básicos |
| **Objetivo** | Embasar decisões de alocação orçamentária com dados históricos e projeções confiáveis |
| **Dor principal** | Falta de modelos que conectem investimento educacional a resultados econômicos mensuráveis |
| **O que espera do projeto** | Projeções claras e interpretáveis sobre o impacto do investimento educacional no PIB e IDH |

---

**Persona 2 — Pesquisador / Analista de Dados**

| Atributo | Descrição |
|---|---|
| **Nome** | Ana Ribeiro |
| **Idade** | 31 anos |
| **Cargo** | Pesquisadora — Instituto de Pesquisa Econômica Aplicada (Ipea) |
| **Formação** | Estatística / Ciência de Dados |
| **Relação com tecnologia** | Alta — Python, R, SQL, modelos preditivos |
| **Objetivo** | Reproduzir e expandir a análise com novas variáveis e metodologias |
| **Dor principal** | Escassez de trabalhos que integrem dados educacionais e econômicos em pipelines reproduzíveis |
| **O que espera do projeto** | Código bem documentado, fontes claras e metodologia replicável |

---

**Persona 3 — Auditor / Controlador Público**

| Atributo | Descrição |
|---|---|
| **Nome** | Roberto Faria |
| **Idade** | 52 anos |
| **Cargo** | Auditor Federal — Tribunal de Contas da União (TCU) |
| **Formação** | Direito / Contabilidade Pública |
| **Relação com tecnologia** | Básica — familiarizado com relatórios e sistemas de transparência |
| **Objetivo** | Verificar se tendências de investimento estão alinhadas com metas de desenvolvimento |
| **Dor principal** | Dificuldade em avaliar o retorno real dos gastos públicos em educação |
| **O que espera do projeto** | Correlações claras entre gasto e resultado, com referências oficiais verificáveis |

---

### Mapa de Stakeholders

```
                        ┌─────────────────────────────┐
                        │     ALTA INFLUÊNCIA          │
                        │                             │
          ┌─────────────┤  • Ministério da Educação   ├─────────────┐
          │             │  • Ministério da Fazenda    │             │
          │             │  • Casa Civil               │             │
          │             └─────────────────────────────┘             │
          │                                                          │
  BAIXO INTERESSE                                          ALTO INTERESSE
          │             ┌─────────────────────────────┐             │
          │             │     BAIXA INFLUÊNCIA         │             │
          └─────────────┤                             ├─────────────┘
                        │  • Ipea / Pesquisadores     │
                        │  • TCU / CGU                │
                        │  • Sociedade Civil          │
                        └─────────────────────────────┘
```

| Stakeholder | Tipo | Interesse | Influência | Relação com o projeto |
|---|---|---|---|---|
| Ministério da Educação (MEC) | Primário | Alto | Alto | Principal beneficiário das análises e projeções |
| Ministério da Fazenda | Primário | Alto | Alto | Define teto orçamentário — impactado pelas projeções |
| Casa Civil | Primário | Médio | Alto | Coordena políticas interministeriais |
| Ipea | Secundário | Alto | Médio | Pode replicar e expandir a metodologia |
| TCU / CGU | Secundário | Médio | Médio | Interesse em evidências para auditorias de impacto |
| Sociedade Civil | Terciário | Baixo | Baixo | Beneficiária indireta das políticas informadas pelos dados |






## Análise exploratórida dos dados

###    Dicionário de dados

Apresente uma descrição das bases de dados a serem utilizadas. 
Dicionários de dados devem conter as bases de dados, os nomes dos atributos 
com seu significado, seu tipo (inteiro, real, textual, categórico, etc).

Este projeto deve utilizar pelo menos duas fontes de dados. Uma fonte principal e 
uma fonte para enriquecimentos dos dados principais.


###    Descrição de dados

Utilize a análise descritiva baseada em estatística de primeira ordem para descrever os dados.
Como descrever dados numéricos: média, desvio padrão, mínimo, máximo, quartis, histograma, etc.
Como descrever dados qualitativos (categóricos): moda (valor mais frequente), quantidade de valores distintos (categorias), distribuição das categorias (histograma), etc.


## Preparação dos dados

A preparação dos dados consiste dos seguintes passos:

> - Seleção dos atributos
> - Tratamentos dos valores faltantes ou omissos: remoção, substituição, indução, etc.
> - Tratamento dos valores inconsistentes: conversão, remoção de dados duplicados, remoção ou tratamento de ouliers.
> - Conversão de dados: p. ex. numérico para categórico, categórico para binário, etc.


## Indução de modelos

### Modelo 1: Algoritmo

Substitua o título pelo nome do algoritmo que será utilizado. P. ex. árvore de decisão, rede neural, SVM, etc.
Justifique a escolha do modelo.
Apresente o processo utilizado para amostragem de dados (particionamento, cross-validation).
Descreva os parâmetros utilizados. 
Apresente trechos do código utilizado comentados. Se utilizou alguma ferramenta gráfica, apresente imagens
com o fluxo de processamento.

### Modelo 2: Algoritmo

Repita os passos anteriores para o segundo modelo.


## Resultados

### Resultados obtidos com o modelo 1.

Apresente aqui os resultados obtidos com a indução do modelo 1. 
Apresente uma matriz de confusão quando pertinente. Apresente as medidas de performance
apropriadas para o seu problema. 
Por exemplo, no caso de classificação: precisão, revocação, F-measure, acurácia.

### Interpretação do modelo 1

Apresente os parâmetros do modelo obtido. Tentre mostrar as regras que são utilizadas no
processo de 'raciocínio' (*reasoning*) do sistema inteligente. Utilize medidas como 
o *feature importances* para tentar entender quais atributos o modelo se baseia no
processo de tomada de decisão.


### Resultados obtidos com o modelo 2.

Repita o passo anterior com os resultados do modelo 2.

### Interpretação do modelo 2

Repita o passo anterior com os parâmetros do modelo 2.


## Análise comparativa dos modelos

Discuta sobre as forças e fragilidades de cada modelo. Exemplifique casos em que um
modelo se sairia melhor que o outro. Nesta seção é possível utilizar a sua imaginação
e extrapolar um pouco o que os dados sugerem.


### Distribuição do modelo (opcional)

Tende criar um pacote de distribuição para o modelo construído, para ser aplicado 
em um sistema inteligente.


## 8. Conclusão

Apresente aqui a conclusão do seu trabalho. Discussão dos resultados obtidos no trabalho, 
onde se verifica as observações pessoais de cada aluno.

Uma conclusão deve ter 3 partes:

   * Breve resumo do que foi desenvolvido
	 * Apresenação geral dos resultados obtidos com discussão das vantagens e desvantagens do sistema inteligente
	 * Limitações e possibilidades de melhoria


# REFERÊNCIAS

Como um projeto de sistema inteligente não requer revisão bibliográfica, 
a inclusão das referências não é obrigatória. No entanto, caso você 
tenha utilizado referências na introdução ou deseje 
incluir referências relacionadas às tecnologias, padrões, ou metodologias 
que serão usadas no seu trabalho, relacione-as de acordo com a ABNT.

Verifique no link abaixo como devem ser as referências no padrão ABNT:

http://www.pucminas.br/imagedb/documento/DOC\_DSC\_NOME\_ARQUI20160217102425.pdf

Por exemplo:

**[1]** - _ELMASRI, Ramez; NAVATHE, Sham. **Sistemas de banco de dados**. 7. ed. São Paulo: Pearson, c2019. E-book. ISBN 9788543025001._

**[2]** - _COPPIN, Ben. **Inteligência artificial**. Rio de Janeiro, RJ: LTC, c2010. E-book. ISBN 978-85-216-2936-8._

**[3]** - _CORMEN, Thomas H. et al. **Algoritmos: teoria e prática**. Rio de Janeiro, RJ: Elsevier, Campus, c2012. xvi, 926 p. ISBN 9788535236996._

**[4]** - _SUTHERLAND, Jeffrey Victor. **Scrum: a arte de fazer o dobro do trabalho na metade do tempo**. 2. ed. rev. São Paulo, SP: Leya, 2016. 236, [4] p. ISBN 9788544104514._

**[5]** - _RUSSELL, Stuart J.; NORVIG, Peter. **Inteligência artificial**. Rio de Janeiro: Elsevier, c2013. xxi, 988 p. ISBN 9788535237016._



# APÊNDICES

**Colocar link:**

Do código (armazenado no repositório);

Dos artefatos (armazenado do repositório);

Da apresentação final (armazenado no repositório);

Do vídeo de apresentação (armazenado no repositório).




