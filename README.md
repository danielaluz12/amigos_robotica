# amigos_robotica

## Grupo amigos da robótica

Daniela Ramos Luz 10883832

Heloísa Vargas  9912869

Lucas Fiorotti 10746686

## Objetivo
Desevolver interface para operação com envio de instruções de comando e recepção e apresentação de estado do equipamento da Manopla robotizada
MOREW -reabilitação de punho. 
Para tanto é preciso entender cada um dos sistemas que compõe o projeto. A ideia é criar uma interface gráfica no computador Host que consiga se comunicar tanto com o Hardware Computacional quanto com o motor e seu encoder.
Para tanto imagina-se implementar uma comunicação via socket entre o Host com a interface gráfica e a placa de Hardware Computacional VIOLA + VF Toradex, e uma comunicação CAN entre a placa de implementação e motor e seu enconder. Um esquemático de como seria esse modelo pode ser visto abaixo:

 ![image](https://user-images.githubusercontent.com/71453516/166116547-45b5193a-db7b-4348-a75c-2a7ec504035e.png)

Analisando o que já foi feito no último desenvolvimento deste tema pelo grupo do ano passado que está no seguinte diretório [ https://github.com/VicDaArSh/Trabalho_Embarcados_2 ], pode-se entender que um protótipo inicial de  interface gráfica para o Host foi criada usando a biblioteca PyQt5 de Python, que permite criar aplicações de GUI usando o toolkit de design de telas Qt. A comunicação entre o Host e VIOLA + VF Toradex, também foi implementada usando socket, ou seja criando um server no Host que recebe e envia comandos para o client, implementado na  VIOLA + VF Toradex.

Pensando nas tarefas que ainda não foram desenvolvidas, segue uma lista do que pode ser implementado:

- Criar código em C para porta CAN, tendo comunicação de escrita com motor e leitura do encoder
- Melhorias na parte visual da interface gráfica
- Implementação de novas funcionalidades na interface gráfica
- entre outros
