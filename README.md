# **Relatório de Análise de Dados: Padrões de Uso das Bicicletas Compartilhadas Yulu**

## **Introdução e Objetivos**

Este projeto teve como objetivo principal investigar os padrões de utilização do sistema de bicicletas compartilhadas Yulu, buscando compreender como diferentes fatores influenciam a demanda pelo serviço. Através de uma análise abrangente dos dados históricos, buscamos responder a perguntas cruciais para o negócio:

- Como a demanda varia ao longo do ano?
- Quais são os horários de maior e menor utilização?
- Qual o perfil predominante dos usuários?
- Como as condições climáticas afetam o uso do serviço?

Esta análise foi conduzida utilizando técnicas de exploração de dados, estatística descritiva e visualização, com o propósito de fornecer insights acionáveis para a equipe de operações, marketing e planejamento estratégico da Yulu.

## **Metodologia e Abordagem Analítica**

Para alcançar nossos objetivos, realizamos uma série de análises complementares:

1. **Análise Temporal**:
   - Sazonalidade ao longo do ano
   - Padrões diários e horários
   - Comparação entre dias úteis e fins de semana

2. **Análise de Segmentação**:
   - Comportamento de usuários registrados versus casuais
   - Diferenças por tipo de dia (úteis, feriados, fins de semana)

3. **Análise de Fatores Externos**:
   - Impacto das condições meteorológicas
   - Relação com temperatura e umidade

4. **Análise de Correlações**:
   - Identificação de relações entre variáveis
   - Padrões ocultos nos dados

Utilizamos ferramentas como Python (Pandas, Matplotlib, Seaborn) para processamento e visualização dos dados, garantindo que cada análise fosse rigorosa e reprodutível.

## **Dicionário Completo de Dados**

Para garantir a clareza na interpretação dos resultados, apresentamos abaixo o detalhamento completo das variáveis analisadas:

| **Variável**       | **Descrição Detalhada**                                                                 | **Tipo**      | **Valores/Intervalos**                     |
|--------------------|----------------------------------------------------------------------------------------|---------------|--------------------------------------------|
| **datetime**       | Carimbo de data e hora exata do registro                                              | DateTime      | Formato: YYYY-MM-DD HH:MM:SS              |
| **season**         | Representação das estações do ano                                                     | Categórica    | 1: Primavera, 2: Verão, 3: Outono, 4: Inverno |
| **holiday**        | Indica se o dia era feriado                                                           | Binária       | 0: Não, 1: Sim                             |
| **workingday**     | Indica se o dia era útil (não-fim de semana, não-feriado)                             | Binária       | 0: Não, 1: Sim                             |
| **weather**        | Condições climáticas no momento do registro                                           | Categórica    | 1: Limpo, 2: Nublado, 3: Chuva leve, 4: Chuva forte |
| **temp**           | Temperatura ambiente em graus Celsius                                                 | Contínua      | Escala em °C                               |
| **atemp**          | Temperatura aparente/sensação térmica em graus Celsius                                | Contínua      | Escala em °C                               |
| **humidity**       | Umidade relativa do ar em porcentagem                                                 | Contínua      | 0-100%                                     |
| **windspeed**      | Velocidade do vento em km/h                                                           | Contínua      | Valores positivos                          |
| **casual**         | Quantidade de aluguéis por usuários não registrados                                   | Discreta      | Inteiros não-negativos                     |
| **registered**     | Quantidade de aluguéis por usuários registrados                                       | Discreta      | Inteiros não-negativos                     |
| **count**          | Total de aluguéis (soma de usuários casuais e registrados)                           | Discreta      | Inteiros não-negativos                     |

## **Aplicações e Impacto Potencial**

Os resultados desta análise possuem diversas aplicações práticas para o negócio:

**1. Otimização Operacional:**
   - Planejamento inteligente da frota com base nos padrões sazonais e horários identificados
   - Programação de manutenção preventiva durante períodos de baixa demanda
   - Ajuste na distribuição geográfica das bicicletas

**2. Estratégias de Marketing:**
   - Desenvolvimento de campanhas segmentadas por perfil de usuário
   - Criação de programas de fidelidade e incentivos
   - Personalização de comunicações com base no comportamento dos usuários

**3. Planejamento Estratégico:**
   - Projeções de demanda em diferentes cenários
   - Identificação de oportunidades de expansão
   - Avaliação de impacto de eventos especiais

**4. Experiência do Usuário:**
   - Melhoria na disponibilidade nos horários e locais de maior demanda
   - Desenvolvimento de funcionalidades personalizadas
   - Antecipação de necessidades com base nos padrões identificados

Os resultados completos, com todas as descobertas específicas e visualizações, estão disponíveis no notebook de análise anexo a este relatório. Cada seção do código está devidamente comentada para facilitar a compreensão e reprodução da análise.

Esta investigação representa um passo importante na transformação de dados brutos em insights acionáveis, proporcionando à Yulu uma base sólida para decisões estratégicas fundamentadas.
