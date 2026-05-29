### Introdução
O **risco relativo (RR)**, também chamado de **razão de risco**, é uma medida estatística fundamental que <mark style="background:#fff88f">compara a probabilidade de um desfecho ocorrer em um grupo exposto versus um grupo não exposto</mark>. É calculado dividindo-se o risco (ou incidência) do desfecho no grupo exposto pelo risco no grupo não exposto.

### Conceito e definição
O risco relativo expressa quantas vezes o risco de um evento é maior (ou menor) em um grupo comparado a outro. É uma medida **relativa** de associação, amplamente utilizada em ensaios clínicos randomizados e estudos de coorte.

**Fórmula básica:**
$$
RR =
\frac{\text{Risco no grupo exposto}}
{\text{Risco no grupo não exposto}}
=
\frac{a/(a+b)}
{c/(c+d)}
$$
Onde:
- a = número de eventos no grupo exposto
- b = número de não-eventos no grupo exposto
- c = número de eventos no grupo não exposto
- d = número de não-eventos no grupo não exposto

### Interpretação do Risco Relativo
| Valor do RR | Interpretação              | Significado Clínico                                                       |
| ----------- | -------------------------- | ------------------------------------------------------------------------- |
| RR = 1,0    | Sem associação             | O risco é igual nos dois grupos; a exposição não afeta o desfecho         |
| RR > 1,0    | Risco aumentado            | A exposição aumenta o risco do desfecho; quanto maior o RR, maior o risco |
| RR 1,0      | Efeito protetor            | A exposição reduz o risco do desfecho; indica proteção                    |
| RR = 2,0    | Risco dobrado              | O risco no grupo exposto é duas vezes maior que no grupo não exposto      |
| RR = 0,5    | Risco reduzido pela metade | O risco no grupo exposto é metade do risco no grupo não exposto           |
#### Exemplo Prático Ilustrativo
Considere um ensaio clínico randomizado avaliando um programa de suporte psicológico para enfermeiros:
- **Grupo Controle (sem suporte):** 70 de 100 enfermeiros desenvolveram depressão = risco de 0,70 (70%)

- **Grupo Intervenção (com suporte):** 35 de 100 enfermeiros desenvolveram depressão = risco de 0,35 (35%)

$$
RR =
\frac{\text{0,35}}
{\text{0,7}}
=
0,5
$$
**Interpretação:** O risco de depressão no grupo que recebeu suporte psicológico é metade do risco no grupo que não recebeu, indicando um efeito protetor do programa.

### Risco Relativo vs. Risco Absoluto
É fundamental distinguir entre medidas relativas e absolutas:
- **Risco Relativo (medida relativa):** Compara proporcionalmente os riscos entre grupos, mas não informa a magnitude absoluta do efeito.
- **Redução Absoluta de Risco (medida absoluta):** Calculada pela diferença entre os riscos dos dois grupos. No exemplo acima: 70% - 35% = 35% de redução absoluta.

>[!info] Relação entre risco relativo e risco absoluto em estudos de saúde cardiovascular, demonstrando que riscos relativos elevados podem corresponder a diferenças absolutas modestas:
>![[Pasted image 20260520203558.png]]
>Esta visualização mostra que em mais de um terço dos estudos, a diferença absoluta de risco foi inferior a 1 ponto percentual, apesar de riscos relativos que podem parecer substanciais. Isso ressalta a importância de sempre considerar tanto medidas relativas quanto absolutas ao interpretar resultados clínicos.

### Intervalo de Confiança e Significância Estatística
O intervalo de confiança (IC) de 95% reflete a precisão dos resultados do estudo e indica a faixa de valores que provavelmente contém o verdadeiro valor populacional.

**Interpretação do IC 95%:**
- Se o IC **não inclui 1,0**: o resultado é estatisticamente significativo
- Se o IC **inclui 1,0**: o resultado não é estatisticamente significativo
- IC estreito: maior precisão
- IC amplo: menor precisão

**Exemplos:**
- RR = 20,0 (IC 95%: 0,10-100): **Não significativo** - apesar do RR alto, o IC inclui 1,0 
- RR = 1,1 (IC 95%: 1,05-1,15): **Significativo** - o IC não inclui 1,0

### Quando Utilizar o Risco Relativo
O risco relativo pode ser calculado apenas em estudos que acompanham grupos ao longo do tempo:
**Estudos apropriados:**
- Ensaios clínicos randomizados (prospectivos)
- Estudos de coorte (prospectivos ou retrospectivos)
- Análises de bancos de dados longitudinais

**Estudos inadequados:**
- Estudos caso-controle (utiliza-se odds ratio)
- Estudos transversais (preferível usar prevalence ratio)

### Limitações e Controvérsias
Pesquisas recentes demonstram limitações importantes do risco relativo:
**Dependência da prevalência basal:** O RR varia não apenas pela magnitude do efeito, mas também pela prevalência basal do desfecho. À medida que a prevalência aumenta, o RR tende ao valor nulo (1,0), independentemente da força da associação. 

**Interpretação em estudos observacionais:** Em estudos epidemiológicos observacionais, muitos epidemiologistas são cautelosos ao aceitar RR < 3,0, e quase nunca RR < 2,0, devido à possibilidade de fatores de confusão não controlados. Aumentos de risco menores que 100% (RR < 2,0) são difíceis de interpretar. 

**Diferença entre RR e Hazard Ratio (HR):** O RR compara riscos cumulativos em um período fixo, enquanto o HR compara taxas instantâneas ao longo do tempo. Frequentemente, HRs são erroneamente interpretados como RRs.

### Aplicação Clínica e Tomada de Decisão
Para decisões clínicas informadas, é essencial:
1. **Avaliar significância estatística E relevância clínica:** Um resultado pode ser estatisticamente significativo, mas clinicamente irrelevante. 
2. **Considerar medidas absolutas:** Calcular o Número Necessário para Tratar (NNT) ou Número Necessário para Causar Dano (NNH) para contextualizar o impacto real da intervenção.
3. **Balancear benefícios e riscos:** Avaliar tanto os benefícios quanto os efeitos adversos em pacientes individuais. 
4. **Contextualizar com risco basal:** O mesmo RR tem implicações clínicas diferentes dependendo do risco basal da população.

### Risco Relativo vs. Odds Ratio
|         Característica         |         Risco Relativo (RR)          |             Odds Ratio (OR)             |
| :----------------------------: | :----------------------------------: | :-------------------------------------: |
|         **Definição**          |       Razão de probabilidades        |            Razão de chances             |
|    **Estudos apropriados**     |       Coorte, ensaios clínicos       | Caso-controle, coorte, ensaios clínicos |
|       **Interpretação**        |            Mais intuitiva            |             Menos intuitiva             |
|        **Aproximação**         | OR ≈ RR quando desfecho é raro (10%) |            OR sempre válido             |
| **Dependência da prevalência** |     Varia com prevalência basal      |       Independente da prevalência       |
|       **Meta-análises**        |            Menos estável             |  Propriedades estatísticas superiores   |

>[!note] Tags
> #RR #risco #OR #IC 

