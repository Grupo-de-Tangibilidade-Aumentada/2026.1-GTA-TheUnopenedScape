# SGDD — Short Game Design Document

O **SGDD (*Short Game Design Document*)** reúne de forma objetiva as decisões de game design, fluxo de jogo, mecânicas e direção estética de **The Unopened Escape**.

## Documento Original

[Abrir SGDD no Google Docs](https://docs.google.com/document/d/19iKjf4_W0coSw6DeEdmJOn1mLrcc9Qn5BeEzh3aXI8o/edit?usp=sharing){ .md-button .md-button--primary target="_blank" }

!!! note "Sincronização"
    O documento colaborativo principal está hospedado no Google Docs. Utilize as seções abaixo para consolidar e versionar o conteúdo do SGDD diretamente nesta documentação.

## 1. Identidade do Jogo

- **Nome:** The Unopened Escape (*The Unopened Scape*)
- **High Concept:** Um minijogo cooperativo assimétrico de horror psicológico em que um jogador imerso em VR (Meta Quest) depende das instruções de um parceiro com acesso à interface mobile para resolver enigmas e escapar.
- **Público-Alvo:** *Definir faixa etária e perfil dos jogadores.*

## 2. Pilares de Design

1. **Cooperação Assimétrica:** informação dividida obriga comunicação constante entre VR e Mobile.
2. **Tensão Psicológica:** atmosfera opressiva construída com iluminação, silêncio e design sonoro.
3. **Interação Tangível:** puzzles manipuláveis diretamente com as mãos/controles em Realidade Virtual.

## 3. Core Gameplay Loop

1. **Explorar e Observar (VR):** o jogador em VR examina o ambiente e descreve símbolos, sons, botões ou mecanismos encontrados.
2. **Consultar e Decifrar (Mobile):** o jogador parceiro interpreta as pistas usando a interface/manual mobile e formula instruções.
3. **Executar e Validar (VR):** o jogador em VR aplica a solução nos dispositivos físicos do cenário.
4. **Progredir:** a validação libera novas etapas até o desbloqueio final do cofre/saída.

## 4. Mecânicas e Sistemas

| Sistema | Descrição |
| :--- | :--- |
| **Interação XR** | Manipulação de botões, alavancas, peças arrastáveis e elementos do cenário no Meta Quest. |
| **Puzzles** | Enigmas baseados em símbolos, sequências sonoras, ordenação e combinação final. |
| **Sistema de Áudio** | Ambiência dinâmica e pistas sonoras essenciais para imersão e resolução de desafios. |
| **Interface Mobile / Manual** | Apoio visual e diagramado (Figma) consultado pelo segundo jogador. |

## 5. Fluxo de Telas e Progressão

- **Menu Inicial:** entrada na experiência, ajustes básicos e início da partida.
- **Sessão de Jogo:** sequência de puzzles interligados até a abertura final.
- **Encerramento:** tela/evento de conclusão (vitória ou falha).

## 6. Escopo Técnico

- **Motor:** Unity Engine + C#
- **Dispositivo VR:** Meta Quest
- **Design de Interfaces e Manuais:** Figma

## Histórico de Versões

| Versão | Data | Descrição | Autor(es) |
| :---: | :---: | :--- | :--- |
| `0.1` | 2026-11-27 | Criação inicial da página de SGDD | Equipe GTA |
