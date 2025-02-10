Projeto: Comunicação Serial e Controle de Periféricos na BitDogLab

Este projeto demonstra o uso de interfaces de comunicação serial (UART e I2C) e o controle de periféricos (LEDs, botões e display OLED) na placa de desenvolvimento BitDogLab, utilizando o microcontrolador RP2040.

Objetivos

Compreender o funcionamento e a aplicação de comunicação serial em microcontroladores.
Aplicar os conhecimentos adquiridos sobre UART e I2C na prática.
Manipular e controlar LEDs comuns e LEDs endereçáveis WS2812.
Fixar o estudo do uso botões de acionamento, interrupções e Debounce.
Desenvolver um projeto funcional que combine hardware e software.

Componentes

Matriz 5x5 de LEDs (endereçáveis) WS2812 (GPIO 7)
LED RGB (GPIO 11, 12 e 13)
Botão A (GPIO 5)
Botão B (GPIO 6)
Display SSD1306 (I2C - GPIO 14 e GPIO 15)

Funcionalidades

Modificação da Biblioteca font.h:

Foram adicionados caracteres minúsculos à biblioteca font.h para possibilitar a exibição de mensagens no display OLED com letras minúsculas.
Entrada de caracteres via PC:

Utilização do Serial Monitor do VS Code para digitar caracteres.
Cada caractere digitado é exibido no display SSD1306.
Números de 0 a 9, quando digitados, acendem os LEDs correspondentes na matriz 5x5 WS2812.

Interação com o Botão A:

A pressão do botão A alterna o estado do LED RGB Verde (ligado/desligado).
O estado do LED é exibido no display SSD1306 e enviado para o Serial Monitor.

Interação com o Botão B:

A pressão do botão B alterna o estado do LED RGB Azul (ligado/desligado).
O estado do LED é exibido no display SSD1306 e enviado para o Serial Monitor.

Instruções de Uso

Clone este repositório.

Instale o SDK do Pico e configure o ambiente de desenvolvimento.

Conecte os componentes à placa BitDogLab de acordo com o esquema de ligação.

Compile o código e carregue-o para o RP2040.

Abra o Serial Monitor do VS Code para interagir com o projeto.
