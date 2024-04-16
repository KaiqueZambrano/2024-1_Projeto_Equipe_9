# (2024/1) EQUIPE 9
Projeto da disciplina "Sistemas Microcontrolados".

## PROPOSTA
A inexistência de alertas sonoros ou visuais quando portas de geladeiras antigas não são
fechadas pode acarretar desperdício de energia, desgastar desnecessariamente os componentes
e acelerar a deterioração de alimentos. É um problema mais acessível que gerenciamento de
energia em servidores, que é um assunto extenso e pouco prático para desenvolver durante a
disciplina. O problema escolhido é mais simples e o uso de recursos também é mais claro. O kit
disponível possui uma variedade de periféricos, como display, teclado matricial alfanumérico,
buzzer e relé, que podem ser integrados ao projeto para fornecer tanto alertas sonoros quanto
visuais. O PIC18F4550 também conta com alguns sensores internos para temperatura, assim
como outros periféricos úteis.

## DESENVOLVIMENTO

### DIVISÃO DE TAREFAS
- Implementar push buttons, LEDs e teclado matricial.
    * Push buttons:
      * Ação de abertura da porta (aberta/fechada).
      * Controle da exibição do display (modo temperatura/modo timer).
    * LEDs:
      * Estado da porta.
      * Temperatura baixa.
      * Temperatura normal.
      * Temperatura alta.
    * Teclado matricial:
      * Escrita no display.
- Implementar o display.
    * Exibir a temperatura do sensor.
    * Interface para o controle de temperatura.
    * Interface para o controle do temporizador (alerta).
- Implementar o buzzer.
    * Alerta indicando porta aberta.
    * Resposta para o acionamento dos botões.
- Implementar potenciômetro.
    * Implementar sistema de controle de temperatura.
- Implementar ventoinha.
    * Ativação da ventoinha, de acordo com a temperatura.
