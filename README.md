# Formiga Mecatrônica
Projeto final de Sistemas Embarcados para Veículos Aéreos 

## Alunos/Desenvolvedores
*[Felipe](#Alunos/Desenvolvedores)

*[Rodrigo](#Alunos/Desenvolvedores)

*[Esther Eleotério Panequi Ferreira ](https://github.com/theursaparda)

# Introdução
Esse projeto foi desenvolvido para a criação de um robô com implementação de movimento lógico atrvés de um sistema de hadware, apartir de uma placa da **Toradex**, e duas **MBEDs**. Com uma saída **PWM** controlando os 12 servos motores (2 por perna), pretendendo no final criar-se uma lógica para sua moviementação na Toradex, onde envia comando para as MBEDs, onde é programada para interpretar e realizar os comandos enviados comandadno seus motores respecivos.

# Proposta
O contexto desse projeto é desenvolver um código para um robô hexapode, onde seu código e sua comunicação seja clara e eficiente, para futuros aprimoramentos e adaptações, usando o PWM para os protocolos de comunicação onde informa as posições dos servos e a CAN para realização da comunicação entre os processadoes. O movimento foi criado com o menor número de variáveis possíveis, com uma movimentação lógica na toradex para processar e enviar o minimo de mensagens possíveis para MBED, onde processa e cria os movimentos do mootr.

# Entendendo o Sistema
# Desenvolvimento
## Desenvolvimento Lógico
A partir da proposta do movimento do robô foi analisada a criar uma interação entre as pernas. Onde as pernas ímpares e pares se comunicam para que as ímpares empurrem o chão e as pares levantem e se movimentam para frente, com isso o movimento dos dois **serovos** da perna sejam realizados por apenas uma variável, diminuindo a mensagem a ser enviada. No qual seja importante que a trajetória seja feita apenas por um sistema, que no caso seria a toradex, para garantir a sincronização dos movimentos, desenvolvimento de cálculos de trajetória futuras, e que os sinais sejam enviados para as duas MBEDs.
A toradex recebe o movimento desejado pelo usuário, onde decide que movimento cada perna realizará o movimento, assim enviado para as MBEDs qual ação será realizada por cada perna, quando a MBED receber a mensagem ela desenvolve o movimento sozinha até que acabe os ciclos completos dos movimentos.

## Desenvolvimento Código

## Desenvolvimento Comunicação



# Conclusão
