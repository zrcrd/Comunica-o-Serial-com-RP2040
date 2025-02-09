🛠️ Projeto: Interfaces de Comunicação Serial com RP2040
📑 Sumário
🎯 Objetivos
📋 Descrição do Projeto
⚙️ Funcionalidades Implementadas
🛠️ Requisitos do Projeto
📂 Estrutura do Repositório
🖥️ Como Compilar
🤝 Contribuições
📽️ Demonstração em Vídeo
💡 Considerações Finais
🎯 Objetivos
Compreender o funcionamento e a aplicação de comunicação serial em microcontroladores.
Aplicar na prática os conceitos de UART e I2C.
Manipular LEDs comuns e LEDs endereçáveis WS2812.
Implementar soluções para botões com interrupções e debounce.
Desenvolver um projeto que combina hardware e software.
📋 Descrição do Projeto
Este projeto utiliza a placa BitDogLab com os seguintes componentes:

Matriz 5x5 de LEDs WS2812 (GPIO 7)
LED RGB (GPIOs 11, 12 e 13)
Botão A (GPIO 5)
Botão B (GPIO 6)
Display SSD1306 via I2C (GPIO 14 (SDA) e GPIO 15 (SCL))
⚙️ Funcionalidades Implementadas
Modificação da Biblioteca font.h:

Adição de caracteres minúsculos criativos.
Entrada de Caracteres via Serial Monitor:

Exibição de cada caractere no display SSD1306.
Exibição de símbolos na matriz 5x5 para números entre 0 e 9.
Interação com Botões:

Botão A: Alterna o estado do LED Verde RGB com registro no display e Serial Monitor.
Botão B: Alterna o estado do LED Azul RGB com registro no display e Serial Monitor.
🛠️ Requisitos do Projeto
Uso de Interrupções: Controlar os eventos dos botões.
Debouncing: Implementação via software.
Controle de LEDs: Utilização dos LEDs comuns e da matriz WS2812.
Uso do Display SSD1306: Exibição de fontes maiúsculas e minúsculas.
Comunicação via UART: Envio de informações ao Serial Monitor.
Organização do Código: Código estruturado e comentado.
📂 Estrutura do Repositório
├── tarefaU403fev.c      # Código principal do projeto
├── font.h               # Biblioteca com fontes modificadas
├── README.md            # Este arquivo
└── ws2818b.pio.h        # Biblioteca para configuração da matriz de led
└── ssd1306.c            # Configuração dos cos caracteres a serem exibidos no display
└── ssd1306.h            # Configura a .c como biblioteca
└── ...                  # Demais arquivos necessários
🖥️ Como Compilar
Clone o repositório:

Navegue até o diretório do projeto:
cd tarefaU403fev
Compile o projeto com seu ambiente de desenvolvimento configurado para o RP2040.
Carregue o código na placa BitDogLab.
🖥️ Metodo alternativo:
Baixe o repositório com arquivo zip.
Extraia para uma pasta de fácil acesso
Utilize a extensão raspberry pi pico dentro do VS Code para importar o projeto.
Aguarde ate criar o arquivo build
Utilize o ícone "compile" para compilar.
Utilize o "RUN" com a BitDogLab em modo boot seel para enviar o programa para a sua RP2040.
Agora, interaja com os botões e o teclado para mergulhar nas funcionalidades do projeto.
🧑‍💻 Autor
José Ricardo de Souza Santos

📝 Descrição
Tarefa apresentada ao Cepedi como parte dos critérios de avaliação do curso EmbarcaTech em Software e Sistemas Embarcados, com foco na aplicação prática de comunicação serial via UART, I2C e SPI, e integração de hardware com o microcontrolador RP2040.

🤝 Contribuições
Este projeto foi desenvolvido por José Ricardo de Souza Santos. Contribuições são bem-vindas! Siga os passos abaixo para contribuir:

Fork este repositório.
Crie uma nova branch:
git checkout -b minha-feature
Faça suas modificações e commit:
git commit -m 'Minha nova feature'
Envie suas alterações:
git push origin minha-feature
Abra um Pull Request.
💡 Considerações Finais
Este projeto oferece uma ótima oportunidade para consolidar conhecimentos sobre comunicação serial,SPI e I2C, manipulação de hardware e desenvolvimento com microcontroladores.
