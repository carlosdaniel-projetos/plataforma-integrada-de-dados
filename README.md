
# Plataforma Integrada de Dados | Supply Chain

### Integração de informações, autonomia analítica e eficiência operacional

## Sobre o projeto

Quanto tempo um profissional de Planejamento e Compras dedica à preparação de dados antes de conseguir analisar as informações necessárias para tomar uma decisão?

Essa foi a questão que motivou a idealização de uma solução voltada à **centralização de informações operacionais e à simplificação dos processos de consulta e análise de produtos**.

Em operações com múltiplas lojas, consultar informações como estoque, vendas, custos e movimentações exigia acessar diferentes relatórios, realizar extrações individuais e consolidar manualmente os resultados em planilhas.

Além do tempo necessário, limitações dos sistemas de origem dificultavam a extração de grandes volumes de informações, tornando o processo ainda mais trabalhoso.

A partir desse cenário, idealizei uma plataforma integrada de dados, materializada no projeto **PRISMA — Plataforma de Resultados Integrados para Monitoramento e Análise**.

A proposta foi transformar informações dispersas em uma estrutura centralizada, acessível e personalizável, permitindo que os profissionais direcionassem **mais tempo à análise e menos à preparação dos dados**.

---

## Impacto da solução no negócio

Inicialmente concebida para atender às necessidades do Planejamento, a solução demonstrou potencial para beneficiar diferentes áreas da organização.

### Planejamento e Compras | Agilidade no abastecimento

A centralização de informações de estoque, vendas, cobertura e movimentação dos produtos simplificou as consultas necessárias ao planejamento do abastecimento.

Os profissionais passaram a contar com uma visão integrada dos produtos por loja, reduzindo a necessidade de extrações individuais e consolidações manuais.

### Operações | Acesso rápido às informações

A plataforma facilitou a localização de produtos e a consulta de informações específicas de cada unidade.

Essa disponibilidade contribuiu para agilizar consultas operacionais e ampliar a autonomia dos usuários no acesso aos dados.

### Diferentes áreas | Democratização da informação

A possibilidade de personalizar consultas e exportar informações em diferentes formatos ampliou a aplicabilidade da solução para além do setor de Planejamento.

Cada profissional passou a poder estruturar consultas de acordo com suas necessidades, sem depender de um relatório único e previamente definido.

### Resultados percebidos

O principal benefício foi a **otimização do tempo dedicado à obtenção e preparação de informações**.

O acompanhamento realizado diretamente com os setores usuários trouxe retornos positivos, especialmente relacionados à rapidez na identificação de produtos e à facilidade de acesso às informações por loja.

A solução contribuiu para transformar um processo operacionalmente trabalhoso em uma experiência mais ágil, integrada e orientada à análise.

---

## Funcionalidades e análises desenvolvidas

A plataforma foi idealizada para oferecer flexibilidade na exploração dos dados, permitindo que diferentes profissionais utilizassem as mesmas informações conforme suas necessidades.

### 1. Consultas personalizáveis

Uma tabela interativa permite:

- Selecionar, adicionar e remover campos.
- Reorganizar colunas e aplicar filtros.
- Estruturar consultas específicas por produto ou operação.
- Salvar diferentes modelos de consulta.
- Recuperar configurações anteriormente utilizadas.
- Compartilhar modelos entre profissionais por meio de arquivos JSON.

**Benefício:** redução do retrabalho e maior autonomia nas consultas recorrentes.

### 2. Visualizações sob demanda

Além das consultas tabulares, a solução disponibiliza um ambiente para construção de gráficos personalizados.

Os usuários podem selecionar diferentes tipos de gráficos, métricas, dimensões e filtros, criando visualizações rápidas para análises e apresentações.

Os painéis podem ser organizados, salvos e exportados conforme a necessidade do profissional.

**Benefício:** acesso à análise visual sem depender da criação de novos dashboards pela equipe de BI.

### 3. Indicadores operacionais e analíticos

Entre as informações estruturadas para consulta estão:

| Indicador | Aplicação |
|---|---|
| Estoque disponível | Quantidade de produtos por unidade |
| Vendas | Quantidade vendida e receita |
| Média de vendas | Referência para análise da demanda |
| Maior volume de vendas | Identificação de picos de demanda |
| Cobertura de estoque | Estimativa de dias de atendimento da demanda |
| Dias sem venda | Identificação de ausência de movimentação comercial |
| Estoque em trânsito | Acompanhamento de produtos em processo de recebimento |
| Custos | Análise de custo unitário e valor total |
| Curva de produtos | Classificação da relevância comercial dos itens |

### 4. Classificação de produtos | Curva A, B, C e E

Foi estruturada uma metodologia de classificação que considera duas perspectivas complementares:

**Receita líquida:** participação financeira de cada produto no resultado comercial da loja.

**Quantidade vendida:** participação de cada produto no volume total comercializado.

A partir de análises de Pareto por loja, os produtos são ordenados e classificados conforme sua participação acumulada:

- **Curva A:** até 80%.
- **Curva B:** acima de 80% até 95%.
- **Curva C:** acima de 95% até 99%.
- **Curva E:** acima de 99%.

Posteriormente, as classificações de receita e quantidade são combinadas por regras de negócio específicas, resultando em uma **classificação multicritério personalizada**.

Produtos sem movimentação comercial também recebem identificação específica.

Essa abordagem amplia a compreensão do desempenho dos produtos e oferece informações para apoiar decisões de abastecimento, priorização e acompanhamento comercial.

### 5. Exportação e compartilhamento

As informações podem ser exportadas em diferentes formatos:

- **Excel (.xlsx):** análises e planilhas operacionais.
- **CSV:** manipulação de bases tabulares.
- **JSON:** integrações e aplicações.
- **Parquet:** processamento e análises de grandes volumes de dados.

A flexibilidade de exportação amplia as possibilidades de utilização das informações por diferentes equipes.

---

## Demonstração visual

Esta seção apresentará versões demonstrativas das principais funcionalidades da solução.

As demonstrações serão organizadas em três perspectivas:

1. **Consulta integrada:** centralização das informações e personalização da tabela.
2. **Análises visuais:** construção de gráficos e painéis sob demanda.
3. **Modelos reutilizáveis:** criação, recuperação e compartilhamento de configurações.

> **Nota:** todas as demonstrações utilizarão dados inteiramente fictícios, preservando a proposta funcional sem divulgar informações corporativas.

---

## Desafios enfrentados no desenvolvimento

### Fragmentação das informações

O primeiro desafio foi compreender como informações essenciais ao processo de abastecimento estavam distribuídas entre diferentes consultas e relatórios.

Foi necessário identificar as fontes, mapear os procedimentos de extração e estruturar as necessidades de integração dos dados.

### Viabilização das fontes automatizadas

Parte das informações dependia de extrações manuais realizadas em sistemas internos.

A partir do mapeamento desses processos, foram levantados os requisitos necessários para a disponibilização automatizada das informações.

Esse trabalho envolveu alinhamentos com as equipes de Engenharia de Dados e TI, responsáveis pelo desenvolvimento dos processos de extração e das DAGs.

### Estruturação das regras analíticas

Outro desafio foi transformar dados provenientes de diferentes fontes em informações prontas para análise.

Indicadores como cobertura de estoque e classificação de produtos exigiram a combinação de dados, a definição de regras de negócio e a validação dos resultados.

As regras analíticas foram previamente estruturadas em ambiente de Business Intelligence e utilizadas como referência funcional para o desenvolvimento da plataforma.

### Experiência e autonomia dos usuários

A solução precisava atender diferentes necessidades sem exigir a criação de um relatório específico para cada solicitação.

Por isso, a proposta funcional priorizou consultas personalizáveis, modelos reutilizáveis, visualizações sob demanda e diferentes formatos de exportação.

---

## Arquitetura e fluxo de dados

A solução foi estruturada a partir de fontes operacionais corporativas, com processos automatizados de extração e disponibilização das informações.

**Fluxo conceitual:**

`Sistemas operacionais → ETL e DAGs → Azure Data Lake Storage → Integração das informações → Plataforma de consulta e análise`

A organização das informações considera dados transacionais, como estoque e vendas, associados a dimensões de produtos e unidades operacionais.

Essa estrutura permite relacionar diferentes indicadores ao mesmo produto e à mesma operação, oferecendo uma visão consolidada para consulta.

As informações são disponibilizadas com atualização diária, conforme os processos automatizados de alimentação das bases.

---

## Tecnologias e ferramentas utilizadas

| Tecnologia | Aplicação |
|---|---|
| Power BI | Estruturação e validação prévia dos indicadores |
| DAX | Desenvolvimento das regras analíticas utilizadas como referência |
| Azure Data Lake Storage | Armazenamento e disponibilização das informações |
| ETL e DAGs | Processos de extração e atualização desenvolvidos pelas equipes técnicas |
| Plataforma web interna | Ambiente de consulta e visualização |
| Excel, CSV, JSON e Parquet | Exportação e compartilhamento de informações |

---

## Minha atuação no projeto

Atuei como **Analista de Planejamento com foco em Dados e Business Intelligence**, conectando as necessidades operacionais à concepção de uma solução tecnológica.

Minhas principais responsabilidades envolveram:

- Identificação das dificuldades enfrentadas pelos profissionais na obtenção das informações.
- Idealização da solução e definição de seus objetivos.
- Levantamento de necessidades junto às áreas de negócio.
- Mapeamento das fontes e dos processos de extração.
- Definição dos indicadores e das regras analíticas.
- Estruturação e validação dos cálculos em ambiente de BI.
- Especificação das funcionalidades e da experiência desejada para os usuários.
- Interface com Engenharia de Dados, TI e desenvolvimento.
- Acompanhamento da implantação e coleta de feedback dos usuários.

A implementação técnica da aplicação web e o desenvolvimento dos pipelines e DAGs foram realizados pelas equipes especializadas, com base nas necessidades e regras de negócio levantadas.

**O projeto demonstra minha capacidade de identificar oportunidades de melhoria, transformar necessidades operacionais em requisitos funcionais e contribuir para a construção de soluções orientadas por dados.**

---

## Confidencialidade

Este repositório apresenta um estudo de caso profissional com finalidade demonstrativa.

As demonstrações visuais utilizarão exclusivamente dados fictícios, sem identificação da empresa ou divulgação de informações comerciais, códigos internos, credenciais, bases corporativas ou componentes proprietários.

O objetivo é apresentar o problema de negócio, a concepção da solução, as competências aplicadas e os benefícios operacionais, preservando a confidencialidade das informações corporativas.
