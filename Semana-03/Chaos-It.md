# O Labirinto de Boehm

O Modelo Espiral de Boehm se diferencia de modelos como Cascata por colocar a análise de riscos como atividade central de cada ciclo, não como uma checagem pontual no início do projeto. Neste caso, o colapso foi causado por riscos técnicos ignorados (cenário que o modelo espiral evita).

## Por que a Análise de Riscos em cada volta da espiral teria evitado a queda dos drones?

Em cada volta da espiral, antes de qualquer compromisso de desenvolvimento, a equipe seria obrigada a responder: "Quais são os maiores riscos desta iteração?" Para um sistema de controle de drones, riscos como falha de comunicação, latência de resposta, comportamento em condições adversas de vento e redundância de sensores seriam identificados e mitigados antes de seguir em frente. O modelo força prototipagem e validação técnica precoce - um protótipo de voo controlado seria testado na 1ª ou 2ª volta, e só após aprovação os recursos seriam comprometidos com o desenvolvimento completo. Sem isso, a equipe só descobriu os riscos quando os drones já estavam no ar.

---

### Ciclo da Espiral (Projeto de IA Subaquática)

```mermaid
flowchart TD
    A[Planejamento - Definição de objetivos da iteração (ex: navegação subaquática)]
    B[Análise de Riscos - falha de comunicação, latência, sensores]
    C[Engenharia - desenvolvimento e testes (IA, sensores, protótipo)]
    D[Avaliação - feedback dos stakeholders e validação]

    A --> B
    B --> C
    C --> D
    D --> A
```

---

## O diagnóstico CMMI

Nível 1 - Inicial.  
Evidências presentes na descrição: cada dev trabalha do seu jeito, prazos são "chutados" (sem planejamento baseado em dados históricos) e o sucesso depende de esforço individual.

## O que falta para chegar ao Nível 2 - Gerenciado?

Para subir ao Nível 2, a Chaos-IT precisa instituir as Áreas de Processo exigidas, que incluem: gerenciamento de requisitos, planejamento de projetos, monitoramento e controle de projetos, gestão de configuração e garantia de qualidade de processo e produto. Ou seja, exige que os mesmos processos básicos sejam repetidos de projeto em projeto, com registro.
