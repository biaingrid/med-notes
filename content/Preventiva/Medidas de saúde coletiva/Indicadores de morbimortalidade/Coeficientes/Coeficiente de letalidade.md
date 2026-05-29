### Definição 
O **coeficiente de letalidade** (também chamado de **taxa de letalidade de casos** ou **case fatality rate - CFR**) é a **proporção de óbitos causados por uma determinada doença em relação ao total de pessoas diagnosticadas com essa doença em um período específico**. Este indicador é convencionalmente expresso como **percentual** e representa uma **medida da gravidade da doença**.

>[!warning] Conceito
>Proporção de **óbitos** causados por uma determinada doença **em relação** **ao total** de pessoas **diagnosticadas** com essa doença em um **período** específico. 

Fórmula:
 $$
\text{Coeficiente de letalidade} =
\frac{\text{Número de óbitos pela doença}}
{\text{Número total de casos diagnosticados}}
X  100
$$
### Diferenças entre indicadores
| Indicador                           | Definição                                              | Numerador             | Denominador                                  |
| ----------------------------------- | ------------------------------------------------------ | --------------------- | -------------------------------------------- |
| **Coeficiente de Letalidade (CFR)** | Proporção de mortes entre os casos diagnosticados      | Óbitos pela doença    | Total de casos diagnosticados                |
| **Taxa de Mortalidade**             | Número de mortes em uma população por unidade de tempo | Óbitos pela doença    | População total (por 100.000 habitantes/ano) |
| **Taxa de Recuperação**             | Proporção de pacientes que se recuperam                | Pacientes recuperados | Total de casos diagnosticados                |
**Diferença crítica**: <mark style="background:#fff88f">A taxa de mortalidade mede o impacto da doença na população geral,</mark> enquanto o coeficiente de letalidade mede a gravidade da doença entre aqueles que foram diagnosticados.

### Fatores que influenciam o coeficiente de letalidade
#### 1. Definição de Caso
A Organização Mundial da Saúde (OMS) estabelece diferentes definições de caso que afetam diretamente o cálculo do coeficiente de letalidade:
- **Caso confirmado**: Pessoa com confirmação laboratorial da infecção, independentemente de sinais e sintomas clínicos
- **Caso suspeito**: Pessoa que atende critérios clínicos E epidemiológicos
- **Caso provável**: Paciente que atende critérios clínicos E é contato de caso provável/confirmado

**Exemplo prático**: Durante a epidemia inicial de COVID-19 na China continental, o coeficiente de letalidade foi de 3,7% quando apenas doença moderada a grave foi incluída no denominador. Quando casos leves foram incluídos, o mesmo estudo calculou um coeficiente de 1,4%.
#### 2. Características Demográficas
O coeficiente de letalidade apresenta **forte dependência da idade**: 
- Pacientes >60 anos: 6,4%
- Pacientes >80 anos: 13,4%
#### 3. Viés de Tempo (Time Lag)
Um dos principais desafios no cálculo do coeficiente de letalidade é o **intervalo de tempo entre a confirmação do caso e o óbito**. O método direto (óbitos totais/casos totais) é simplista e não considera esse atraso temporal essencial, levando frequentemente a **estimativas subestimadas**, especialmente nos estágios iniciais de surtos.
#### 4. Subnotificação e Testagem Incompleta
A notificação incompleta do número de indivíduos infectados (tanto recuperados quanto falecidos) pode levar a **estimativas enviesadas** do coeficiente de letalidade. A subtestagem e populações heterogêneas são fontes importantes de incerteza nos dados.

### Método de cálculo
**Método tradicional**

$$
\text{CFR} =
\frac{\text{Óbitos confirmados até a data}}
{\text{Casos confirmados até a data}}
X 100
$$
**Limitações**: Não considera o intervalo de tempo entre confirmação e óbito, nem atrasos de notificação.

**Métodos avançados**
Pesquisadores desenvolveram métodos mais sofisticados que incorporam a **distribuição do tempo entre caso e óbito** sem exigir suposições prévias sobre parâmetros de distribuição. Esses métodos recuperam o coeficiente de letalidade verdadeiro muito mais cedo que o método direto em várias configurações de simulação.

### Aplicações práticas
**Vigilância Epidemiológica**
O coeficiente de letalidade é um **indicador crucial do risco de uma doença** durante surtos epidêmicos. Estimá-lo de forma precisa e rápida é fundamental quando uma doença epidemiológica está prevalente.

**Alocação de Recursos**
Saber quais populações estão em maior risco de desfechos graves é **crucial para decidir a alocação ótima de recursos** durante uma resposta a surtos.

**Comparação entre Doenças**
O coeficiente de letalidade permite comparar a gravidade de diferentes doenças:
- COVID-19 (China, casos moderados a graves): 3,7% 
- COVID-19 (China, incluindo casos leves): 1,4% 
- Pandemia de influenza H1N1 2009: substancialmente menor que COVID-19 
- Bacteremia por Staphylococcus aureus de origem comunitária: 20,3% (MSSA 20,2%, MRSA 22,3%)

### Limitações e vieses
#### Vieses na Estimativa Absoluta
1. **Identificação preferencial de casos graves**: Casos mais graves são mais provavelmente identificados 
2. **Viés de atraso de notificação**: Atrasos entre infecção, diagnóstico e notificação de óbito 
#### Vieses na Estimativa Relativa
Ao comparar coeficientes de letalidade entre grupos (por exemplo, para avaliar impacto de intervenções): 
1. **Confundimento**: Variáveis não controladas que afetam tanto a exposição quanto o desfecho
2. **Viés de sobrevivência**: Inclusão apenas de pacientes que sobreviveram tempo suficiente para receber intervenção
3. **Viés de seleção**: Inclusão preferencial de hospitalizados e/ou óbitos em conjuntos de dados de vigilância
**Recomendação**: Cautela na interpretação causal de coeficientes de letalidade diferenciais entre grupos que recebem diferentes intervenções em conjuntos de dados observacionais.

### Informações complementares
#### Coeficiente de Letalidade vs. Probabilidade Individual de Morte
O coeficiente de letalidade calculado pelo método tradicional **não representa diretamente a probabilidade de morte de um indivíduo infectado**. [4] Modelos de probabilidade de sobrevivência e modelos SIR (Suscetível-Infectado-Recuperado) dependentes da duração da infecção são necessários para definir estimativas individuais e populacionais de medidas dinâmicas de mortalidade.
#### Tendências Temporais
Estudos de vigilância populacional demonstram que o coeficiente de letalidade e a taxa de mortalidade fornecem **informações complementares**. Por exemplo, na bacteremia por _S. aureus_:
- Coeficiente de letalidade de MSSA permaneceu estável, mas a taxa de mortalidade aumentou
- Coeficiente de letalidade de MRSA diminuiu, enquanto sua taxa de mortalidade permaneceu baixa

Isso destaca a importância de avaliar **ambos os indicadores** para compreender completamente o impacto da doença.

### Contexto brasileiro
Embora as diretrizes internacionais sejam amplamente aplicáveis, o Brasil utiliza o coeficiente de letalidade como indicador fundamental em seus sistemas de vigilância epidemiológica. O Ministério da Saúde e as Secretarias Estaduais de Saúde monitoram regularmente este indicador para doenças de notificação compulsória, incluindo dengue, COVID-19, febre amarela, meningites, entre outras.
A interpretação adequada do coeficiente de letalidade requer considerar as definições de caso utilizadas, a qualidade da vigilância epidemiológica, a cobertura de testagem e as características demográficas da população afetada. Durante surtos e epidemias, estimativas precoces devem ser interpretadas com cautela devido aos vieses temporais e de notificação descritos acima.

>[!note] Tags
> #coeficiente #letalidade #viés #vieses #CFR 

