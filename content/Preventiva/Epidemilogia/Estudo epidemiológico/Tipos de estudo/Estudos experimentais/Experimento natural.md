### Definição
Combina características de estudos experimentais e observacionais. <mark style="background:#fff88f">A exposição não é controlada pelo pesquisador</mark>, mas ocorre por processos naturais, sociais, políticos ou administrativos que criam condições semelhantes a uma randomização - o conceito de "como se fosse randomizado".

>[!warning] Característica
>A **exposição não é controlada pelo pesquisador.** 
>Como se fosse randomizado.

#### Comparativo com os outros estudos

|          Característica          |         Ensaio Clínico Randomizado (ECR)          |                            Experimento Natural                            |       Estudo Observacional Tradicional       |
| :------------------------------: | :-----------------------------------------------: | :-----------------------------------------------------------------------: | :------------------------------------------: |
|    **Alocação da exposição**     |            Controlada pelo pesquisador            | Determinada por processos externos (naturais, políticos, administrativos) |   Auto-seleção ou fatores não controlados    |
|         **Randomização**         |                Randomização formal                |           "Como se fosse randomizado" <br>(as-if randomization)           |               Sem randomização               |
|      **Controle de vieses**      | Alto controle (randomização quebra confundimento) |   Controle moderado (depende da plausibilidade da as-if randomization)    | Baixo controle (alto risco de confundimento) |
|      **Viabilidade ética**       |         Limitada para certas intervenções         |         Permite avaliar intervenções não manipuláveis eticamente          |                    Ampla                     |
| **Aplicabilidade ao mundo real** |           Condições ideais/controladas            |                          Condições do mundo real                          |           Condições do mundo real            |
|            **Custo**             |                       Alto                        |                Moderado a baixo <br>(usa dados existentes)                |                   Variável                   |

### Conceito chave: Como se fosse randomizado
A força da inferência causal em experimentos naturais depende da **plausibilidade da as-if randomization** - ou seja, o quanto a alocação da exposição pode ser considerada aleatória em relação aos fatores prognósticos.

**Critérios para avaliar a plausibilidade:**
- Os participantes tinham **informação** suficiente para controlar sua própria alocação?
- Tinham **incentivos** para escolher um grupo específico?
- Tinham **capacidade** de controlar sua alocação?

Quanto menos informação, incentivos e capacidade os indivíduos tiverem para auto-selecionar sua exposição, mais plausível é a as-if randomization.

### Exemplos
#### 1. John Snow e a Epidemia de Cólera em Londres (1854)
**Contexto:** Duas companhias de água abasteciam Londres. Uma mudou sua captação para montante do esgoto; a outra manteve a captação a jusante (água contaminada). 

**Por que é um experimento natural?**
- A distribuição das companhias pelas casas foi feita por proprietários anos antes da epidemia
- Moradores não escolheram nem sabiam qual companhia os abastecia
- Ambas as companhias serviam casas ricas e pobres, grandes e pequenas, na mesma rua
- Resultado: Taxa de mortalidade por cólera 8,5 vezes maior nas casas com água contaminada

#### 2. Loteria e Saúde Mental
Estudo usando dados do British Household Panel Survey mostrou melhorias na saúde mental após ganhar prêmios de loteria - a randomização foi feita pelo próprio sorteio da loteria.

### Vantagens
| Vantagem                                               | Descrição                                                                                                                                     |
| ------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------------------------------- |
| **Avaliação de intervenções não manipuláveis**         | Permite estudar políticas públicas, reformas de sistemas de saúde, eventos naturais que não podem ser randomizados eticamente ou praticamente |
| **Validade externa (mundo real)**                      | Resultados refletem condições reais de implementação, não ambientes controlados artificialmente                                               |
| **Custo-efetividade**                                  | Frequentemente utilizam dados rotineiramente coletados (registros de saúde, censos), reduzindo custos                                         |
| **Menor viés que estudos observacionais tradicionais** | A as-if randomization reduz confundimento e viés de seleção comparado a estudos observacionais sem essa característica                        |
| **Avaliação de efeitos de longo prazo**                | Podem capturar efeitos que levam tempo para aparecer, usando dados longitudinais existentes                                                   |

### Limitações e desafios
| Limitação                           | Descrição                                                                                 | Estratégias de Mitigação                                                                      |
| ----------------------------------- | ----------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- |
| **Viés de seleção**                 | Exposição pode não ser verdadeiramente aleatória; auto-seleção pode ocorrer               | Avaliar rigorosamente a plausibilidade da as-if randomization; usar análises de sensibilidade |
| **Confundimento residual**          | Fatores não medidos podem influenciar tanto exposição quanto desfecho                     | Incluir múltiplos métodos de análise; testes de falsificação                                  |
| **Falta de controle sobre timing**  | Pesquisador não controla quando a "intervenção" ocorre, podendo perder dados basais       | Usar dados retrospectivos quando disponíveis; desenhos antes-depois                           |
| **Definição de exposição complexa** | Difícil definir quem foi realmente "exposto" em intervenções populacionais amplas         | Medir níveis graduados de exposição ao invés de binário exposto/não-exposto                   |
| **Suposições não verificáveis**     | Muitas suposições necessárias para inferência causal não podem ser testadas empiricamente | Transparência na descrição de suposições; análises de sensibilidade robustas                  |
| **Dados disponíveis limitados**     | Dependência de dados existentes que podem não incluir todas as variáveis relevantes       | Investimento em infraestrutura de dados e linkage de bases de dados                           |

### Desenhos metodológicos comuns em experimentos naturais
#### 1. Diferenças-em-Diferenças (Difference-in-Differences)
Compara mudanças ao longo do tempo entre grupo exposto e não-exposto. É o desenho mais comum (25% dos estudos). 

**Fórmula:**
$$\text{Efeito} = (\text{Pós}_{\text{exposto}} - \text{Pré}_{\text{exposto}}) - (\text{Pós}_{\text{controle}} - \text{Pré}_{\text{controle}})$$

#### 2. Antes-Depois (Before-After)
Compara desfechos no mesmo grupo antes e depois da intervenção (23% dos estudos). 
#### 3. Variáveis Instrumentais
Usa uma variável (instrumento) que afeta o desfecho apenas através da exposição. 
#### 4. Regressão com Descontinuidade
Explora limiares arbitrários que determinam exposição (ex: idade para elegibilidade a programa).

### Quando usar Experimento Natural vs ECR?

| <u>Prefira Experimento Natural quando:</u> <br>- Randomização é eticamente impossível <br>(ex: avaliar efeito de poluição do ar)<br><br>- Randomização é **praticamente inviável** <br>(ex: políticas nacionais já implementadas)<br>    <br>- Intervenção já é **padrão de cuidado** e não pode ser negada ao grupo controle<br>    <br>- Interesse em **efeitos no mundo real** sob condições naturais de implementação<br>    <br>- **Recursos limitados** e dados rotineiros estão disponíveis<br>    <br><br> | <u>**Prefira ECR quando:** </u><br><br>- Objetivo é avaliar **eficácia** sob condições ideais<br>    <br>- Randomização é **ética e viável**<br>    <br>- Necessário **controle rigoroso** de confundimento<br>    <br>- Avaliação de **novos tratamentos** antes da aprovação regulatória |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |


>[!note] Tags
> #estudo #experimento #ramdomizado 
