# O Labirinto de Boehm

O Modelo Espiral de Boehm se diferencia de modelos como Cascata por colocar a análise de riscos como atividade central de cada ciclo, não como uma checagem pontual no início do projeto. Neste caso, o colapso foi causado por riscos técnicos ignorados (cenário que o modelo espiral evita).

## Por que a Análise de Riscos em cada volta da espiral teria evitado a queda dos drones?

Em cada volta da espiral, antes de qualquer compromisso de desenvolvimento, a equipe seria obrigada a responder: "Quais são os maiores riscos desta iteração?" Para um sistema de controle de drones, riscos como falha de comunicação, latência de resposta, comportamento em condições adversas de vento e redundância de sensores seriam identificados e mitigados antes de seguir em frente. O modelo força prototipagem e validação técnica precoce - um protótipo de voo controlado seria testado na 1ª ou 2ª volta, e só após aprovação os recursos seriam comprometidos com o desenvolvimento completo. Sem isso, a equipe só descobriu os riscos quando os drones já estavam no ar.

---

### Ciclo da Espiral (Projeto de IA Subaquática)

![espiral_boehm](https://github.com/user-attachments/assets/4888ddbd-dc37-434c-b66f-71ac69ac245d)

![Uploading espiral_bo<svg width="800" height="800" viewBox="0 0 800 800" xmlns="http://www.w3.org/2000/svg" style="background:#ffffff;font-family:Arial,Helvetica,sans-serif">

  <!-- Quadrant backgrounds -->
  <rect x="0"   y="0"   width="400" height="400" fill="#EEEDFE"/>
  <rect x="400" y="0"   width="400" height="400" fill="#FAECE7"/>
  <rect x="400" y="400" width="400" height="400" fill="#E1F5EE"/>
  <rect x="0"   y="400" width="400" height="400" fill="#FAEEDA"/>

  <!-- Quadrant dividers -->
  <line x1="0" y1="400" x2="800" y2="400" stroke="#b0aec8" stroke-width="1"/>
  <line x1="400" y1="0" x2="400" y2="800" stroke="#b0aec8" stroke-width="1"/>

  <!-- Quadrant labels -->
  <text x="200" y="46" text-anchor="middle" font-size="15" font-weight="700" fill="#3C3489">Q1 · Planejamento</text>
  <text x="600" y="46" text-anchor="middle" font-size="15" font-weight="700" fill="#993C1D">Q2 · Análise de Riscos</text>
  <text x="600" y="780" text-anchor="middle" font-size="15" font-weight="700" fill="#0F6E56">Q3 · Desenvolvimento</text>
  <text x="200" y="780" text-anchor="middle" font-size="15" font-weight="700" fill="#854F0B">Q4 · Avaliação</text>

  <!-- ========== SPIRAL ARCS ========== -->
  <!-- Each arc is a quarter-circle, alternating quadrant colors, growing outward -->

  <!-- Volta 1 (r=35) -->
  <path d="M400 365 A35 35 0 0 0 365 400" fill="none" stroke="#534AB7" stroke-width="2.5" opacity="0.45"/>
  <path d="M365 400 A35 35 0 0 0 400 435" fill="none" stroke="#993C1D" stroke-width="2.5" opacity="0.45"/>
  <path d="M400 435 A35 35 0 0 0 435 400" fill="none" stroke="#0F6E56" stroke-width="2.5" opacity="0.45"/>
  <path d="M435 400 A35 35 0 0 0 400 365" fill="none" stroke="#854F0B" stroke-width="2.5" opacity="0.45"/>

  <!-- Volta 2 (r=90) -->
  <path d="M400 310 A90 90 0 0 0 310 400" fill="none" stroke="#534AB7" stroke-width="2.5" opacity="0.65"/>
  <path d="M310 400 A90 90 0 0 0 400 490" fill="none" stroke="#993C1D" stroke-width="2.5" opacity="0.65"/>
  <path d="M400 490 A90 90 0 0 0 490 400" fill="none" stroke="#0F6E56" stroke-width="2.5" opacity="0.65"/>
  <path d="M490 400 A90 90 0 0 0 400 310" fill="none" stroke="#854F0B" stroke-width="2.5" opacity="0.65"/>

  <!-- Volta 3 (r=170) — destaque -->
  <path d="M400 230 A170 170 0 0 0 230 400" fill="none" stroke="#534AB7" stroke-width="3.5"/>
  <path d="M230 400 A170 170 0 0 0 400 570" fill="none" stroke="#993C1D" stroke-width="3.5"/>
  <path d="M400 570 A170 170 0 0 0 570 400" fill="none" stroke="#0F6E56" stroke-width="3.5"/>
  <path d="M570 400 A170 170 0 0 0 400 230" fill="none" stroke="#854F0B" stroke-width="3.5"/>

  <!-- Center dot -->
  <circle cx="400" cy="400" r="6" fill="#534AB7" opacity="0.8"/>

  <!-- ========== DETAIL CARDS ========== -->

  <!-- Q1 card: Planejamento (top-left) -->
  <rect x="48" y="68" width="310" height="148" rx="10" fill="#EEEDFE" stroke="#534AB7" stroke-width="1.2"/>
  <text x="203" y="94" text-anchor="middle" font-size="13" font-weight="700" fill="#3C3489">Objetivos e restrições</text>
  <text x="64"  y="116" font-size="11.5" fill="#534AB7">· Escopo: profundidade, autonomia e precisão da IA</text>
  <text x="64"  y="134" font-size="11.5" fill="#534AB7">· Restrições: custo de hardware, regulações</text>
  <text x="64"  y="152" font-size="11.5" fill="#534AB7">  ANATEL / Marinha do Brasil</text>
  <text x="64"  y="170" font-size="11.5" fill="#534AB7">· Plano de iteração e alocação de recursos</text>
  <text x="64"  y="188" font-size="11.5" fill="#534AB7">· Critérios de entrada para Q2</text>

  <!-- Q2 card: Análise de Riscos (top-right) -->
  <rect x="442" y="68" width="310" height="148" rx="10" fill="#FAECE7" stroke="#993C1D" stroke-width="1.2"/>
  <text x="597" y="94" text-anchor="middle" font-size="13" font-weight="700" fill="#993C1D">Identificação de riscos</text>
  <text x="458" y="116" font-size="11.5" fill="#993C1D">· Falha do modelo IA em água turva</text>
  <text x="458" y="134" font-size="11.5" fill="#993C1D">· Latência de comunicação sônica (&gt;200 ms)</text>
  <text x="458" y="152" font-size="11.5" fill="#993C1D">· Falha de sensores por pressão hidrostática</text>
  <text x="458" y="170" font-size="11.5" fill="#993C1D">· Deriva de posicionamento sem GPS</text>
  <text x="458" y="188" font-size="11.5" fill="#993C1D">· Protótipo em tanque para validação</text>

  <!-- Q3 card: Desenvolvimento (bottom-right) -->
  <rect x="442" y="584" width="310" height="148" rx="10" fill="#E1F5EE" stroke="#0F6E56" stroke-width="1.2"/>
  <text x="597" y="610" text-anchor="middle" font-size="13" font-weight="700" fill="#0F6E56">Implementação técnica</text>
  <text x="458" y="632" font-size="11.5" fill="#0F6E56">· Fine-tuning de modelo de visão computacional</text>
  <text x="458" y="650" font-size="11.5" fill="#0F6E56">· Módulo de navegação autônoma com sonar</text>
  <text x="458" y="668" font-size="11.5" fill="#0F6E56">· DVL para odometria subaquática (fallback)</text>
  <text x="458" y="686" font-size="11.5" fill="#0F6E56">· Deploy embarcado (NVIDIA Jetson Orin)</text>
  <text x="458" y="704" font-size="11.5" fill="#0F6E56">· Suite de testes automatizados ≥ 85%</text>

  <!-- Q4 card: Avaliação (bottom-left) -->
  <rect x="48" y="584" width="310" height="148" rx="10" fill="#FAEEDA" stroke="#854F0B" stroke-width="1.2"/>
  <text x="203" y="610" text-anchor="middle" font-size="13" font-weight="700" fill="#854F0B">Avaliação do cliente</text>
  <text x="64"  y="632" font-size="11.5" fill="#854F0B">· Testes: piscina (sem. 9–10) → baía (sem. 11–12)</text>
  <text x="64"  y="650" font-size="11.5" fill="#854F0B">· Critério: detecção ≥ 92%, latência ≤ 180 ms</text>
  <text x="64"  y="668" font-size="11.5" fill="#854F0B">· Revisão com engenheiros navais e Marinha</text>
  <text x="64"  y="686" font-size="11.5" fill="#854F0B">· Aprovação da diretoria para próxima volta</text>
  <text x="64"  y="704" font-size="11.5" fill="#854F0B">· Decisão: avançar / replaneja / reitera</text>

  <!-- ========== DIRECTION INDICATOR ========== -->
  <!-- Arrow showing spiral direction (anti-clockwise), near volta 3 arc top -->
  <path d="M460 218 Q490 192 510 218" fill="none" stroke="#534AB7" stroke-width="2" marker-end="url(#arrowhead)"/>
  <text x="536" y="214" font-size="11" fill="#534AB7" font-weight="600">volta 3</text>
  <text x="536" y="228" font-size="11" fill="#534AB7">(atual)</text>

  <!-- Small rotation labels near center for volta 1 and 2 -->
  <text x="310" y="358" font-size="10" fill="#888" text-anchor="middle">volta 1</text>
  <text x="285" y="326" font-size="10" fill="#888" text-anchor="middle">volta 2</text>

  <!-- Arrowhead marker -->
  <defs>
    <marker id="arrowhead" viewBox="0 0 10 10" refX="8" refY="5" markerWidth="6" markerHeight="6" orient="auto-start-reverse">
      <path d="M2 1L8 5L2 9" fill="none" stroke="#534AB7" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"/>
    </marker>
  </defs>

  <!-- ========== LEGEND STRIP (center) ========== -->
  <rect x="302" y="378" width="196" height="44" rx="8" fill="white" fill-opacity="0.85" stroke="#b0aec8" stroke-width="0.8"/>
  <text x="400" y="396" text-anchor="middle" font-size="10.5" fill="#444" font-weight="600">Sentido: anti-horário</text>
  <text x="400" y="413" text-anchor="middle" font-size="10" fill="#666">Q1 → Q2 → Q3 → Q4 → próxima volta</text>

</svg>
ehm.svg…]()


---

## O diagnóstico CMMI

Nível 1 - Inicial.  
Evidências presentes na descrição: cada dev trabalha do seu jeito, prazos são "chutados" (sem planejamento baseado em dados históricos) e o sucesso depende de esforço individual.

## O que falta para chegar ao Nível 2 - Gerenciado?

Para subir ao Nível 2, a Chaos-IT precisa instituir as Áreas de Processo exigidas, que incluem: gerenciamento de requisitos, planejamento de projetos, monitoramento e controle de projetos, gestão de configuração e garantia de qualidade de processo e produto. Ou seja, exige que os mesmos processos básicos sejam repetidos de projeto em projeto, com registro.
