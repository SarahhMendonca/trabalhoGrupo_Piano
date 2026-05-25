# Piano Eletrônico de 11 Notas com Arduino ✨💗🎶

Este projeto consiste em um piano eletrônico simplificado desenvolvido no **Tinkercad**, capaz de reproduzir 11 notas musicais diferentes utilizando botões (push-buttons) e um buzzer.

## 🚀 Visão Geral
O projeto utiliza uma placa Arduino Uno para ler as entradas de 11 botões. Cada botão está associado a uma frequência específica, permitindo ao usuário tocar escalas musicais básicas.

## 🛠️ Componentes Utilizados
* 1x Arduino Uno R3
* 1x Piezo Buzzer
* 11x Botões (Push-buttons)
* 11x Resistores de 10kΩ (configuração Pull-Down)
* 2x Protoboards
* Jumpers de conexão

## 📋 Pinagem e Configuração
As notas estão mapeadas nos seguintes pinos digitais do Arduino:

| Nota | Pino Arduino | Frequência (Hz) |
| :--- | :---: | :---: |
| DO  | 2 | 200 |
| RE  | 3 | 225 |
| MI  | 4 | 250 |
| FA  | 5 | 260 |
| SOL | 6 | 290 |
| LA  | 7 | 330 |
| SI  | 8 | 370 |
| DO2 | 9 | 400 |
| FAS | 10 | 450 |
| RE2 | 11 | 495 |
| MI2 | 12 | 520 |
| **Buzzer** | **13** | - |

## 💻 Funcionamento do Código
O código-fonte segue uma lógica direta de leitura e resposta:
1. **Definição de Variáveis**: Cada nota e o buzzer recebem um nome associado ao seu pino digital.
2. **Setup**: Configura os pinos dos botões como entradas (`INPUT`) e o buzzer como saída (`OUTPUT`).
3. **Loop**: Realiza a leitura digital (`digitalRead`) de cada botão. Se o valor for igual a 1 (pressionado), a função `tone()` é acionada para gerar o som na frequência programada.

## ⚙️ Esquema de Ligação
* Os botões estão conectados ao barramento positivo (5V).
* Resistores de 10kΩ conectam a saída do botão ao GND (Pull-down).
* O sinal de cada botão é enviado para os pinos digitais 2 a 12 do Arduino.
* O Buzzer Piezo está conectado ao pino 13 e ao GND.

---
**Programadora:** Sarah Mendonça  🦋🌸🪻
*Projeto desenvolvido para fins educacionais e prática de eletrônica básica.* 🎹✨
