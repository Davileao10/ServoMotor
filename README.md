# Controle de Servomotor por PWM com Raspberry Pi Pico W

## Descrição
Este projeto tem como objetivo a implementação de um controle de servomotor utilizando o módulo PWM (Pulse Width Modulation) do microcontrolador **RP2040** presente no **Raspberry Pi Pico W**. A simulação é realizada na plataforma **Wokwi**, permitindo testar o comportamento do servomotor em diferentes posições.

## Demonstração em Vídeo
Um vídeo demonstrando o funcionamento do projeto pode ser acessado no link abaixo:

🔗 **[Inserir link do vídeo aqui]**

## Requisitos
Para a realização desta atividade, foram definidos os seguintes requisitos:

1. Configurar a GPIO 22 com uma frequência PWM de aproximadamente **50Hz** (período de 20ms). *(20% da nota)*
2. Ajustar o ciclo ativo do PWM para **2.400µs** (duty cycle de 0,12%) para posicionar o servomotor em **180 graus** e aguardar 5 segundos. *(10% da nota)*
3. Ajustar o ciclo ativo do PWM para **1.470µs** (duty cycle de 0,0735%) para posicionar o servomotor em **90 graus** e aguardar 5 segundos. *(10% da nota)*
4. Ajustar o ciclo ativo do PWM para **500µs** (duty cycle de 0,025%) para posicionar o servomotor em **0 graus** e aguardar 5 segundos. *(10% da nota)*
5. Criar uma rotina para movimentar suavemente o servomotor entre **0 e 180 graus** com incrementos de **±5µs** a cada **10ms**. *(35% da nota)*
6. Testar o comportamento da iluminação do **LED RGB (GPIO 12)** utilizando a ferramenta educacional **BitDogLab** e documentar as observações. *(15% da nota)*

## Ferramentas Utilizadas
- **Microcontrolador:** Raspberry Pi Pico W
- **Linguagem:** C
- **Ambiente de Desenvolvimento:** VS Code
- **Kit de Desenvolvimento:** Pico SDK
- **Simulador:** Wokwi
- **Ferramenta Educacional:** BitDogLab

## Como Executar o Projeto
### Configuração do Ambiente
1. Instale o **VS Code** e o **Pico SDK**.
2. Configure o **Wokwi** para simulação do Raspberry Pi Pico W.
3. Clone este repositório:
   ```sh
   git clone https://github.com/Davileao10/ServoMotor.git
   cd ServoMotor
   ```
4. Compile o código utilizando o CMake:
   ```sh
   mkdir build
   cd build
   cmake ..
   make
   ```
5. Execute a simulação no Wokwi.

## Resultados
- O servomotor movimenta-se entre 0º, 90º e 180º conforme o controle PWM.
- O LED RGB (GPIO 12) apresenta alterações de iluminação durante o experimento com BitDogLab.

## Autor
Desenvolvido por **Davi Leão**.

