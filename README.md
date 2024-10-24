# Flappy Dev

Flappy Dev é um jogo inspirado no clássico "Flappy Bird", onde o jogador controla um pássaro que precisa voar entre canos sem colidir. O objetivo é passar pelo maior número possível de canos para aumentar sua pontuação.

## Requisitos

- Navegador web moderno (Chrome, Firefox, Edge, etc.)

## Como Jogar

1. Abra o arquivo `index.html` no seu navegador.
2. O jogo começará assim que uma tecla for pressionada (espaço, seta para cima, ou "X").
3. Pressione espaço, seta para cima ou "X" para fazer o pássaro voar.
4. Desvie dos canos e tente alcançar a maior pontuação!

## Controles

- **Espaço/Seta para cima/Tecla "X"**: Faz o pássaro voar.
- O pássaro desce automaticamente com a gravidade, então você precisará continuar pressionando para mantê-lo no ar.

## Estrutura do Jogo

- **Pássaro**: Controlado pelo jogador, ele sobe quando uma tecla é pressionada e desce devido à gravidade.
- **Canos**: Aparecem continuamente do lado direito da tela e se movem para a esquerda. O jogador deve passar por entre eles sem colidir.
- **Pontuação**: Aumenta toda vez que o jogador passa com sucesso por um conjunto de canos.
- **Fim de Jogo**: O jogo termina se o pássaro colidir com um cano ou cair no chão. Uma mensagem de "Game Over" será exibida.

## Imagens e Sons

- **Sprites do Pássaro**: O pássaro tem três estados visuais — asas para cima, para baixo e no meio — que são atualizados de acordo com o movimento.
- **Canos**: Canos superiores e inferiores são renderizados na tela e posicionados de forma aleatória.
- **Sons**: 
  - `hit.wav`: Tocado quando o pássaro colide com um cano.
  - `wing.wav`: Tocado quando o pássaro sobe.
  - `point.wav`: Tocado quando o jogador ganha um ponto.

## Física

- **Gravidade**: O pássaro desce automaticamente devido à gravidade (0.4 por frame).
- **Velocidade de movimento dos canos**: Os canos se movem da direita para a esquerda com uma velocidade constante (-2).

## Colisões

O jogo detecta colisões entre o pássaro e os canos usando uma simples verificação de sobreposição de caixas delimitadoras. Se houver colisão, o jogo termina.

## Pontuação

A pontuação é calculada toda vez que o pássaro passa com sucesso por um conjunto de canos. A pontuação é desenhada no topo da tela, centrada horizontalmente.

## Reiniciando o Jogo

Quando o jogo termina, o jogador pode pressionar qualquer uma das teclas de controle novamente para reiniciar o jogo, resetando a pontuação e a posição do pássaro.

## Tecnologias Utilizadas

- **HTML5 Canvas**: Utilizado para desenhar os elementos do jogo.
- **JavaScript**: Lógica de jogo, física e controle de eventos.
- **CSS**: Estilização básica da página.
- **Sprites e Áudio**: Usados para melhorar a experiência visual e sonora.

## Como Executar Localmente

1. Clone o repositório ou faça o download dos arquivos.
2. Certifique-se de que todos os arquivos, incluindo os sprites e sons, estão na pasta `assets` correspondente.
3. Abra o arquivo `index.html` no seu navegador.


