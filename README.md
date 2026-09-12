# 🚀 Miniguia de Estudos: Otimização de Salto Vertical com NotebookLM

Repositório criado para documentar o processo de aprendizado, curadoria e extração de conhecimento utilizando o **Google NotebookLM**, desenvolvido como projeto prático para a plataforma **DIO**.

---

## 🎯 Contexto e Objetivos

* **Tema de Estudo:** Biomecânica, periodização de treino e otimização do salto vertical.
* **Meta Pessoal:** Desenvolver a capacidade de realizar uma enterrada em aro regulamentar (3,05 m) com 1,80 m de altura corporal.
* **Objetivos com o NotebookLM:**
  1. Centralizar e sintetizar o conhecimento prático de treinadores e atletas de elite com a literatura científica esportiva.
  2. Estruturar um protocolo seguro de reintrodução a treinos de pliometria e força máxima.
  3. Diagnosticar desequilíbrios neuromusculares via Perfil Força-Velocidade ($F-V$) e entender a influência mecânica dos membros superiores no salto.

---

## 📚 Curadoria de Fontes

Para garantir rigor técnico aliado à aplicabilidade prática, a base de fontes combinou análises práticas do YouTube com artigos científicos complementados pelo *Deep Research* do próprio NotebookLM:

1. **[Isaiah Rivera - How to 2 Foot Jump](https://www.youtube.com/watch?v=sPelD0VEphs)**: Foco em mecânica de aproximação, penúltimo passo (*penultimate step*) e bloqueio de frenagem para conversão horizontal-vertical.
2. **[Riq B - How to Jump Higher](https://www.youtube.com/watch?v=KA4eeJJiiRA)**: Exercícios de pliometria reativa, rigidez de tornozelo (*ankle stiffness*) e transferência de força.
3. **[Riq B - How to Jump Higher (Deep Dive)](https://www.youtube.com/watch?v=RUdn3W9zzPg)**: Periodização de saltos, progressões de carga e prevenção de sobrecarga articular.
4. **Deep Research (NotebookLM)**: Artigos científicos e modelos biomecânicos de Pierre Samozino e Jean-Benoît Morin sobre o Perfil Força-Velocidade e artigos sobre a contribuição biomecânica do balanço dos braços no salto com contramovimento (CMJ).

---

## 🧠 Engenharia de Prompts e "Cicatrizes" (Troubleshooting)

A exploração do caderno exigiu refinamentos sucessivos para evitar generalismos fitness e focar em dados biomecânicos precisos:

### Ciclo de Testes e Ajustes

| Pergunta / Intenção | Desafio Encontrado (Cicatriz) | Ajuste de Prompt (Solução) |
| :--- | :--- | :--- |
| **Retorno aos treinos** | A resposta inicial sugeria listas de exercícios genéricos (ex: "faça agachamento 3x10"). | Contextualizei o histórico pregresso com força/pliometria e solicitei um roteiro focado em adaptação tendínea e controle de dor (regra 24–48h). |
| **Déficit Força-Velocidade** | A ferramenta explicava apenas o conceito teórico sem os inputs/outputs necessários para cálculo. | Solicitei a metodologia exata de Samozino e Morin com dados de entrada ($h_{PO}$, massa, cargas) e interpretação do $FV_{imb}$. |
| **Balanço dos braços** | As respostas focavam em dicas superficiais de postura. | Direcionei o prompt para o mecanismo biomecânico (elevação de centro de massa, transferência de energia cinética e sincronização temporal). |

---

## 📖 Miniguia de Estudo (Entrega Final)

### 1. Resumo Estruturado

* **Fase de Retorno (Reaclimatização):** Priorizar a saúde do tendão patelar com isometrias (como *Spanish Squats*) e *Heavy Slow Resistance* (HSR). O tendão responde tardiamente à carga; monitorar o desconforto na janela de 24 a 48 horas (limite ≤ 3/10).
* **Diagnóstico de Força-Velocidade ($F-V$):** Atletas com mesma impulsão podem necessitar de estímulos opostos. Se o teste ($FV_{imb}$) indicar déficit de força ($F_0$), a prioridade é agachamento pesado (>80% 1RM); se indicar déficit de velocidade ($V_0$), priorizam-se treinos balísticos e saltos assistidos.
* **Mecânica dos Braços:** O balanço correto dos braços pode agregar de 9% a 38% na altura final do salto, sendo 28% atribuídos à elevação prévia do centro de massa e 72% ao aumento da velocidade vertical de decolagem via transferência de energia cinética. O início ideal da subida dos braços dá-se em ~76% da duração do salto.

---

### 2. Glossário de Conceitos-Chave

* **Stiffness (Rigidez Musculotendínea):** Propriedade da unidade músculo-tendão de resistir à deformação sob carga rápida, essencial para o tornozelo devolver energia elástica sem tempo de contato excessivo com o solo.
* **Ciclo de Alongamento-Encurtamento (CAE):** Mecanismo no qual uma contração excêntrica rápida é seguida imediatamente por uma contração concêntrica, maximizando a produção de potência.
* **Taxa de Desenvolvimento de Força (TDF / RFD):** A velocidade com que a força muscular é gerada nos primeiros milissegundos do movimento.
* **$FV_{imb}$ (Desequilíbrio Força-Velocidade):** Desvio percentual entre a relação real de força/velocidade de um atleta e o seu perfil ótimo teórico.
* **PAPE (Potenciação do Desempenho Pós-Ativação):** Fenômeno neuromuscular em que a força ou potência é temporariamente aumentada após uma contração muscular prévia intensa.

---

### 3. Prompts Reutilizáveis para Revisão Contínua

Copie e cole no NotebookLM para aprofundar seus estudos futuros:

```text
1. Diagnóstico e Treino:
"Com base nas fontes, elabore um microciclo semanal de treino para um atleta com Déficit de [Força/Velocidade], integrando exercícios isométricos para tendão patelar e sprints curtos."

2. Correção de Mecânica:
"Explique o passo a passo técnico do penúltimo passo (penultimate step) para um salto com dois pés, detalhando os erros mais comuns que causam perda de velocidade horizontal."

3. Planejamento de Carga:
"Como estruturar uma sessão utilizando o Método de Contraste Francês (FCM) para salto vertical sem sobrecarregar a articulação do joelho?"
