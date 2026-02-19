# Análise do Transporte Interestadual – Pipeline de Dados e Power BI

Desenvolvimento baseado em dados públicos da Agência Nacional de Transportes Terrestres (ANTT), relacionados ao transporte rodoviário interestadual.

O projeto integrou o tratamento e a organização dos dados em Python com a construção de um dashboard analítico no Power BI. A proposta foi transformar dados brutos, originalmente distribuídos em múltiplos arquivos, em uma base estruturada, confiável e preparada para análise. O foco esteve na organização das informações, padronização dos dados e criação de indicadores que permitissem uma visão clara do comportamento das viagens interestaduais.

## Tratamento de Dados – Python
O tratamento foi realizado no script [Pipeline de Dados – ANTT.ipynb](https://github.com/KatiellySantos/projetos_PowerBI/blob/958a450873e6276e0996bc33611a2ded2404931e/Projeto_An%C3%A1lise%20do%20Transporte%20Interestadual/Pipeline%20de%20Dados%20%E2%80%93%20ANTT.ipynb), responsável por consolidar, padronizar e estruturar os dados antes da importação no Power BI.
A etapa contemplou:
- Consolidação de múltiplos arquivos CSV em um único dataset
- Tratamento de valores nulos
- Padronização textual
- Separação de cidade e estado
- Criação de variáveis derivadas (categoria de gratuidade)
- Renomeação e reorganização das colunas
- Exportação para banco SQLite

Essa etapa foi fundamental para garantir consistência, integridade e melhor desempenho na modelagem analítica.

## Modelagem e Visualização – Power BI
Com o dataset tratado e estruturado, foram desenvolvidas no Power BI:
- Medidas em DAX
- KPIs estratégicos
- Filtros interativos
- Visualizações analíticas

O dashboard permite análise temporal, geográfica e operacional dos dados, possibilitando identificar padrões de fluxo, concentração de passageiros e comportamento das rotas interestaduais.

## Indicadores Desenvolvidos
- Total de Passageiros
- Valor Médio das Tarifas
- Receita Estimada
- Cobertura de Estados
- Rotas Ativas

## Principais Análises
- Fluxo de bilhetes por mês
- Distribuição de bilhetes por estado
- Origem | Destino | Passageiros
- Distribuição por categoria de benefício tarifário

## Decisões Técnicas
Durante o desenvolvimento, algumas decisões foram adotadas para garantir melhor organização e desempenho:
- Utilização de Python para consolidar e padronizar os dados antes da importação no Power BI
- Estruturação de variáveis geográficas para segmentação eficiente
- Criação de medidas em DAX para garantir cálculos dinâmicos
- Armazenamento em SQLite como etapa intermediária

Essas decisões contribuíram para uma modelagem mais limpa e um dashboard mais eficiente.

O GIF abaixo apresenta a navegação entre páginas, aplicação de filtros e interação com os principais visuais, evidenciando a dinâmica da análise e a responsividade do modelo construído no Power BI.

<p align="center">
  <img src="analise_transporte_interestadual.gif" width="1100">
</p>

A visualização destaca o comportamento dos indicadores diante das segmentações temporais e geográficas, reforçando a proposta analítica desenvolvida.
