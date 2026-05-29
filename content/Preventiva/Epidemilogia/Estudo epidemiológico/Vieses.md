### Introdução
**Viés em pesquisa epidemiológica** refere-se a qualquer **desvio sistemático da verdade** que compromete a validade interna de um estudo, diferindo do conceito comum de preconceito. Todos os estudos observacionais apresentam algum grau de viés, sendo fundamental identificá-los e avaliar seu impacto nos resultados. Os vieses são tradicionalmente classificados em **três categorias principais: viés de seleção, viés de informação e confundimento**.

### Validade interna vs Externa
A validade interna significa que o estudo mediu o que se propôs a medir, enquanto a validade externa refere-se à capacidade de generalizar os achados para outros pacientes. O viés compromete principalmente a validade interna, distorcendo a comparação planejada através de algo "diferente" entre os grupos estudados.

>[!info] 2 tipos de erro sistemático
>![[Pasted image 20260526192228.png]]
>A figura acima ilustra dois tipos importantes de erro sistemático: o **viés em direção ao nulo** (quando uma associação verdadeira é subestimada) e o **viés de inversão** (quando o viés é tão substancial que inverte completamente a direção da associação, fazendo um fator protetor parecer prejudicial ou vice-versa).

### Tipos de viés
#### <u>1. Viés de Seleção</u>
**Definição:** Ocorre quando há ausência de comparabilidade entre os grupos estudados devido a diferenças nas características basais dos participantes. 

**Questões-chave para identificação:**
- Em estudos de coorte: Os participantes nos grupos expostos e não expostos são similares em todos os aspectos importantes, exceto pela exposição?
- Em estudos caso-controle: Os casos e controles são similares em todos os aspectos importantes, exceto pela doença em questão? 

**Tipos específicos:**
**Viés de usuário saudável (Healthy User Bias):** Refere-se à propensão de pacientes que recebem uma terapia preventiva também buscarem outros serviços preventivos ou adotarem outros comportamentos saudáveis. Um subtipo é o viés de aderência saudável, quando pacientes que aderem à terapia preventiva são mais propensos a engajar em outros comportamentos saudáveis. 

**Viés de usuário prevalente (Prevalent User Bias):** Distorção sistemática associada ao risco tempo-dependente que resulta na perda precoce de indivíduos mais suscetíveis ao evento e no seguimento de indivíduos de baixo risco. 

**Viés de canalização (Channeling Bias):** Ocorre quando intervenções com indicações similares são prescritas diferencialmente para grupos de pacientes com níveis variados de risco ou diferenças prognósticas.

#### <u>2. Viés de Informação</u>
**Definição:** Resulta da determinação incorreta da exposição, desfecho ou ambos. 

**Questões-chave para identificação:**
- Em estudos de coorte: A informação sobre o desfecho foi obtida da mesma forma para expostos e não expostos?
- Em estudos caso-controle: A informação sobre exposição foi coletada da mesma forma para casos e controles? 

**Características importantes:**
O efeito do viés de informação depende do seu tipo. Se a informação é coletada de forma diferente para um grupo em comparação a outro, ocorre viés. Por outro lado, a **classificação incorreta não diferencial** tende a obscurecer diferenças reais. 

**Viés de classificação incorreta:** Pode ocorrer na exposição (classificar sujeitos como expostos quando não são, ou vice-versa), no desfecho (classificar sujeitos como tendo o desfecho quando não têm) ou em confundidores. 

**Viés protopatológico (Protopathic Bias):** Ocorre quando um sinal precoce da doença em estudo levou à prescrição do medicamento em estudo, interpretando-se erroneamente um fator como resultado da exposição quando na verdade é um determinante da exposição.

#### <u>3. Confundimento</u>
**Definição:** É uma mistura ou confusão de efeitos - o pesquisador tenta relacionar uma exposição a um desfecho, mas na verdade mede o efeito de um terceiro fator (a variável de confusão). 

**Características da variável de confusão:**
- Está associada tanto à exposição quanto ao desfecho
- Não está diretamente envolvida na via causal entre exposição e desfecho 

**Questão-chave:** Os resultados poderiam ser explicados pela presença de um fator (idade, tabagismo, comportamento sexual, dieta) associado tanto à exposição quanto ao desfecho, mas não diretamente envolvido na via causal? 

**Viés de confundimento por indicação:** Ocorre quando o diagnóstico subjacente ou outras características clínicas que afetam o uso de determinado medicamento também estão relacionadas ao desfecho em estudo.

#### 4. Vieses Relacionados ao Desenho do Estudo
**Viés de tempo imortal (Immortal Time Bias):** Distorção sistemática resultante da classificação incorreta ou exclusão do tempo imortal - um período de seguimento durante o qual, por definição, a morte ou o desfecho do estudo não pode ocorrer. 

**Viés de atrito:** Afeta a representatividade dos participantes e as estimativas de efeito do tratamento devido a perdas de seguimento diferenciais entre grupos.

### Estratégias de controle e prevenção de vieses

>[!info]
>![[Pasted image 20260526192546.png]]
>A figura acima demonstra o processo sistemático de abordagem do viés em pesquisa farmacoepidemológica, desde o planejamento inicial até o relato final, enfatizando que a mitigação do viés começa na fase de planejamento do estudo.

| Tipo de Viés                            | Métodos de Mitigação                                                                                                                                                                                                      |
| --------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Confundimento por indicação**         | Seleção de desenho alternativo, G-estimation, variáveis instrumentais, modelos estruturais marginais, pareamento, regressão multivariada, escores de propensão, métodos de restrição, padronização, estratificação        |
| **Viés de canalização**                 | Seleção de desenho alternativo, pareamento, escores de propensão, regressão multivariada                                                                                                                                  |
| **Viés de usuário saudável**            | Comparador ativo, restrição, ajuste multivariado, escores de propensão                                                                                                                                                    |
| **Viés protopatológico**                | Abordagem de tempo de latência (lag-time), restrição de análises (incluindo apenas populações com baixo risco de viés protopatológico)                                                                                    |
| **Viés de usuário prevalente**          | Desenho de novo usuário, desenho de novo usuário prevalente                                                                                                                                                               |
| **Viés de tempo imortal**               | Abordagem analítica alternativa (método Mantel-Byar/exposição variável no tempo, método landmark), seleção de desenho alternativo (desenho de novo usuário com comparador ativo)                                          |
| **Viés de classificação incorreta**     | Análise de viés bayesiana, máxima verossimilhança modificada, imputação múltipla para erro de medida, análise de viés probabilística, calibração de escore de propensão, calibração de regressão, análise de viés simples |
| **Dados faltantes/perda de seguimento** | Análise de casos completos, ponderação por probabilidade inversa, método de indicador faltante, imputação múltipla, análises de sensibilidade incorporando cenários de pior e melhor caso, imputação de valor único       |

### Métodos gerais de controle de confundimento
O confundimento pode ser controlado de várias formas: 
1. **Restrição:** Limitar a inclusão de participantes a categorias específicas da variável de confusão
2. **Pareamento:** Selecionar controles que sejam similares aos casos em relação às variáveis de confusão
3. **Estratificação:** Analisar os dados separadamente dentro de estratos da variável de confusão
4. **Técnicas multivariadas sofisticadas:** Regressão logística, modelos de Cox, entre outros

### Avaliação de viés em ensaios clínicos randomizados
Mesmo ensaios clínicos randomizados bem conduzidos podem apresentar vieses. A ferramenta Cochrane revisada para avaliação de risco de viés (RoB 2) distingue cinco domínios de viés: 
1. **Processo de randomização**
2. **Desvios das intervenções pretendidas**
3. **Dados de desfecho faltantes**
4. **Medição do desfecho**
5. **Relato seletivo dos achados**

### Checklist para avaliação de estudos observacionais
Ao avaliar estudos observacionais, deve-se seguir esta sequência: 
1. **Viés de seleção está presente?**
2. **Viés de informação está presente?**
3. **Confundimento está presente?**
4. **Se os resultados não podem ser explicados por esses três vieses, poderiam ser resultado do acaso?**
    - Qual é o risco relativo ou odds ratio e o IC 95%?
    - A diferença é estatisticamente significativa?
    - O estudo teve poder adequado?
5. **Somente se os resultados ainda não puderem ser explicados, então (e somente então) os achados podem ser reais e dignos de nota**

### Critérios para associação causal
Diferenciar entre associações espúrias, indiretas e causais pode ser difícil. Critérios que apoiam uma relação causal incluem: 
- **Sequência temporal:** A exposição precede o desfecho
- **Força da associação:** Magnitude do efeito
- **Consistência:** Reprodutibilidade em diferentes estudos e populações
- **Evidência de efeito dose-resposta:** Maior exposição leva a maior efeito
- **Plausibilidade biológica:** Mecanismo biológico plausível

>[!note] Tags
> #viés #vieses 