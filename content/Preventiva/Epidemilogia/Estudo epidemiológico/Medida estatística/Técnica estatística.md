### Introdução
As **técnicas estatísticas** são ferramentas fundamentais para a pesquisa clínica e médica, permitindo que profissionais de saúde analisem dados, testem hipóteses e tomem decisões baseadas em evidências. A estatística médica divide-se em duas categorias principais: **estatística descritiva** (que resume e descreve características dos dados) e **estatística inferencial** (que testa hipóteses e faz inferências sobre populações a partir de amostras).

### Tipos de dados em pesquisa clínica
**Dados Contínuos**
- Variáveis mensuráveis em escala numérica (peso, altura, pressão arterial, níveis laboratoriais)
- Podem assumir qualquer valor dentro de um intervalo
- Analisados com média, mediana e desvio padrão

**Dados Binários (Dicotômicos)**
- Apenas duas categorias possíveis (sim/não, vivo/morto, doente/saudável)
- Expressos como proporções ou porcentagens
- Fundamentais para cálculo de risco relativo e odds ratio

**Dados de Contagem**
- Números inteiros que representam frequências (número de hospitalizações, episódios de dor)
- Seguem distribuições específicas como Poisson ou binomial negativa

**Dados Multinomiais**
- Variáveis categóricas com mais de duas categorias (estágios de câncer, grupos sanguíneos)
- Podem ser ordinais (com ordem) ou nominais (sem ordem)

**Dados de Tempo até Evento (Sobrevida)**
- Medem o tempo até ocorrência de um desfecho (morte, recorrência, cura)
- Requerem análises especiais como curvas de Kaplan-Meier e modelos de Cox

### Estatística descritiva
**Medidas de Tendência Central** 
- **Média**: soma de todos os valores dividida pelo número de observações
- **Mediana**: valor central quando dados estão ordenados (mais resistente a valores extremos)
- **Moda**: valor mais frequente no conjunto de dados

**Medidas de Dispersão** 
- **Desvio padrão**: quantifica a variabilidade dos dados em torno da média
- **Erro padrão da média**: estima a variação da média amostral em relação à média populacional
- **Intervalo interquartil**: diferença entre o 3º e 1º quartil, útil para dados não-normais

### Testes de hipóteses
**Conceitos Fundamentais** 
A testagem de hipóteses envolve:
- **Hipótese nula (H₀)**: assume que não há diferença ou efeito
- **Hipótese alternativa (H₁)**: propõe que existe diferença ou efeito
- **Valor p**: probabilidade de obter os resultados observados se a hipótese nula for verdadeira
- **Nível de significância**: convencionalmente estabelecido em 0,05 (5%)

**Tipos de Erros**
- **Erro Tipo I (α)**: rejeitar a hipótese nula quando ela é verdadeira (falso positivo)
- **Erro Tipo II (β)**: não rejeitar a hipótese nula quando ela é falsa (falso negativo)
- **Poder estatístico (1-β)**: probabilidade de detectar um efeito real quando ele existe

>[!info] Diagrama de teste estatístico de tomador de decisão
>![[Pasted image 20260526191235.png]]

### Testes estatísticos paramétricos
**Teste t de Student** 
- **Teste t de uma amostra**: compara a média de uma amostra com um valor conhecido
- **Teste t independente**: compara médias entre dois grupos independentes
- **Teste t pareado**: compara médias de medidas repetidas no mesmo grupo
_Pressupostos_: dados contínuos, distribuição normal, variâncias homogêneas

**Análise de Variância (ANOVA)**
- Compara médias entre três ou mais grupos
- **ANOVA de uma via**: um fator independente
- **ANOVA de medidas repetidas**: medições múltiplas no mesmo sujeito
- **ANOVA fatorial**: múltiplos fatores independentes
_Pressupostos_: normalidade, homogeneidade de variâncias, independência das observações

### Testes Estatísticos Não-Paramétricos
Utilizados quando os dados não atendem aos pressupostos dos testes paramétricos (distribuição não-normal, dados ordinais, amostras pequenas): 
- **Teste de Mann-Whitney (Wilcoxon rank-sum)**: alternativa ao teste t independente
- **Teste de Wilcoxon signed-rank**: alternativa ao teste t pareado
- **Teste de Kruskal-Wallis**: alternativa à ANOVA de uma via
- **Teste de Friedman**: alternativa à ANOVA de medidas repetidas

### Testes para Dados Categóricos
**Teste Qui-quadrado (χ²)** 
- Avalia associação entre variáveis categóricas
- Compara frequências observadas com frequências esperadas
- Requer contagens esperadas ≥5 em cada célula

**Teste Exato de Fisher**
- Alternativa ao qui-quadrado para amostras pequenas
- Calcula probabilidade exata sem aproximações

### Análise de correlação e regressão
**Correlação** 
- **Correlação de Pearson (r)**: mede associação linear entre duas variáveis contínuas (varia de -1 a +1)
- **Correlação de Spearman (ρ)**: versão não-paramétrica, baseada em ranks
- Importante: correlação não implica causalidade

**Regressão Linear**
- Modela relação entre variável dependente contínua e uma ou mais variáveis independentes
- Permite predição e controle de confundidores
- Equação: Y = β₀ + β₁X₁ + β₂X₂ + ... + ε

**Regressão Logística** 
- Utilizada quando o desfecho é binário (doença sim/não)
- Produz odds ratios ajustados
- Fundamental em estudos caso-controle

### Análise de Sobrevida
**Curvas de Kaplan-Meier** 
- Estimam probabilidade de sobrevida ao longo do tempo
- Consideram dados censurados (pacientes perdidos no seguimento)
- Comparação entre grupos: teste log-rank

**Modelo de Riscos Proporcionais de Cox** 
- Regressão multivariada para dados de tempo até evento
- Calcula hazard ratios ajustados
- Permite controle de múltiplos fatores prognósticos

**Medidas de Associação em Estudos Clínicos**

| Tipo de Estudo             | Medida de Associação         | Interpretação                                          |
| -------------------------- | ---------------------------- | ------------------------------------------------------ |
| Ensaio Clínico Randomizado | Risco Relativo (RR)          | RR > 1: aumento de risco; RR 1: redução de risco       |
| Estudo de Coorte           | Risco Relativo (RR)          | Razão entre incidências nos grupos exposto/não-exposto |
| Estudo Caso-Controle       | Odds Ratio (OR)              | Razão entre chances de exposição em casos/controles    |
| Testes Diagnósticos        | Sensibilidade/Especificidade | Capacidade de detectar doença/excluir doença           |
### Intervalos de Confiança
Os **intervalos de confiança (IC)** fornecem um intervalo plausível de valores para o parâmetro populacional, geralmente com 95% de confiança: 
- IC que não inclui o valor nulo (1,0 para RR/OR; 0 para diferenças) indica significância estatística
- Fornecem informação sobre magnitude do efeito e precisão da estimativa
- Mais informativos que valores p isolados

### Testes diagnósticos
**Parâmetros de Desempenho** 
- **Sensibilidade**: proporção de doentes corretamente identificados (verdadeiros positivos)
- **Especificidade**: proporção de não-doentes corretamente identificados (verdadeiros negativos)
- **Valor Preditivo Positivo (VPP)**: probabilidade de doença quando teste é positivo
- **Valor Preditivo Negativo (VPN)**: probabilidade de ausência de doença quando teste é negativo

**Curva ROC (Receiver Operating Characteristic)** 
- Gráfico de sensibilidade versus (1-especificidade)
- Área sob a curva (AUC) mede acurácia global do teste
- AUC = 0,5: teste sem valor discriminatório; AUC = 1,0: teste perfeito

### Diretrizes para Análise Estatística
**Plano de Análise Estatística (SAP)** 
Segundo diretrizes internacionais, um SAP completo deve incluir:
- Descrição detalhada das análises primárias e secundárias
- Métodos para lidar com dados faltantes
- Estratégias para análises de subgrupos
- Ajustes para comparações múltiplas
- Análises de sensibilidade

**Diretrizes de Reporte**
- **CONSORT**: ensaios clínicos randomizados
- **STROBE**: estudos observacionais
- **TRIPOD**: modelos de predição
- **REMARK**: estudos de marcadores prognósticos
- **AMSTAR**: revisões sistemáticas

### Considerações Especiais
**Comparações Múltiplas** 
- Múltiplos testes aumentam risco de erro Tipo I
- Correções necessárias: Bonferroni, Holm, ou False Discovery Rate (FDR)
- Definir desfecho primário a priori reduz necessidade de ajustes

**Tamanho Amostral** 
- Deve ser calculado antes do estudo
- Depende de: diferença clinicamente relevante, variabilidade esperada, poder desejado (geralmente 80-90%), nível de significância (geralmente 5%)

**Dados Faltantes**
- Podem introduzir viés se não tratados adequadamente
- Métodos: análise de casos completos, imputação múltipla, modelos de máxima verossimilhança

### Contexto Brasileiro
Embora as técnicas estatísticas sejam universais, a aplicação em pesquisa clínica no Brasil deve seguir:
- **Resolução CNS 466/2012 e 510/2016**: normas éticas para pesquisa envolvendo seres humanos
- **REBEC (Registro Brasileiro de Ensaios Clínicos)**: registro obrigatório de ensaios clínicos
- **Diretrizes metodológicas da CONITEC**: para avaliação de tecnologias em saúde no SUS
- **Normas da ANVISA**: para estudos de registro de medicamentos e dispositivos

As análises estatísticas devem ser conduzidas com rigor metodológico, transparência e reprodutibilidade, sempre com suporte de estatístico qualificado quando necessário. A escolha adequada do teste estatístico depende do tipo de dados, desenho do estudo e pressupostos estatísticos, sendo fundamental para a validade das conclusões da pesquisa clínica.

>[!note] Tags
> #teste #estatística 

