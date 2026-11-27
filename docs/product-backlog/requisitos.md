# Requisitos

## 1. Introdução

Esta página documenta os requisitos levantados para o desenvolvimento de **The Unopened Escape**. Todo o levantamento apresentado abaixo foi elaborado **exclusivamente a partir do Jogo Mental** descrito em [Descrição do Jogo](../descricao-do-jogo.md), contemplando a inicialização, as interações e ambientação das áreas do jogo e a experiência do aplicativo do Jogador 2. Os requisitos referentes aos desfechos de fim de jogo serão adicionados futuramente, após sua definição final.

## 2. Metodologia e Estrutura

Os requisitos estão divididos em **Requisitos Funcionais (RF)** — comportamentos, mecânicas e fluxos que o sistema deve executar — e **Requisitos Não Funcionais (RNF)** — critérios de estética, áudio, usabilidade e compatibilidade de hardware.

Cada tabela segue o padrão de colunas abaixo:

- **ID:** identificador único do requisito (`RF01`... para funcionais e `RNF01`... para não funcionais).
- **Descrição:** especificação objetiva do comportamento ou qualidade esperada.
- **Categoria:** agrupamento temático do requisito conforme a etapa ou dimensão do jogo.
- **Referência:** rastreabilidade para a frase específica da descrição do jogo que deu origem ao requisito.
- **Versão:** versão atual da especificação de cada requisito.

## 3. Requisitos Funcionais (RF)

|   ID   | Descrição                                                                                                                                                                                                                                                      | Categoria          | Referência | Versão |
| :----: | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :----------------- | :--------- | :----: |
| `RF01` | O sistema deve exibir uma tela de carregamento inicial contendo os nomes dos estudantes e do professor envolvidos no projeto, tanto para o Jogador 1 quanto para o Jogador 2.                                                                                  | Inicialização      |            | `1.0`  |
| `RF02` | O jogo do Jogador 1 deve apresentar uma recomendação expressa para o uso de fones de ouvido logo após a tela de carregamento.                                                                                                                                  | Inicialização      |            | `1.0`  |
| `RF03` | O sistema deve manter o Jogador 1 preso e imóvel em uma cadeira de ferro enferrujada na Área 1, restringindo sua interação com o ambiente ao uso de mãos virtuais flutuantes.                                                                                  | Área 1             |            | `1.0`  |
| `RF04` | O sistema deve permitir que o Jogador 1 segure o rádio velho sobre a mesa e ajuste o volume da música e dos sons do jogo através dos botões do aparelho.                                                                                                       | Área 1             |            | `1.0`  |
| `RF05` | O sistema deve retornar automaticamente o rádio à sua posição padrão sobre a mesa sempre que o Jogador 1 o soltar ou arremessar.                                                                                                                               | Área 1             |            | `1.0`  |
| `RF06` | O sistema deve disponibilizar um cubo mecânico no centro da mesa que o Jogador 1 pode segurar e girar horizontalmente em torno do próprio eixo (da direita para a esquerda), fixando e centralizando automaticamente a face mais próxima dos olhos do usuário. | Área 1             |            | `1.0`  |
| `RF07` | O sistema deve travar o movimento vertical do cubo de baixo para cima e permitir a visualização da face superior apenas enquanto o jogador arrasta e segura de cima para baixo, retornando o cubo à posição normal ao soltá-lo.                                | Área 1             |            | `1.0`  |
| `RF08` | O cubo mecânico deve iniciar sempre exibindo uma face vazia com uma seta desgastada riscada, instruindo o jogador a girar o cubo como tutorial de movimentação.                                                                                                | Área 1             |            | `1.0`  |
| `RF09` | O cubo mecânico deve possuir uma face de Autenticação que permite selecionar uma combinação de dois números girando engrenagens mecânicas (aumentar/diminuir) e confirmar a senha por meio de um botão.                                                        | Área 1             |            | `1.0`  |
| `RF10` | O cubo mecânico deve possuir um botão de Configuração que, ao ser pressionado, faz o rádio emitir um som e piscar com um contorno branco por alguns segundos para indicar que o volume de som e música é ajustado nele.                                        | Área 1             |            | `1.0`  |
| `RF11` | O cubo mecânico deve possuir um botão de Sair que, ao ser pressionado, apaga lentamente a luz _spotlight_, faz o rádio chiar intensamente até desligar e mantém _blackout_ total e silêncio absoluto por 2 segundos antes de encerrar o aplicativo.            | Área 1             |            | `1.0`  |
| `RF12` | Ao pressionar o botão de Autenticar, o sistema deve reconhecer a credencial como falsa, acionar o Protocolo Anti-Intruso com um alarme estridente e arrastar mecanicamente a cadeira do Jogador 1 através de uma escotilha no teto até a Área 2.               | Área 1             |            | `1.0`  |
| `RF13` | Ao chegar à Área 2, o sistema deve fechar a escotilha e aplicar um efeito visual de ofuscamento pela mudança repentina de iluminação, recuperando gradualmente a visão do personagem.                                                                          | Área 2             |            | `1.0`  |
| `RF14` | O sistema deve disponibilizar na mesa central da Área 2 um cofre rústico contendo os puzzles em suas faces manipuláveis e uma sinalização com luzes na face superior indicando a quantidade de puzzles resolvidos.                                             | Área 2             |            | `1.0`  |
| `RF15` | O sistema deve iniciar a contagem de tempo em um relógio digital no canto da mesa ao começar a etapa na Área 2, controlando o limite temporal da partida.                                                                                                      | Área 2             |            | `1.0`  |
| `RF16` | O sistema deve disparar eventos aleatórios durante a partida na Área 2, incluindo luzes piscando agressivamente e barulhos altos, para gerar desconforto e quebrar a comunicação entre os jogadores.                                                           | Área 2             |            | `1.0`  |
| `RF17` | Ao errar um puzzle, o sistema deve aplicar punição emitindo um som de erro, decrescendo segundos do relógio e exibindo um número vermelho flutuante acima do display com trajetória de baixo para cima que desaparece após um tempo.                           | Área 2             |            | `1.0`  |
| `RF18` | Após a tela de carregamento, o aplicativo do Jogador 2 deve exibir uma tela inicial com vídeo do galpão simulando visão de câmera e um botão "Iniciar" centralizado.                                                                                           | Jogador 2 (Mobile) |            | `1.0`  |
| `RF19` | Ao acionar "Iniciar", o aplicativo do Jogador 2 deve ativar a câmera do smartphone exibindo uma marcação gráfica centralizada e a instrução visual "Aponte o QR Code das instruções".                                                                          | Jogador 2 (Mobile) |            | `1.0`  |
| `RF20` | Ao apontar a câmera para o QR Code de uma carta física, o aplicativo do Jogador 2 deve identificar o marcador e abrir um documento fixo na tela (similar a um PDF) com as instruções correspondentes ao puzzle específico daquela carta.                       | Jogador 2 (Mobile) |            | `1.0`  |
| `RF21` | O aplicativo do Jogador 2 deve disponibilizar um botão "Voltar" no topo da tela do documento para retornar à câmera sempre que o jogador precisar escanear uma nova carta física.                                                                              | Jogador 2 (Mobile) |            | `1.0`  |

## 4. Requisitos Não Funcionais (RNF)

|   ID    | Descrição                                                                                                                                                                                                                                                                     | Categoria             | Referência | Versão |
| :-----: | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :-------------------- | :--------- | :----: |
| `RNF01` | O ambiente da Área 1 — quarto pequeno, degradado, escuro e sem janelas, com cadeira de ferro enferrujada, mesa de madeira desgastada e luz _spotlight_ natural vinda de cima — deve seguir a temática de horror psicológico com realismo sombrio e sujo.                      | Estética e Arte       |            | `1.0`  |
| `RNF02` | O ambiente da Área 2 — galpão claustrofóbico e sujo com ratos correndo pelo chão eventualmente, câmera discreta identificada apenas pela luz de ligada e janela ao fundo com vista para um bosque — deve manter a estética de horror psicológico com realismo sombrio e sujo. | Estética e Arte       |            | `1.0`  |
| `RNF03` | As mãos virtuais flutuantes do Jogador 1 devem apresentar aparência levemente ferida e suja, condizente com a temática sombria do jogo.                                                                                                                                       | Estética e Arte       |            | `1.0`  |
| `RNF04` | A Área 1 deve manter ambientação sonora constante composta por música ambiente agonizante proveniente do rádio, acompanhada por ruídos de goteiras, faíscas elétricas e passos fortes vindos do teto.                                                                         | Áudio e Imersão       |            | `1.0`  |
| `RNF05` | As interações com o cubo mecânico devem reproduzir feedback sonoro característico de mecanismo analógico antigo.                                                                                                                                                              | Áudio e Imersão       |            | `1.0`  |
| `RNF06` | Os documentos abertos no aplicativo do Jogador 2 devem ser estilizados na temática de horror psicológico, assemelhando-se a um manual de instruções velho com anotações corridas feitas à mão e ilustrações misteriosas.                                                      | Estética e Arte       |            | `1.0`  |
| `RNF07` | As cartas físicas utilizadas pelo Jogador 2 devem apresentar estética eldritchiana e mítica.                                                                                                                                                                                  | Estética e Arte       |            | `1.0`  |
| `RNF08` | As interações devem fornecer feedback diegético e visual claro para guiar os jogadores sem quebrar a imersão.                                                                                                                                                                 | Usabilidade           |            | `1.0`  |
| `RNF09` | O aplicativo do Jogador 2 deve operar em smartphone com acesso funcional à câmera para leitura dos marcadores QR Code presentes nas cartas físicas.                                                                                                                           | Plataforma e Hardware |            | `1.0`  |

## Pendências

- Devemos elaborar a história do jogo para definir os requisotos relacionados ao desfecho do jogo e demais outros requisitos neceśsarios a depender da escolha da lore.

## 5. Histórico de Versões

| Versão |    Data    | Descrição                                 | Autor(es)                                        |
| :----: | :--------: | :---------------------------------------- | :----------------------------------------------- |
| `0.1`  | 27/11/2026 | Estrutura inicial da página de Requisitos | [Yan Matheus](https://github.com/Yanmatheus0812) |
