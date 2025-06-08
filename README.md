# Grua Eletromagnética com Arduino e Bluetooth 🔧🧲

Este projeto apresenta o desenvolvimento de uma grua eletromagnética automatizada com controle via *Bluetooth. A estrutura foi construída com materiais recicláveis (palitos de sorvete) e utiliza **Arduino UNO, **3 motores DC, **duas pontes H, **relé, e um **módulo Bluetooth HC-05* para comando remoto.

## 📌 Funcionalidades

- Movimentação *vertical* (içamento do eletroímã)
- Movimentação *horizontal* (em trilho de impressora)
- *Rotação no eixo* da grua
- Controle *ligar/desligar do eletroímã* por relé
- Parada automática dos motores após inatividade
- Controle via aplicativo Bluetooth de celular (Serial Bluetooth Terminal ou similar)

## 🔌 Hardware Utilizado

- Arduino UNO
- 3 Motores DC (2 reciclados de impressoras)
- 2 Módulos Ponte H L298N
- 1 Módulo Relé 5V
- Módulo Bluetooth HC-05
- Fonte de 12V ou 4x pilhas AA
- Fios jumper, protoboard e palitos de sorvete (estrutura)
- Eletroímã caseiro com fio de cobre esmaltado e núcleo metálico

## ⚙️ Diagrama de Conexão (Resumo)

| Componente | Pinos Arduino |
|------------|----------------|
| Motor A    | IN1 (4), IN2 (5), ENA (6) |
| Motor B    | IN3 (8), IN4 (9), ENB (10) |
| Motor C    | IN5 (7), IN6 (12), ENA2 (11) |
| Relé       | 13 |
| Bluetooth  | RX (2), TX (3) |

## 📱 Comandos Bluetooth

- F – Motor A frente  
- B – Motor A ré  
- G – Motor B frente  
- H – Motor B ré  
- L – Motor C frente  
- M – Motor C ré  
- R – Liga o eletroímã (relé ON)  
- S – Desliga o eletroímã (relé OFF)

## 🧠 Lógica de Parada Automática

O sistema monitora a última ação de controle dos motores. Se nenhum comando for recebido por *300 ms*, os motores são automaticamente desligados para preservar energia e evitar travamentos.

## 📂 Código

O código-fonte completo está no arquivo [grua_eletromagnetica.ino](./grua_eletromagnetica.ino).

## 📸 Estrutura Física

A estrutura foi construída com palitos de sorvete seguindo o princípio de treliça. Motores foram fixados em suportes de madeira. Todo o projeto foi feito sem uso de parafusos ou pregos, conforme regras estabelecidas.

## ♻️ Sustentabilidade

O projeto tem como foco a reutilização de materiais eletrônicos (motores, trilhos e fios) e o uso de estrutura reciclável, atendendo aos Objetivos de Desenvolvimento Sustentável (ODS 4, 9 e 12).

## 📘 Licença

Este projeto é de uso educacional e está licenciado sob a [MIT License](LICENSE).

---

### 👨‍💻 Desenvolvido por

- Guilherme Feitosa Santana - 823111787
- Victor Henrique da Silva Perillo Brasil 823130525
- Breno Ramos dos Santo – 823159781
- Guilherme dos Santos Coelho - 823120490

- Universidade [Universidade são judas thadeu - USJT - campus Mooca]
