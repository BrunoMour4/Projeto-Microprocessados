# Projeto Final - Sistemas Microprocessados
## Interfaceando Sensor Ultrassônico no STM32

Link do vídeo: [Sensor Ultrassônico no STM32](https://www.youtube.com/watch?v=N5KTY0HST3M)

Aluno: **Bruno Moura - 396433**

## Proposta

A proposta do projeto, aqui disposto, foi implementar a interface do sensor ultrassônico HC-SR04 no microprocessador stm32f103c6. Semelhante ao sonar dos morcegos, o sistema do sensor ultrassônico tem como princípio de funcionamento a emissão de uma onda sonora de alta frequência. O objeto a ser detectado (que é capaz de refletir essa onda) resulta em um eco, que é convertido em sinais elétricos. A detecção desse eco depende da intensidade e da distância entre o objeto e o sensor. É a partir disso que se sabe se o objeto está dentro dos parâmetros estabelecidos, ou mesmo se está no local para o sensor identifica-lo. Na prática, isso significa que por meio do sensor ultrassônico, é possível, por exemplo: 

- Registrar a posição dos objetos
- Realizar a medição de distância ou o registro de meios sólidos, em pó ou líquido
- Medir níveis
- Contar objetos
- Medir o diâmetro de bobinas

E o melhor: o sensor ultrassônico apresenta uma detecção confiável e sem contato, independente da textura, cor ou formato do objeto a ser identificado, o que inclui itens transparentes. A presença de névoa, poeira ou sujeira também não influencia no resultado da detecção. 

## Configuração dos pinos no microcontrolador

O pino PA9 (*output*) está conectado ao pino TRIG do sensor. O pino PA8 (*input*), por sua vez, está conectado ao pino ECHO do sensor. Os pinos PB0, PB1, PB2, PB3, PB4, PB5, PB6, PB7, PB8 e PB9 fazem a interface do display LCD que exibe a distância medida em cm. O timer 1 é utilizado para a contagem do tempo.


![alt text](https://i.ibb.co/BPw0Px0/Capturar.png)

## Flowchart da implementação

![alt text](https://i.ibb.co/2YpRw7v/flowchart.png)

## Simulação no Proteus

![alt text](https://i.ibb.co/6nKDRYp/proteus.png)


