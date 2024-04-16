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

### HIPÓTESES
- A porta da geladeira quando permanece aberta aumenta a temperatura interna, causando o
desperdício de energia, desgastando desnecessariamente os componentes e acelerando a deterioração
de alimentos.
   * Um LED indica o estado da porta (aberta/fechada).
   * O sensor de distância corresponde ao estado da porta.
   * Após um tempo definido pelo usuário o buzzer alertará até a porta ser fechada.
   
- O funcionamento indadequado dos componentes podem ocasionar os problemas citados acima, fazendo-se
necessário o monitoramento da temperatura pelo sistema.
   * A temperatura atual é monitorada constantemente, com exibição no display.
   * A temperatura alvo pode ser controlada pelo usuário utilizando o teclado matricial.

- O usuário terá possibilidade de controlar a temperatura alvo e o tempo do alerta quando a porta permanece aberta.

### ESBOÇO DA CONFIGURAÇÃO DOS PERIFÉRICOS
![Print do esboço](https://github.com/KaiqueZambrano/2024-1_Projeto_Equipe_9/blob/main/lab5.drawio.png)

### DIVISÃO DE TAREFAS
- Implementar push buttons, LEDs e teclado matricial.
    * Push buttons:
      * Controle da exibição do display (modo temperatura/modo timer).
    * LEDs:
      * Estado da porta.
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
