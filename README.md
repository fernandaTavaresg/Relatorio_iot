# Programação para Internet das Coisas
CURSO: TECNOLOGIA EM SISTEMAS PARA INTERNET

GRUPO: 

 FERNANDA BEATRIZ TAVARES GOMES

 POLIANA DE ARAUJO PEREIRA

TEMA: SERVIÇOS IOT E IMPLEMENTAÇÃO

### Introdução

Devido ao grande número de desperdicios com alimentos (frutas e legumes), que acontece diariamente, buscando formas de reduzir esses dados, seja no ambiente, transporte e até mesmo disponibilizando conhecimento para os transportadores, comerciantes e outros usuários. Como forma de solução a ideia é a criação de um pequeno projeto prático utilizando: Arduino Uno e sensor DHT11 (Umidade e temperatura), leds (amarelo e verde) e entre outro materias. Posteriomente a implementação com o Esp8266, para comunicação com MQTT.

Dentre os materiais e métodos para o desenvolvimento, também realizamos pesquisas diversas referente a construção e implementação do dispositivo em arduino, como os componentes utilizados, conexões e códigos; e também sobre o tema a ser desenvolvido, a conservação de frutas e hortaliças, condições que interferem nesses alimentos, dados referentes a temperatura, umidade relativa e ventilação do ar.

Descrevendo também sobre Serviços IoT que foram estudados, principalmente da Watson IBM e da Azure Microsoft, como eles são utilizados e como podem ser implementados no nosso projeto.

### Desenvolvimento

#### Implementação do dispositivo (Arduino)

Para a implementação do dispositivos utilizamos: 
- Arduino Uno
- Placa de Ensaio (Protoboard)
- Sensor DHT11 (Umidade e Temperatura)
- Leds (Amarelo e Verde)
- Servo Motor 
- Resistores (220Ohms e 10 k Ohms)
- Jumpers/fios (macho-macho)
- Cabo USB para Arduino

Na imagem a seguir, temos o dispositivo Arduino Uno que utilizamos e o sensor DHT11, que é a base do nosso projeto, para coleta de dados da temperatura e umidade, tendo uma faixa de temperatura entre 0ºC a 50ºC e de umidade relativa de 20% UR a 90% UR, e a conexão com cabo USB para carregar o programa apartir do computador.

![Imagem 3](Imagem3.jpg)

Fizemos a montagem do DHT11 ao Arduino, com o protoboard, um resistor de 10k Ohms. O DHT11 possui 4 pinos, sendo eles: o primeiro (VCC), sendo ligado a alimentação da placa 5V. O segundo é o de dados, que conectamos ao resistor e também ao pino 2 do Arduino. o terceiro (NC) não é utilizado. e o quarto conectado ao terra (GND).

Utilizamos o modelo de conexão da imagem 2.

![Imagem 2](Image2.jpg)
![Imagem 5](Image5.jpg)

Iniciamos também a inserção dos leds ao projeto, para avisar quando a umidade relativa estiver baixa (led amarelo) e alta (led verde). não conseguimos fazer funciona-los devido ao tempo. 

Para a conexão dos leds, utilizamos um resistor de 220Ohms para cada led e fios macho-macho, igual o modelo abaixo.

![Imagem 1](Imagem1.jpg)
![Imagem 6](Image6.jpg)

Também faremos a inserção do Servo Motor, para ser utilizado apartir de dados da temperatura para o acionamento de algum dispositivo de refrigeração, ventilador ou ar-condicionado.

Para ligar o Servo Motor ao Arduino, temos três pinos, sendo eles: um para alimentação no pino de 5V do Arduino, outro para o terra (GND) e o ultimo para o pino 9 porta digital do Arduino. Seguindo o modelo abaixo.

![Imagem 4](Image4.jpg)
![Imagem 7](Image7.jpg)

Para a programação do Arduino. Foi necessário para uma nova versão do programa 'Arduino', e duas bibliotecas para a utilização do sensor: a Biblioteca DHT11 e a AdaFruit. 

A seguir, temos o código utilizado para a execução do sensor. E Também a saída respectiva do sensor, apresentando a temperatura e umidade do ambiente.

![Imagem 9](image99.jpg)
![Imagem 8](image88.jpg)


#### Implementação do dispositivo (ESP8266)
Para a implementação do dispositivos utilizamos: 
- ESP8266
- Placa de Ensaio (Protoboard)
- Sensor DHT11 (Umidade e Temperatura)
- Resistores (220Ohms e 10 k Ohms)
- Jumpers/fios (macho-macho)
- Cabo USB para ESP8266


### Aplicação dos Serviços
### WATSON IBM
Possui diversas ferramentas que são bem completas e servem para ser implementadas por empresas. Baseado na computação cognitiva. Dentre alguns exemplos temos: reconhecimento de imagem, reconhecimento de voz, identificação de usuário, transformação de texto em voz e voz em texto, criação de chatbots e outros.
### Visual Recognition
Esta ferramenta  utiliza de deep learning. Quer dizer que é possível fazer análises de imagens. O serviço utiliza de classes padrão, tornando-o capaz de compreender o conteúdo de alguma imagem e também identifica palavras-chave para descrever a imagem. Taambém é possível treinar o Visual Recognition com imagens adicionadas pelo usuário e depois ajustar para que seja utilizada em algum domínio específico de aplicação, gerando classificadores personalizados.
#### Utilização
  
#### Implementação com projeto

### Language Translator
Capaz de traduzir textos entre vários idiomas diferentes e pode ser facilmente inserido em qualquer aplicação. 
#### Utilização
  
#### Implementação com projeto

### AZURE MICROSOFT
#### Utilização
  
#### Implementação com projeto
     
### Considerações finais

Buscando através desse projeto prático controlar os produtos e diminuir o desperdício. Emitindo dados do ambiente, relacionados a temperatura e umidade, com o objetivo de coletar esses dados e posteriormente enviar os dados obtidos para o broker MQTT e exibir em um dashboard para acesso dos usuários. Consiste na implementação dos dispositivos em Arduino e ESP8266, com sensor DHT11. Alguns pontos podem ser melhorados, como a implementação com motor servo e leds de sinalização, o envio correto para o MQTT, e a exibição na interface do Node-Red.

Como também é descrito sobre os serviços Iot, e sua utilização e possível implementação com o projeto. E como trabalhos futuros, realizar a implementação dos serviços com o projeto.



