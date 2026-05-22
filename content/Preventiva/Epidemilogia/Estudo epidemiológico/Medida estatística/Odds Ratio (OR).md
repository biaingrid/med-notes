### Definição
O **Odds ==Ratio== (OR)** ou **Razão de Chances** é uma <mark style="background:#fff88f">medida estatística que quantifica a força de associação entre uma exposição e um desfecho em estudos epidemiológicos e clínicos</mark>. É especialmente utilizada em estudos caso-controle, regressão logística e meta-análises.

### O que é Odds (chance)?
Antes de entender o Odds Ratio, é fundamental compreender o conceito de "odds" (chance). **Odds é a probabilidade de um evento ocorrer dividida pela probabilidade do evento não ocorrer**.
$$
\text{Odds} =
\frac{\text{Probabilidade do evento}}
{\text{Probabilidade de não ocorrer}}
=
\frac{p}{1-p}
$$

**Exemplo prático:** Se 20 de 100 pacientes desenvolvem uma doença, a probabilidade é 20/100 = 0,20 (20%). O odds seria:
$$
\text{Odds} =
\frac{\text{20}}
{\text{80}}
=
0,25
$$
### Diferença entre Risco e Odds
|         Conceito          |                       Definição                       | Fórmula | Exemplo (20 casos em 100 pessoas) |
| :-----------------------: | :---------------------------------------------------: | :-----: | :-------------------------------: |
| **Risco (Probabilidade)** |   Número de eventos dividido pelo total de pessoas    | a/(a+b) |       20/100 = 0,20 ou 20%        |
|     **Odds (Chance)**     | Número de eventos dividido pelo número de não-eventos |   a/b   |           20/80 = 0,25            |
Quando o evento é **raro (< 10%)**, o odds aproxima-se do risco. Quando o evento é **comum (> 10%)**, odds e risco divergem significativamente.

### O que é Odds Ratio?
O **Odds Ratio é a razão entre os odds de dois grupos diferentes** - tipicamente um grupo exposto versus um grupo não exposto, ou casos versus controles.

**Fórmula geral:**
$$
\text{OR} =
\frac{\text{Odds no grupo exposto}}
{\text{Odds no grupo não exposto}}
$$
Em uma tabela 2x2:

| Doença Presente | Doença Ausente | Total |
| :-------------: | :------------: | :---: |
|        a        |       b        |  a+b  |
|        c        |       d        |  c+d  |
|       a+c       |      b+d       |   N   |
$$
\text{OR} =
\frac{\text{a/b}}
{\text{c/d}}
=
\frac{\text{a*d}}
{\text{b*c}}
$$
### Interpretação do OR
| Valor do OR  |         Interpretação          |                   Significado Clínico                    |
| :----------: | :----------------------------: | :------------------------------------------------------: |
| **OR = 1,0** |         Sem associação         |             A exposição não afeta o desfecho             |
| **OR > 1,0** |      Associação positiva       |          A exposição aumenta o odds do desfecho          |
|  **OR 1,0**  | Associação negativa (proteção) | A exposição diminui o odds do desfecho (efeito protetor) |
| **OR = 2,0** |         Dobro do odds          |   O odds do desfecho é 2 vezes maior no grupo exposto    |
| **OR = 0,5** |         Metade do odds         |     O odds do desfecho é 50% menor no grupo exposto      |

### Exemplo prático de cálculo
**Estudo caso-controle:** Investigação da associação entre tabagismo e câncer de pulmão.

| Câncer de Pulmão (Casos) | Sem Câncer (Controles) | Total |
| :----------------------: | :--------------------: | :---: |
|           105            |           95           |  200  |
|           180            |          240           |  420  |
|         **285**          |        **335**         |  620  |
**Cálculo:**
- Odds de exposição nos casos = 105/95 = 1,105
- Odds de exposição nos controles = 180/240 = 0,75
- **OR = 1,105 / 0,75 = 1,47**

**Interpretação:** Os pacientes com câncer de pulmão têm 1,47 vezes o odds de serem fumantes comparados aos controles sem câncer.

### Quando usar OR?
| Tipo de Estudo                    | Uso do OR               | Justificativa                                                                  |
| --------------------------------- | ----------------------- | ------------------------------------------------------------------------------ |
| **Estudos caso-controle**         | Recomendado             | É a medida apropriada de associação; não é possível calcular risco diretamente |
| **Regressão logística**           | Recomendado             | É o resultado natural deste método estatístico                                 |
| **Estudos transversais**          | Aceitável               | Pode ser usado quando não há avaliação de incidência                           |
| **Ensaios clínicos randomizados** | Usar com cautela        | Pode superestimar o efeito quando o desfecho é comum (>10%)                    |
| **Estudos de coorte**             | Preferir Risco Relativo | OR pode exagerar a magnitude do efeito                                         |
| **Meta-análises**                 | Muito usado             | Tem propriedades estatísticas favoráveis para agregação de estudos             |
>[!warning] Estudos que utilizam OR
>- Caso-controle
>- Regressão logística
>- Meta-análises

### Limitações
#### 1. Exagero do Risco Relativo
O OR sempre exagera o risco relativo verdadeiro em algum grau. Quando a doença é **rara (< 10%),** o OR aproxima-se do risco relativo. Quando o evento é **comum**, o exagero aumenta e o OR não é mais um bom substituto para o risco relativo.

**Exemplo comparativo (desfecho comum - 54%):**

| Medida                  | Valor | Interpretação                |
| ----------------------- | ----- | ---------------------------- |
| **Risco Relativo (RR)** | 0,50  | Redução de 50% no risco      |
| **Odds Ratio (OR)**     | 0,23  | Aparenta redução muito maior |
A diferença é substancial porque a incidência do desfecho era alta (54%). Se o OR for incorretamente interpretado como RR, pode levar a uma superestimação do risco.
#### 2. Dificuldade de Interpretação
Odds e odds ratios são difíceis para muitos clínicos compreenderem. A interpretação não é tão intuitiva quanto o risco relativo. Por isso, seu uso deve ser limitado a situações onde é a medida apropriada (estudos caso-controle e regressão logística).
#### 3. Impossibilidade de Cálculo em Certas Situações
- Quando não há eventos no grupo controle, nem OR nem RR podem ser calculados
- Quando todos os participantes do grupo intervenção apresentam o desfecho, o OR não pode ser calculado

>[!warning] Impossibilidade
>É **obrigatório** haver um grupo base, sem o desfecho

### Intervalo de confiança
O **intervalo de confiança (IC)** reflete a precisão dos resultados do estudo. O IC 95% é o mais comumente usado e fornece um intervalo de valores que tem 95% de probabilidade de conter o valor verdadeiro para toda a população.

**Interpretação:**
- Se o IC 95% do OR **não inclui 1,0**: a associação é estatisticamente significativa
- Se o IC 95% do OR **inclui 1,0**: a associação não é estatisticamente significativa

**Exemplo:**
- OR = 2,5 (IC 95%: 1,8 - 3,5) → Associação significativa
- OR = 1,3 (IC 95%: 0,8 - 2,1) → Associação não significativa

### OR vs RR: resumo
|         Característica          |                 Odds Ratio (OR)                 |     Risco Relativo (RR)      |
| :-----------------------------: | :---------------------------------------------: | :--------------------------: |
|          **Definição**          |           Razão de odds entre grupos            | Razão de riscos entre grupos |
|     **Estudos apropriados**     | Caso-controle, transversal, regressão logística |   Coorte, ensaios clínicos   |
|  **Quando evento raro (10%)**   |                Aproxima-se do RR                |        Medida direta         |
| **Quando evento comum (>10%)**  |                  Exagera o RR                   |     Medida mais precisa      |
| **Facilidade de interpretação** |                     Difícil                     |        Mais intuitiva        |
|     **Uso em meta-análise**     |                   Muito usado                   |         Menos usado          |



>[!note] Tags
> #OR #IC #VP #odds #ratio 







