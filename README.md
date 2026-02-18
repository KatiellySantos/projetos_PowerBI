Análise do Transporte Interestadual – Pipeline de Dados e Power BI

Desenvolvimento baseado em dados públicos da Agência Nacional de Transportes Terrestres (ANTT), relacionados ao transporte rodoviário interestadual.

O projeto integrou o tratamento e a organização dos dados em Python com a construção de um dashboard analítico no Power BI. A proposta foi transformar dados brutos, originalmente distribuídos em múltiplos arquivos, em uma base estruturada, confiável e preparada para análise. O foco esteve na organização das informações, padronização dos dados e criação de indicadores que permitissem uma visão clara do comportamento das viagens interestaduais.

Tratamento de Dados – Python

O tratamento foi realizado no script Pipeline_de_Dados_–_ANTT.py, responsável por consolidar, padronizar e estruturar os dados antes da importação no Power BI.

A etapa contemplou:

Consolidação de múltiplos arquivos CSV em um único dataset

Tratamento de valores nulos

Padronização textual

Separação de cidade e estado

Criação de variáveis derivadas (categoria de gratuidade)

Renomeação e reorganização das colunas

Exportação para banco SQLite

Essa etapa foi fundamental para garantir consistência, integridade e melhor desempenho na modelagem analítica.

Modelagem e Visualização – Power BI

Com o dataset tratado e estruturado, foram desenvolvidas no Power BI:

Medidas em DAX

KPIs estratégicos

Filtros interativos

Visualizações analíticas

O dashboard permite análise temporal, geográfica e operacional dos dados, possibilitando identificar padrões de fluxo, concentração de passageiros e comportamento das rotas interestaduais.

Indicadores Desenvolvidos

Total de Passageiros

Valor Médio das Tarifas

Receita Estimada

Cobertura de Estados

Rotas Ativas

Principais Análises

Fluxo de bilhetes por mês

Distribuição de bilhetes por estado

Origem x Destino x Passageiros

Distribuição por categoria de benefício tarifário