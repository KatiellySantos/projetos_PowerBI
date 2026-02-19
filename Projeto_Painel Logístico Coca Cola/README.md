# Análise Logística Estratégica – Performance Operacional

Desenvolvido com base em operações logísticas simuladas da Coca-Cola, com foco na transformação de dados operacionais em indicadores estratégicos de desempenho.

A proposta foi estruturar um modelo analítico capaz de apoiar decisões relacionadas à eficiência logística, controle de custos e nível de serviço (SLA), utilizando modelagem dimensional e métricas dinâmicas em DAX.

O dashboard foi construído priorizando clareza, objetividade e capacidade de análise multidimensional.

## Objetivo Estratégico

Desenvolver um painel gerencial que permita:
- Monitorar a performance logística
- Avaliar o nível de serviço das entregas
- Comparar desempenho entre centros de distribuição
- Analisar impacto financeiro por produto e tipo de transporte
- Identificar oportunidades de melhoria operacional

O foco não foi apenas visualização, mas geração de insight para suporte à decisão.

## Arquitetura de Dados
O modelo foi estruturado em formato **Star Schema**, separando claramente:

🔹 **Tabela Fato – Entregas**

Base central contendo métricas operacionais:
- Quantidade transportada
- Distância média
- Custo por entrega
- Tempo de entrega
- Status (no prazo / atraso)

🔹 **Dimensões**
- Produtos
- Veículos
- Centros de Distribuição (CDs)
- Tempo
  
Essa modelagem garante:

- Escalabilidade
- Melhor performance de consulta
- Clareza nas relações
- Facilidade de expansão do modelo

## Indicadores Estratégicos (KPIs)
O dashboard foi estruturado com foco nas seguintes métricas:

- Total de Entregas
- Entregas Dentro do Prazo (%)
- Tempo Médio de Entrega
- Custo Médio por Entrega
- Volume Total Transportado

Esses indicadores permitem avaliar simultaneamente volume operacional, eficiência logística e nível de serviço.

## Análises de Negócio

O painel foi dividido em duas páginas analíticas.

Na primeira página, o foco está na performance operacional, com análises como:
- **Entregas por CD x Entregas Dentro do Prazo por CD**, permitindo comparar volume e SLA entre centros de distribuição.
- **Custo Médio por CD x Tempo Médio de Entrega por Região**, evidenciando a relação entre eficiência operacional e impacto financeiro.

Na segunda página, o foco é eficiência e custo:
- **Quantidade Transportada por Veículo**, possibilitando avaliar a distribuição de volume por tipo de transporte.
- **Top 10 Produtos com Maior Custo Logístico**, destacando itens com maior impacto financeiro na operação.

O modelo também utiliza tooltips analíticos personalizados, permitindo aprofundamento sem comprometer a clareza visual:
- No gráfico de veículos, o tooltip apresenta número de entregas, distância média, custo médio por entrega e taxa de atraso.
- No gráfico de produtos, o tooltip detalha o custo de entrega por marca.
  
A estrutura favorece análise comparativa, segmentação por CD e período e exploração dinâmica dos dados.

## Decisões Técnicas
Durante o desenvolvimento, foram adotadas decisões voltadas para boas práticas de BI:
- Separação clara entre fato e dimensões
- Criação de medidas DAX para cálculos dinâmicos
- Segmentação por Centro de Distribuição e período
- Uso de tooltips personalizados para aprofundamento analítico
- Organização visual orientada à análise comparativa

A abordagem prioriza não apenas visualização, mas modelagem consistente e raciocínio analítico aplicado ao contexto logístico.

O GIF abaixo apresenta a navegação entre páginas, aplicação de filtros e interação com os principais visuais, evidenciando a dinâmica da análise e a responsividade do modelo construído no Power BI.

<p align="center">
  <img src="painel_logístico_coca_cola.gif" width="1100">
</p>

Simulação de um cenário corporativo de BI com foco em performance logística, controle de custos e monitoramento de nível de serviço.
