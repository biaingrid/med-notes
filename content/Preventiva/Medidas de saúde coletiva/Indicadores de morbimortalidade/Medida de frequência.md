### Introdução
As **medidas de frequência** são ferramentas fundamentais em epidemiologia que quantificam a ocorrência de doenças ou eventos de saúde em populações. As principais medidas são **incidência** (casos novos) e **prevalência** (casos existentes), cada uma com aplicações específicas no planejamento de saúde, pesquisa etiológica e avaliação de intervenções.

### Conceitos fundamentais
**Incidência** refere-se à <mark style="background:#fff88f">ocorrência de novos casos</mark> de uma doença durante um período específico de tempo. É utilizada principalmente para avaliar etiologia, fatores de risco e eficácia de medidas preventivas. 

**Prevalência** refere-se à <mark style="background:#fff88f">existência de casos (novos e antigos)</mark> de uma doença em um determinado momento ou período. Reflete a carga da doença na população e é essencial para planejamento de recursos e serviços de saúde.

### Tipos de incidência
#### Incidência Cumulativa (Risco)
A incidência cumulativa expressa a proporção de pessoas que desenvolvem a doença durante um período específico.
Fórmula:
$$
\text{Incidência cumulativa} =
\frac{\text{Número de casos novos em um período}}
{\text{População em risco no início do período}}
X 100
$$
**Características:**
- Expressa como proporção ou percentual
- Requer população fechada (sem entrada ou saída)
- Período de observação fixo
- Varia de 0 a 1 (ou 0% a 100%)

**Exemplo:** Em uma coorte de 1.000 trabalhadores acompanhados por 5 anos, 50 desenvolveram diabetes. A incidência cumulativa = 50/1.000 = 0,05 ou 5%.

#### Taxa de incidência (densidade de incidência)
A taxa de incidência considera o tempo que cada pessoa permanece em risco, sendo mais apropriada para populações dinâmicas.
Fórmula:

$$
\text{Taxa de Incidência} =
\frac{\text{Número de casos novos}}
{\text{Soma de pessoas-tempo em risco}}
$$

**Características:**
- Expressa como casos por pessoa-tempo (por exemplo, casos/1.000 pessoas-ano)
- Apropriada para populações dinâmicas
- Considera perdas de seguimento e riscos competitivos
- Não tem limite superior

**Exemplo:** Se 50 casos de diabetes ocorreram em 4.500 pessoas-ano de seguimento, a taxa de incidência = 50/4.500 = 11,1 casos por 1.000 pessoas-ano.

|         Característica         |            Incidência Cumulativa            |          Taxa de Incidência          |
| :----------------------------: | :-----------------------------------------: | :----------------------------------: |
|        **Denominador**         |        População em risco no início         |        Pessoas-tempo em risco        |
|     **Tipo de população**      |               Fechada (fixa)                |               Dinâmica               |
|          **Unidade**           |            Proporção (0-1 ou %)             |      Taxa (casos/pessoa-tempo)       |
| **Considera tempo individual** |                     Não                     |                 Sim                  |
|         **Melhor uso**         | Estudos de curta duração, população estável | Estudos longos, perdas de seguimento |
|    **Perdas de seguimento**    |                Problemático                 |             Bem manejado             |

### Tipos de de prevalência
#### Prevalência pontual (point prevalence)
Mede a proporção de pessoas com a doença em um momento específico no tempo.
**Fórmula:**

$$
\text{Prevalência pontual} =
\frac{\text{Número de casos existentes em um momento}}
{\text{População total naquele momento}}
X 100
$$

**Características:**
- "Fotografia" da doença em um momento
- Útil para doenças crônicas
- Não considera duração da doença

**Exemplo:** Em 1º de janeiro de 2024, havia 200 casos de hipertensão em uma população de 5.000 pessoas. Prevalência pontual = 200/5.000 = 4%.

#### Prevalência de período (period prevalence)
Mede a proporção de pessoas que tiveram a doença durante um intervalo de tempo específico.
**Fórmula:**

$$
\text{Prevalência do período} =
\frac{\text{Casos existentes no início + casos novos durante o período}}
{\text{População em risco durante o período}}
X 100
$$

**Características:**
- Inclui casos prevalentes no início + casos incidentes
- Sempre maior que prevalência pontual
- Útil para planejamento de serviços

A prevalência de período pode ser substancialmente maior que a prevalência pontual, especialmente para doenças de longa duração (diferenças de 58,3% a 206,6% foram observadas).

| Tipo de Prevalência    | Definição                             | Quando Usar                               |
| ---------------------- | ------------------------------------- | ----------------------------------------- |
| **Pontual**            | Casos em um momento específico        | Avaliação rápida da carga de doença       |
| **Período (1 ano)**    | Casos durante um período de tempo     | Planejamento de recursos anuais           |
| **Período (lifetime)** | Casos que já tiveram a doença na vida | Estudos de saúde mental, doenças crônicas |

### Relação entre incidência e prevalência
A prevalência é influenciada tanto pela incidência quanto pela duração da doença. 

**Relação aproximada (para doenças estáveis):**

<center>Prevalência ≈ Incidência × Duração média da doença</center>

**Implicações práticas:**
- **Alta incidência + curta duração** = Baixa prevalência (exemplo: resfriado comum)
- **Baixa incidência + longa duração** = Alta prevalência (exemplo: diabetes tipo 1)
- **Alta incidência + longa duração** = Alta prevalência (exemplo: hipertensão)
- **Baixa incidência + curta duração** = Baixa prevalência (exemplo: doenças raras agudas)

### Outras medidas de frequência
#### Taxa de Mortalidade
**Taxa de Mortalidade Geral:**

$$
\text{Taxa de mortalidade} =
\frac{\text{Nº de óbitos em um período}}
{\text{População em risco}}
X 1000
$$

**Taxa de Mortalidade Específica por Causa:**

$$
\text{Taxa de Mortalidade Específica por Causa} =
\frac{\text{Óbitos por causa específica}}
{\text{População em risco}}
X 100.000
$$

#### Taxa de Letalidade
Mede a gravidade de uma doença.

$$
\text{Taxa de letalidade} =
\frac{\text{Nº de óbitos por uma doença}}
{\text{Nº de casos da doença}}
X 100
$$
**Exemplo:** Se 10 de 100 pacientes com COVID-19 grave morreram, a letalidade = 10%.

#### Taxa de ataque
Usada em surtos e epidemias.

$$
\text{Taxa de ataque} =
\frac{\text{Nº de casos durante um surto}}
{\text{População exposta}}
X 100
$$

| Medida                     | Numerador                  | Denominador                 | Interpretação               |
| -------------------------- | -------------------------- | --------------------------- | --------------------------- |
| **Incidência Cumulativa**  | Casos novos                | População em risco (início) | Risco de desenvolver doença |
| **Taxa de Incidência**     | Casos novos                | Pessoas-tempo em risco      | Velocidade de ocorrência    |
| **Prevalência Pontual**    | Casos existentes (momento) | População total (momento)   | Carga atual da doença       |
| **Prevalência de Período** | Casos existentes + novos   | População durante período   | Carga da doença no período  |
| **Taxa de Mortalidade**    | Óbitos                     | População em risco          | Risco de morte              |
| **Taxa de Letalidade**     | Óbitos por doença          | Casos da doença             | Gravidade da doença         |

### Considerações metodológicas importantes
#### Escolha do Denominador
A escolha do denominador afeta significativamente os resultados: 
- **Pessoas-ano em risco:** Exclui tempo após o evento (mais preciso)
- **Pessoas-ano total:** Inclui todo o tempo de seguimento
- **População no meio do período:** Estimativa da população média

Diferenças de -1,3% a 14,8% foram observadas dependendo do denominador utilizado.

#### População em Risco
A população em risco deve incluir apenas pessoas que podem desenvolver a doença
- Excluir pessoas que já têm a doença (para incidência)
- Excluir pessoas imunes ou não suscetíveis
- Considerar características demográficas relevantes

#### Período de Washout
Para doenças recorrentes, é necessário definir um período de washout (tempo livre de doença) para distinguir casos novos de recorrências.

### Aplicações práticas no Brasil
**Vigilância Epidemiológica**
O Ministério da Saúde utiliza medidas de frequência para:
- Monitorar tendências de doenças (incidência)
- Avaliar carga de doenças crônicas (prevalência)
- Planejar campanhas de vacinação (cobertura e incidência)
- Detectar surtos (taxa de ataque)

**Planejamento de Saúde**
- **Prevalência:** Dimensionar serviços, estimar custos, alocar recursos
- **Incidência:** Avaliar programas de prevenção, identificar grupos de risco

 **Pesquisa Etiológica**
- **Incidência:** Estudar fatores de risco e causas de doenças
- **Estudos de coorte:** Calcular risco relativo usando incidência

>[!note] Tags
> #incidência #prevalência #taxas 

