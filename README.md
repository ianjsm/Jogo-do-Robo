# Robô em Busca de Alimento

Este é um projeto simples que simula um robô em busca de alimento em um espaço bidimensional. O projeto é dividido em várias classes e funcionalidades para atingir esse objetivo.

## Exceção MovimentoInvalidoException

Para lidar com movimentos inválidos, foi criada uma exceção personalizada chamada `MovimentoInvalidoException`. Essa exceção é lançada quando o robô tenta fazer um movimento que o levaria para uma posição negativa no eixo cartesiano.

## Classe Robô

A classe `Robo` representa o personagem robô neste projeto. Ela possui os seguintes atributos:
- Posição no eixo x.
- Posição no eixo y.
- Cor que identifica o robô.

A classe possui um construtor que permite inicializar o robô com uma cor específica e inicia o robô na posição (0, 0). Além disso, há métodos de acesso (getters e setters) para as posições do robô.

## Método de Movimento

A classe `Robo` também possui um método `mover` que permite ao robô se mover no espaço bidimensional. Esse método aceita uma string que representa o movimento desejado: "up", "down", "right" ou "left". Se o movimento resultar em uma posição negativa em qualquer eixo, a exceção `MovimentoInvalidoException` será lançada, e o movimento não será permitido. Após cada movimento, a posição atual do robô será exibida.

Além disso, o método `mover` foi sobrecarregado para aceitar um inteiro de 1 a 4, onde 1 representa "up", 2 representa "down", 3 representa "right" e 4 representa "left".

## Método de Verificação de Alimento

A classe `Robo` possui um método que verifica se o robô encontrou o alimento, ou seja, se está na mesma posição que o alimento. Esse método retorna um valor booleano.

## Classe Main

A classe `Main` é responsável por instanciar um robô, pedir ao usuário para determinar a posição do alimento e, em seguida, permitir que o usuário mova o robô até encontrar o alimento. A exceção `MovimentoInvalidoException` é tratada para garantir que o robô não saia da área permitida.

Este projeto demonstra a criação de uma classe personalizada de exceção, a implementação de um robô com funcionalidades de movimento e verificação de alimento, e a interação do usuário para controlar o robô em busca do alimento.
